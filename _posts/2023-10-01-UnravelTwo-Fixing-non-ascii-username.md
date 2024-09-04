---
tags: windows
---

## The Unicode Problem in 2023
<img src="https://raw.githubusercontent.com/brocbyte/brocbyte.github.io/main/img/unravel.jpg" alt="UnravelTwo">

You launch a game, play for a while, exit. Relaunch and... nothing was saved :(

A problem might happened bc you're on windows and the game of yours handles unicode poorly (oh year 2023).

To fix it, you need to recreate windows user from scratch with proper eNgLisH-onLY letters in it.
Which is kinda lot just to play a game.

## Or...

You can debug the game a little!

Our patient, when opened using ImHex (strings search) shows this:

<img src="https://raw.githubusercontent.com/brocbyte/brocbyte.github.io/main/img/unraveltwo_binary.png" alt="ImHex output">

We've got an 'LOCALAPPDATA' entry here. It is a name of an environmental variable on Windows, pointing to personal user's folder.

The thing is, when a program wants to save sth for a single user (like a game's progress), it often has to query the OS for some env variable, which points to an appropriate location.

We cannot actually edit particularly 'LOCALAPPDATA' one using standard 'Edit the system environment variables' Windows's dialog, for some reason.

## Getting to know each other

So, what do we do? WinAPI provides several ways for quering environment variables:

* DWORD GetEnvironmentVariable(LPCTSTR lpName, LPTSTR  lpBuffer, DWORD   nSize);

* LPCH GetEnvironmentStrings();

The first one returns the value of a particular variable, the second lists all of them.

Our game has to use some of those to save our progress correctly.
We will use http://www.rohitab.com/apimonitor to determine which one actually. It allows you to take a look into api-calls that a program is doing.

For e.g. we will add both GetEnvironmentVariable() and GetEnvironmentStrings() for monitoring and then launch our program.
In the output we don't see a single GetEnvironmentVariable() call with 'LOCALAPPDATA' as an argument, so it gets all the information it needs by calling GetEnvironmentStrings().
If we were to enable C++RuntimeFunctions tracing too, we would actually see some 'strcmp'-family functions being called on the returned value of GetEnvironmentStrings() :)

We could modify the actual return value of this function somehow (dll injection?), but we're stupid and lazy...

Or, we can go a much simpler way and just create our brand new own environment variable 'COCALAPPDATA'! Naming is poor sry. Important: the length of the name must be kept the same.

So we open our game.exe once again using ImHex. 'LOCALAPPDATA' entry found previously can be easily patched to 'COCALAPPDATA', bc it lies in some .data region.

Then we just set a new environment variable using standard windows dialog - and sheesh, saving system is working!

### A note

The thing is, we didn't do anything hard at all and got the good result. Environment variables are cool!
---
tags: Induction
---

> Whether we are a detective trying to catch a thief, a scientist trying to discover a new physical law, or a businessman attempting to understand a recent change in demand, we are all in the process of collecting information and trying to infer the underlying causes.
>
> _-Shane Legg_

based on https://www.lesswrong.com/posts/Kyc5dFDzBg4WccrbK/an-intuitive-explanation-of-solomonoff-induction

## Human's Induction

So, we've got some Data, produced by some algorithm: [1, 3, 5, 7] - our observations of the real world.

The question is: *what is the next number in a sequence? - what will happen in the future?*

Your perfectly balanced Occam’s Razor tells you: man it's just the list of odd numbers, go on, be sure!

So, you type '9' in an Answer Box. Machine beeps 'yo dump ass' and makes some Glados-like jokes. You failed.

The underlying number generation program was kinda simple too: 2n − 1 + (n − 1)(n − 2)(n − 3)(n − 4).

## What to do

You lost. Lost to the Machine. What'll u do about it?

Ray Solomonoff has already come up with a solution for you: Solomonoff induction.

Firstly we reformulate the problem statement slightly: you can't know 4 sure what's the real answer is, but u can get your _best guess_.

Our final answer will consist of several hypotheses together with their probabilities of occurrence.

For example, in our situation set of possible answers could look like that:

    'odd numbers': 0.8;

    '2n − 1 + (n − 1)(n − 2)(n − 3)(n − 4)': 0.05;

    ... go on ...

List of possible hypotheses is formed from the list of all possible turing machines: if a given turing machine halts with the desired output (1, 3, 5, 7), then it's interesting for us and we're happy to keep it.

Each turing machine T with Data on its output tape is assigned with probability 1 / 2^(len(T)). That's the way of sticking to easier explanations (do not yet throw away your amazon-delivered Occam's Razor :)).

## The bad news

Of course this thing is incomputable, like most of the funny ones.
You can't filter all turing machines by their output, the halting problem in its core.

However, there are ways to approximate it. This way, approximate predictions of the future.
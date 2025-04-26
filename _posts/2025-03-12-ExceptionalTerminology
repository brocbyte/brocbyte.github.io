---
tags: windows
---

## Hardware/OS exceptions:

### interrupts

Interrupts occur asynchronously as a result of signals from I/O devices that are external to the processor. Hardware interrupts are asynchronous in the sense that they are not caused by the execution of any particular instruction. 
Always returns to the next instruction.

### traps / syscalls
Traps are intentional exceptions that occur as a result of executing an instruction. Used to implement system calls.
Always returns to the next instruction.

### faults
Faults result from error conditions that a handler might be able to correct. When a fault occurs, the processor transfers control to the fault handler. If the handler is able to correct the error condition, it returns control to the faulting instruction, thereby _reexecuting_ it. Otherwise, the handler returns to an 'abort' routine in the kernel that terminates the application program that caused the fault.
Might return to current instruction.

### aborts
Aborts result from unrecoverable fatal errors, typically hardware errors
Never returns control to the application program.

### Signals = OS way to notify user processes about events

#### Group [SIGFPE, SIGILL, SIGSEGV]
Low-level hardware exceptions are processed by the kernel’s exception handlers and would not normally be visible to user processes. Signals provide a mechanism for exposing the occurrence of such exceptions to user processes. 

#### Group [SIGINT, SIGKILL, SHIGCHLD]
Other signals correspond to higher-level software events in the kernel or in other user processes

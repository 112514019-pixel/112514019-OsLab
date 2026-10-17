# PROGRAM 4 : PROCESS CREATION AND MANAGEMENT USING LINUX SYSTEM CALLS

## AIM :
To study process creation, execution, and synchronization using Linux process system calls:
• fork()
• exec()
• wait()
• getpid()
• getppid()
and to understand parent-child process relationships.

## CONTEXT :
A process is a program that is currently being executed. Linux allows a process to create another process (called a child process) and manage its execution.

## LINUX SYSTEM CALLS USED :

| System Call | Function |
|---|---|
| `fork()` | Creates a new child process by duplicating the current (parent) process. |
| `getpid()` | Returns the Process ID (PID) of the currently executing process. |
| `getppid()` | Returns the Process ID (PID) of the parent process. |
| `wait()` | Suspends the parent process until the child process terminates. |
| `sleep()` | Suspends the execution of the current process for the specified number of seconds. *(Library function that internally uses kernel timing services; often included in OS labs.)* |

## SOURCE CODE (Process Creation) :
**File:** [forkDemo.c](https://github.com/sumaiyasumai2711-arch/osLab/blob/ebc4bf3495aaaf2496964309063db46434662fbc/ex04/ProcessCreation/forkDemo.c)

## COMPILATION :

```bash
gcc forkDemo.c -o forkDemo
```

## EXECUTION :

```bash
./forkDemo
```
## OUTPUT :
![Output for Experiment 4_1](https://github.com/112514019-pixel/112514019-OsLab/blob/07284d97034a26bac02d0d103da32a54ebe92ac9/ex04/ProcessCreation/image.png)

## SOURCE CODE (Process Management) :
**File:** [waitDemo.c](https://github.com/sumaiyasumai2711-arch/osLab/blob/5a6877d0896728f0c00778351d044b218bb206b0/ex04/ProcessManagement/waitDemo.c)

## COMPILATION :

```bash
gcc waitDemo.c -o waitDemo
```

## EXECUTION :

```bash
./waitDemo
```

## OUTPUT :
![Output for Experiment 4_2](https://github.com/112514019-pixel/112514019-OsLab/blob/455a9ff50daf94a7e5efe17ad2aaf59703eccec1/ex04/ProcessManagement/image.pngg)

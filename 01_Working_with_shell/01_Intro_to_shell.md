# Introduction to Shell in Linux

A shell is a program that takes the commands we type and asks the Linux operating system (the kernel) to run them. It is also called a command-line interpreter. The most common shell on Linux is **Bash** (`/bin/bash`).

## Types of Shell Commands

1. Built-In Commands
2. External Commands

## 01 Built-In Commands

These are commands that are built into the shell program itself. The shell runs them directly, without starting a separate program, so they are fast. They are part of the shell (for example Bash), not of the Linux distribution.

### Some Examples of Built-In Commands

1. **`echo`**: This command is used to print text in the shell.
2. **`cd`**: This command is used to change the working directory.
3. **`pwd`**: This command is used to print the present working directory.

## 02 External Commands

These are commands that are not part of the shell. Each one is a separate program (an executable file) stored on disk, usually in directories like `/bin` or `/usr/bin`. The shell finds them by searching the directories listed in the `PATH` variable. Most common ones come pre-installed with the system (for example in the `coreutils` package); others can be installed with a package manager such as `apt` or `yum`.

### Some Examples of External Commands

1. **`mv`**: This command is used to move a file from one directory to another directory. It is also used to rename a file.
2. **`cp`**: This command is used to copy a file from one directory to another directory.
3. **`date`**: This command is used to print the current local date and time of the system.
4. **`uptime`**: This command is used to check how long the system has been running since the last reboot.

## How to Check the Type of a Command

Use the `type` command to see whether a command is built-in or external:

```bash
type echo     # echo is a shell builtin
type mv       # mv is /usr/bin/mv
```

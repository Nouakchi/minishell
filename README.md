# Minishell - A Simple Shell Implementation

## Summary

Minishell is a project focused on creating a simple shell, akin to Bash, where you will learn about processes and file descriptors.

## Version

Version: 7.1

## Contents

- [Chapter I - Introduction](#chapter-i-introduction)
- [Chapter II - Common Instructions](#chapter-ii-common-instructions)
- [Chapter III - Mandatory Part](#chapter-iii-mandatory-part)
- [Chapter IV - Bonus Part](#chapter-iv-bonus-part)
- [Chapter V - Submission and Peer-evaluation](#chapter-v-submission-and-peer-evaluation)

## Chapter I - Introduction

Minishell allows you to create a shell environment where users can interact with the operating system using command lines. It's a fundamental part of Unix-like systems, providing a command-line interface.

## Chapter II - Common Instructions

- Your project must be written in C.
- Adhere to the Norm for coding style and conventions.
- Functions should handle errors gracefully without crashing.
- All dynamically allocated memory must be freed appropriately to avoid leaks.
- Use a Makefile to compile your project with flags `-Wall -Wextra -Werror`.
- Makefile must include: `$(NAME)`, `all`, `clean`, `fclean`, `re`.
- Include a `bonus` rule in Makefile for bonus functionalities.

## Chapter III - Mandatory Part

### Program Details

Program name: `minishell`

### Turn in files

- `Makefile`
- `*.h`, `*.c`

### Makefile Requirements

- `NAME`, `all`, `clean`, `fclean`, `re`

### Arguments

External functions allowed:
`readline`, `rl_clear_history`, `rl_on_new_line`, `rl_replace_line`, `rl_redisplay`, `add_history`, `printf`, `malloc`, `free`, `write`, `access`, `open`, `read`, `close`, `fork`, `wait`, `waitpid`, `wait3`, `wait4`, `signal`, `sigaction`, `sigemptyset`, `sigaddset`, `kill`, `exit`, `getcwd`, `chdir`, `stat`, `lstat`, `fstat`, `unlink`, `execve`, `dup`, `dup2`, `pipe`, `opendir`, `readdir`, `closedir`, `strerror`, `perror`, `isatty`, `ttyname`, `ttyslot`, `ioctl`, `getenv`, `tcsetattr`, `tcgetattr`, `tgetent`, `tgetflag`, `tgetnum`, `tgetstr`, `tgoto`, `tputs`

### Description

Minishell functionalities:
- Display a prompt when waiting for a new command.
- Implement a working history feature.
- Execute commands using PATH variable or specified paths.
- Handle single and double quotes to interpret meta-characters appropriately.
- Implement redirections: `<`, `>`, `<<`, `>>`.
- Implement pipes (`|`) for command chaining.
- Expand environment variables (`$VAR`) and special variables (`$?`).
- Handle signals: ctrl-C, ctrl-D, ctrl-\.
- Implement built-in commands: `echo`, `cd`, `pwd`, `export`, `unset`, `env`, `exit`.

### Evaluation

Ensure all requirements are met, following behavior similar to Bash where applicable.

## Chapter IV - Bonus Part

### Additional Features (Optional)

Enhance your Minishell with:
- Implementing `&&` and `||` with parentheses for command priorities.
- Support for wildcards (`*`) in current working directory.

### Note

Bonus part evaluated only if mandatory part is perfect.

## Chapter V - Submission and Peer-evaluation

Submit your work to the assigned git repository. Only the work in the repository will be graded. Peer evaluations may follow before final grading.


# OSSP Practical Session 9

## File Copy Using Low-Level Linux I/O and Standard Library I/O

### Objective

This practical implements file copying using:

- Low-level Linux system calls
- C standard library I/O
- `lseek()` for file offset manipulation
- Performance comparison using `time`
- `dup2()` for standard input and output redirection

## 1. Low-Level File Copy

Program:

`copy_lowlevel.c`

Uses:

- `open()`
- `read()`
- `write()`
- `lseek()`
- `close()`

Compile:

```bash
gcc -Wall -Wextra -O2 copy_lowlevel.c -o copy_lowlevel

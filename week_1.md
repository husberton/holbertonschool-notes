# A Beginner-Friendly Guide to the Shell, vi, and Git

## Introduction

Computers may look simple on the outside, but underneath the graphical
interfaces you click on every day is a powerful text-based world called
**the shell**. Developers use it because it's fast, flexible, and gives
full control over the system. Alongside the shell, there are tools like
**vi**, a classic text editor, and **Git**, the world's most popular
system for tracking changes in code.

------------------------------------------------------------------------

# 1. Shell: Navigation and Basics

## What Is the Shell?

The shell is a program that takes commands you type and tells the
computer what to do. When you open a Terminal app, you're looking at the
shell prompt---that small blinking line waiting for a command.

### Terminal vs Shell

-   **Terminal** = the window/program you type into\
-   **Shell** = the interpreter running inside the terminal

### Shell Prompt

Often looks like:

    username@computer:~$

### History

Press `↑` and `↓` to scroll through old commands.

------------------------------------------------------------------------

## Navigation Commands

  Command   Description
  --------- -------------------------
  `pwd`     Print working directory
  `ls`      List files
  `cd`      Change directory

### Special Directories

-   `.` = current directory\

-   `..` = parent directory\

-   `~` = home directory\

-   `/` = root directory

-   Hidden files start with `.`\

-   `cd -` switches to your previous location

------------------------------------------------------------------------

# 2. Looking Around the System

### Useful Commands

-   `less` --- view files\
-   `file` --- check file type\
-   `ln` --- create links

### Hard vs Symbolic Links

-   **Hard link**: another name for the same data\
-   **Symbolic link**: a shortcut

### Common Directories

-   `/bin`, `/etc`, `/home`, `/var`, `/usr`

------------------------------------------------------------------------

# 3. Manipulating Files

### Commands

-   `cp` --- copy\
-   `mv` --- move/rename\
-   `rm` --- delete\
-   `mkdir` --- create directory

### Wildcards

-   `*` matches anything\
-   `?` matches one character

------------------------------------------------------------------------

# 4. Working With Commands

### Help Tools

-   `man` --- manual pages\
-   `help` --- shell built-ins\
-   `type` --- tells what a command is\
-   `which` --- shows where a command is stored

### Aliases

Shortcuts for commands.

### Man Page Sections

-   **1**: user commands\
-   **2**: system calls\
-   **3**: library functions

------------------------------------------------------------------------

# 5. Shell Permissions

Every file has permissions for: - **owner** - **group** - **others**

### Permission Values

-   `4` = read\
-   `2` = write\
-   `1` = execute

### Commands

-   `chmod`\
-   `chown`\
-   `chgrp`\
-   `sudo`\
-   `su`

Regular users cannot change ownership (`chown`) of files they don't own.

### Other Useful Commands

-   `id`\
-   `groups`\
-   `useradd`\
-   `groupadd`

------------------------------------------------------------------------

# 6. Shell I/O, Redirection, and Filters

### Common Tools

-   `head`, `tail`, `grep`, `sort`, `uniq`, `wc`, `tr`, `find`

### Redirection

-   `>` write to file\
-   `>>` append\
-   `<` read input from file

### Pipes

    ls | grep ".txt"

### Special Characters

Quotes, escape characters, comments, pipes, semicolons, tilde.

### Important Files

-   `/etc/passwd`\
-   `/etc/shadow`

------------------------------------------------------------------------

# 7. vi Editor

Created by **Bill Joy**.

### Starting / Exiting

    vi filename
    :q
    :q!
    :wq

### Modes

-   **Normal mode**
-   **Insert mode**

Switch: - Normal → Insert: `i`\
- Insert → Normal: `Esc`

### Editing

-   `dd` --- delete line\
-   `p` --- paste\
-   `u` --- undo\
-   `/text` --- search forward\
-   `?text` --- search backward

------------------------------------------------------------------------

# 8. Git and GitHub

### Git

A version control tool.

### GitHub

A website that hosts Git repositories.

### Creating a Repo

    git init

### Commit

    git add .
    git commit -m "message"

### Push and Pull

    git push
    git pull

### Branches

    git branch
    git checkout
    git merge

### What Not to Commit

-   passwords\
-   large binaries\
-   compiled files

------------------------------------------------------------------------

# 9. Other Concepts

### Shebang

Specifies interpreter:

    #!/bin/bash

### RTFM

Read The Manual.

### LTS

Long-Term Support.

------------------------------------------------------------------------

# Conclusion

Mastering the shell, vi, and Git builds a strong foundation for becoming
a capable developer.

# MiX_Examples (Work in Progress)

## Overview
The MiX_Examples package provides guides for beginners on Python and Linux operation systems to help them get involved in MiX analysis.

## Linux

### Linux Commands Guide

#### Navigation
- `pwd` : Print current working directory.
- `ls` : List directory contents.
- `cd <directory>` : Change directory to \<directory\>.
- `mkdir <directory>` : Create a new \<directory\>.
- `rmdir <directory>` : Remove an empty \<directory\>.

#### File Operations
- `touch <file>` : Create a new empty \<file\>.
- `cp <source> <destination>` : Copy file or directory from \<source\> to \<destination\>.
- `mv <source> <destination>` : Move or rename file or directory from \<source\> to \<destination\>.
- `rm <file>` : Remove the \<file\>.
- `rm -r <directory>` : Remove the \<directory\> and all its contents. (Be careful about the \<directory\> you are removing, since it will delete files permanently)

#### Viewing and Editing Files
- `cat <file>` : View \<file\> contents.
- `nano <file>` : Edit \<file\> with Nano editor.
- `vim <file>` : Edit \<file\> with Vim editor.
- `head <file>` : View the first 10 lines of the \<file\>.
- `tail <file>` : View the last 10 lines of the \<file\>.

#### System Information
- `df -h` : Show disk space.
- `top` : Display all running processes.

#### Permissions
- `chmod <permissions> <file>` : Change \<file\> permissions to \<permissions\>.
- `chown <user>:<group> <file>` : Change \<file\> owner to \<user\> and group to \<group\>.

#### Package Management (We won't use it on GreatLakes, but yes on local machines)
- `sudo apt update` : Update package lists.
- `sudo apt upgrade` : Upgrade installed packages.
- `sudo apt install <package>` : Install a new \<package\>.
- `sudo apt remove <package>` : Remove the \<package\>.

#### Searching
- `grep <pattern> <file>` : Search for the \<pattern\> in the \<file\>.
- `find <directory> -name <filename>` : Find files and directories.

#### Miscellaneous
- `echo <text>` : Print text to the terminal.
- `man <command>` : Display manual for a command.
- `history` : Show command history.

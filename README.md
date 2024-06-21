# MiX_Intro (Work in Progress)

## Overview
The MiX_Intro package provides guides for beginners on Python and Linux operation systems to help them get started on MiX analysis.

1. [Linux](#linux)
   - [Linux Command Lines](#linux-command-lines)
1. [Git](#git)

## Linux

### Linux Command Lines
Some commonly used Linux commands and their options (flags) are:

#### Navigation
- `pwd` : Print current working directory.
- `ls` : List directory contents.
  - `-l` :	Display in long list format.
  - `-a` :	Display hidden contents.
  - `-r` :	Display in reverse order.
  - `-t` :	Display in time order.
  - Above options can be combined, for example: `ls -lrt` is display in long list format and in reverse time order.
- `cd <directory>` : Change current working directory to \<directory\>.
- `mkdir <directory>` : Create a new \<directory\>.

#### File Operations
- `touch <file>` : Create a new empty \<file\>.
- `cp <source> <destination>` : Copy file or directory from \<source\> to \<destination\>.
- `mv <source> <destination>` : Move or rename file or directory from \<source\> to \<destination\>.
- `rm <file>` : Remove the \<file\>.
  - `-r` : Recursively, typically used when removing directories; i.e. `rm -r <directory>`. Be careful about the \<directory\> you are removing, since Linux will delete files permanently.

#### Viewing and Editing Files
- `cat <file>` : View \<file\> contents.
- `vim <file>` : Edit \<file\> with Vim editor.
- `head <file>` : View the first 10 lines of the \<file\>.
- `tail <file>` : View the last 10 lines of the \<file\>.

#### System Information
- `df -h` : Show disk space.
- `top` : Display all running processes.

#### Searching
- `grep <pattern> <file>` : Search for the \<pattern\> in the \<file\>.
- `find <directory> -name <filename>` : Find files and directories.

#### Displays
- `echo <text>` : Print \<text\> to the terminal.
- `man <command>` : Display manual for \<command\>.
- `history` : Show command history.

#### Permissions (Not used often since MiX codes are for everyone in the group)
- `chmod <permissions> <file>` : Change \<file\> permissions to \<permissions\>.
  - `0`: no permission.
  - `1` or `x` : execute.
  - `2` or `w`: write.
  - `4` or `r`: read.
  - If using digits, you need to add them up and put them in `user-group-others` order. For example, `chmod 751` means "user can read, write execute; group can execute and read; others can only execute".
- `chown <user>:<group> <file>` : Change \<file\> owner to \<user\> and group to \<group\>.


## Git
Since you are here, you should already know what is Git and some basic command lines for Git.
Below are some quick reminders of the basic Git commands and their options.

#### Initialization
- `git init` : Initialize a new Git repository.
- `git clone <repository>` : Clone an existing repository from a URL (now only supports SSH).

#### Configuration
- `git config --global user.name "<name>"` : Set Git user name.
- `git config --global user.email "<email>"` : Set Git user email.

#### Changing Files
- `git status` : Show the working directory status, like file changes.
- `git add <file>` : Stage a \<file\> for commit.
- `git commit -m "<message>"` : Commit changes with a message.
- `git push origin <branch>` : Push changes to the remote \<branch\>.
- `git pull origin <branch>` : Pull changes from the remote \<branch\>.
- `git log` : Show commit history.

#### Branching (We don't need to worry about it on MiX since we only use the `master` branch)
- `git branch` : List Git branches.
- `git branch <branch>` : Create a new branch named \<branch\>.
- `git checkout <branch>` : Switch to the \<branch\>.
- `git merge <branch>` : Merge \<branch\> into the current branch.

#### Undoing Changes
- `git checkout -- <file>` : Discard changes in a \<file\> and use the version on Git.


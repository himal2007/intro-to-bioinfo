# Introduction to shell
## Introduction
### Why shell?
- lots of functionalities
- Automate repetitive tasks - thus makes bioinformatics less boring - reduces error
- Accessing remote computer
- Reproducible when working in command line rather that GUI

### Accessing shell
- Mac or Linux machine: Access via Terminal
- Windows: Access via PuTTy
	- IP address `ec2-user@203.101.228.128` and PW: `combine2021`
	- SSH - `22`
	- Press `Open`
## Navigating files and directories
- `pwd` - print where we are, i.e. current working directory
- `ls` - flags `-`
	- `man ls` - you can navigate through the documentation and know the purpose of each flags
	- Exercise: Use the `-l` option for the `ls` command to display more information for each item in the directory. What is one piece of additional information this long format gives you that you don’t see with the bare `ls` command?
		- Answer: The additional information given includes the name of the owner of the file, when the file was last modified, and whether the current user has permission to read and write to the file.
	- Shortcut: Tab Completion 
		- Makes you more efficient
		- autocomplete the name of the command or the directories

> ## Challenge
> Use the `-l` option for the `ls` command to display more information for each item 
> in the directory. What is one piece of additional information this long format
> gives you that you don't see with the bare `ls` command?
>
> > ## Solution
> > ~~~
> > $ ls -l
> > ~~~
> > {: .bash}
> > 
> > ~~~
> > total 8
> > drwxr-x--- 2 dcuser dcuser 4096 Jul 30  2015 sra_metadata
> > drwxr-xr-x 2 dcuser dcuser 4096 Nov 15  2017 untrimmed_fastq
> > ~~~
> > {: .output}
> > 
> > The additional information given includes the name of the owner of the file,
> > when the file was last modified, and whether the current user has permission
> > to read and write to the file.
> > 
> {: .solution}
{: .challenge}

- `man`
- `cd`
- Full vs relative path `~`: home directory and `/`: root directory  and `.`: current directory, `..`: back one level
- Tab completion, Command history
- Wild cards
- Creating, moving, copying and removing directory
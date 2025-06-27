# **Unix**
#unix, #linux
The Unix operating system is a set of programs that act as a link between the computer and the user.

The computer programs that allocate the system resources and coordinate all the details of the computer's internals is called the **operating system or the kernel.**

Users communicate with the kernel through a program known as the **Shell**. The shell is a command line interpreter; it translates commands entered by the user and converts them into a language that is understood by the kernel.

## Unix Architecture
![Pasted image 20240806230324](https://github.com/user-attachments/assets/32385848-73f1-4359-83a7-a50a2959100f)

**Kernel** − The kernel is the heart of the operating system. It interacts with the hardware and most of the tasks like memory management, task scheduling and file management.

**Shell** − The shell is the utility that processes your requests. When you type in a command at your terminal, the shell interprets the command and calls the program that you want. 
The shell uses standard syntax for all commands. C Shell, Bourne Shell and Korn Shell are the most famous shells which are available with most of the Unix variants.

**Commands and Utilities**
There are various commands and utilities which you can make use of in your day to day activities. **cp**, **mv**, **cat** and **grep**, etc. are few examples of commands and utilities. There are over 250 standard commands plus numerous others provided through 3rd party software. All the commands come along with various options.

**Files and Directories**
All the data of Unix is organized into files. All files are then organized into directories. These directories are further organized into a tree-like structure called the **filesystem**.
## Features of UNIX:
1. **Multiuser support:** UNIX allows multiple users to simultaneously access the same system and share resources.
2. **Multitasking:** UNIX is capable of running multiple processes at the same time.
3. **Shell scripting:** UNIX provides a powerful scripting language that allows users to automate tasks.
4. **Security:** UNIX has a robust security model that includes file permissions, user accounts, and network security features.
5. **Portability:** UNIX can run on a wide variety of hardware platforms, from small embedded systems to large mainframe computers.

##  History of Unix:

·       **001-Unix** is an operating system which was first developed in the 1960s, and has been under constant development ever since. By operating system, we mean the suite of programs which make the computer work.

·       **MULTIX** The multi-user, multi-tasking operating system. You can have many users logged into a system simultaneously, each running many programs was named as.

·       First Version of Unix was created in Bell Labs in 1969. 
	Some of the Bell Labs programmers who had worked on this project, Ken Thompson, Dennis Ritchie, Rudd Canaday, and Doug McIlroy designed and implemented the first version of the Unix File System on a PDP-7 along with a few utilities. It was given the name UNIX by Brian Kernighan.

·       1973 Unix is re-written mostly in C, a new language developed by Dennis Ritchie.

·       1977 There were about 500 Unix sites world-wide.

·       1980 BSD 4.1 (Berkeley Software Development)

·       1983 SunOS, BSD 4.2, System V

·       1988 AT&T and Sun Microsystems jointly develop System V Release 4 (SVR4). This later developed into UnixWare and Solaris 2.

·       1991 Linux was originated.
## Unix File Structure
Users interact with the Unix environment through the shell, a CLI for entering commands that are passed to the kernel for execution. A command is used to invoke one of the available utilities. Each utility carries out a specific operation, such as creating files, deleting directories, retrieving system information or configuring the user environment.

In addition, the Unix shell supports the use of pipes **(|)**, a powerful tool for linking multiple commands to create complex workflows. When two or more commands are piped together, the output from the first command is used as input for the second command, the output from the second command is used as input for the third command and so on.

Another important Unix feature is the file system, which provides a hierarchical structure for working with files. The file system organizes directories into an inverted tree with the root directory at the top. Files are then assigned to specific directories and accessed through the directory structure. Previous operating systems divided a storage device into sections by a fixed number of levels.

Unix treats all types of files as simple byte arrays, resulting in a much simpler file model than those in other operating systems. Unix also treats devices and certain kinds of interprocess communication as files.

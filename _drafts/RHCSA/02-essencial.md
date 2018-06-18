---
title: "2 - Using Essential Tools"
excerpt: "This certification guide will provide a comprehensive overview of Red Hat Enterprise Linux, RHEL 7,
covering the EX200 exam topics, in order to be a RHCSA - Red Hat Certified System Administrator Guide."
last_modified_at: 2018-01-02 21:28:04 +00:00
toc: true
---

## RHCSA Objectives
* Access a shell prompt and issue commands with correct syntax
* Use input-output redirection `(>, >>, |, 2>, etc.)`
* Use grep and regular expressions to analyse texta
* Access remote systems using ssh
* Log in and switch users in multiuser targets

* Archive, compress, unpack, and uncompress files using tar, star, * gzip, and bzip2

* Create and edit text files
* Create, delete, copy, and move files and directories

* Create hard and soft links
* List, set, and change standard ugo/rwx permissions
*
* Locate, read, and use system documentation including man, info, and files in `/usr/share/doc`


## Seccions

### Accessing the command Line using the local console

* Access a shell prompt and issue commands with correct syntax

#### The Command line
A commmand line is a text based interface wich can be used to input instructions to a computer, provided by the program interpreter **shell**. The default shell for RHEL is *bash* (Bourne-Again Shell), an inproved version of the *sh* (Bourne Shell).

when using a shell interactivelly, it displays a string, warning for a command, the *shell prompt*. When using a regular user, the prompt is the `$` character.
```console
marcelo@mo:~$
```
The `$` is replaced by `#`, if the you are the *superuser*, root, to avoid accidents
```console
root@mo:~#
```


The shell makes a difference between three kinds of commands:
* An *alias* is a command that a user can define as needed and are executed before anything else. 
It's usually used as way to subsitute long commands, such as `alias ll='ls -l --color=auto'`. You can use the `alias` command to check the alias currently defined.
* An *internal command* is a command that is a part of the shell itself. It is available when the shell is loaded and can be executed from memory without any lookup from disk.
* An *external command* is a command that exists as an executable file on disk of the computer. The shell first looks to determine whether it is an internal command. If not, looks for an executable file with a matching filename in the list of directories defined by the `$PATH` variable.

To find out the type of command you are using, you can use the `type` command and to find out which exact command the shell will be using, you can use the`which` command.




* Access remote systems using ssh


##

### Laboratory

* [1.1 lab - Initial Setup](/RHCSA/02.01-essencial-lab/)

### Pratice

* [1.1 lab - Initial Setup](/RHCSA/02.01-essencial-ex/)
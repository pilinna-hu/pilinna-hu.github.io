---
layout: default
---

# Command-line course for linguists

The course consisted of three main topics that were in a very interesting way dispersed in the course weeks. This page presents the actual content of the course, not its structure.

### The main topics

- how to work in a Unix like environment and the command line
- how to develop tools
- how to work with strings

## How to work in a Unix like environment and the command line

The first one had as the starting point that the participants are familiar with computers but have only used Windows or Mac with a graphical user interface. Quite many of the tools that have been developed for working with text data are actually built to be run in a Unix like environment and meant to be operated from the command line, and therefore one of the main goals of the course was to familiarise the participants with the command line in a Unix like environment.

In a Unix like environment it is important to be able to manage and access the files one is working with and therefore the participants would train managing the directory structure and moving around in it as a basic skill. As another basic skill the participants were told how to manage files in the direcory structure: creating a file, checking the basic information or the contents of a file, moving, renaming and deleting files. Also the possibility to use remote servers was presented.

Specific contents of this part were about the commands with which it is possible to get these things done (mkdir, rmdir, cd, mv, cp -R, rm, rm -R, ssh, scp) and understanding the basic direcotry structure (/tmp, /usr/, /bin, /home).

- an example: $ mkdir feedback
- this command is fed on the Bash command-line, hence the dollar sign. The actual command "mkdir feedback" creates a new directory called "feedback" into the current directory, i.e., the directory wheer the user is when giving this command

There was also the idea of learning how to manage the computing environment on a higher level. The participants were taught how to control the access rights to files and directories and how to install and run programs. There was also a brief look into the Unix environment and the dependencies between the different components, and as part of this the participants learned how to create and activate virtual environments.

Specific contents of this part were about the commands with which it is possible to get these things done (chmod, sudo, apt-get, brew, pip, pip install, python -m venv, source) and understanding that programs need certain versions of packages to be installed in their running environment.

- an example: $ sudo apt-get install nltk 
- the part "sudo" (superuser do) means that this command is given with temporary root priviledges, the "apt-get" means that some sort of package should be fetched and loaded to the computer and "install" that it should be installed as well. Here the package is "nltk": the natural language toolkit  

Active programs run as processes and it is possible to manage them as such. This way of looking at programs is also possible for example in Windows but it is the native way of relating to running programs in a Linux like environment when using the command line as the interface. Therefore the participants were also taught how to identify and manage the processes that relate to the programs of interest.

Specific contents of this part were about the commands with which it is possible to get these things done (ps, top, kill, ) and understanding that processes can sometimes become orphans and get stuck and need to be shutdown with a command.

- an example: $ kill 451
- if e.g. process 451 is nano, then this would stop the text processor program nano and return the command-line view with the dollar sign

## How to develop tools

The course was not concentrating on developing sizable programs with a dedicated programming language, but it teach how to collect operations into a pipeline that can be run as a command on the command line and also how to write scripts that can be run in the Bash. It also paved the way for even more ambitious development work by introducing version control as a concept and also a tool for controlling the versions, the git. These were maybe a bit out of sync as needs and tools, the developmental work being so small, but I think it makes sense to learn to use version control tools at the go while learning how to develop more complicated programmatic entities.

Specific contents of this part were about the commands with which it is possible to get these things done (git init, git clone, git status, git add, git commit, git log, git branch, git merge, git push). We also learned how to work with Github, graphical interface to the material that at the same time functions as a social hub for developers.

- an example: $ git commit -m "Personalisation"
- this would make the added changes to the current branch, register those changes and the comment "Personalisation" relating to those changes

## How to work with strings

We also learned how to work with character-based material, texts, words or ”strings”. On the other hand we learned how to look at the contents of text files (cat, less), and we also learned how to create or modify them with a command-line text processor (nano). This was a good warm-up but the actual core of the core of the course was to learn how to operate on files that contain vast amount of character-based material.

Here the foundation was to understand that the various writing systems need to be somehow encoded, in order for a text written in them to be possible to be stored in a file. And a moment of meta-learning was that there are always multiple not that easily compatible solutions to all needs in the world of computers and programs. So we learned how to find out the encoding format of the text-file, and how to change it from one format to another.

Specific contents of this part were about the commands with which it is possible to get these things done (file, iconv, dos2unix, unix2dos). We also learned about Unicode and its different versions.

- an example: $  file katinka_rabe.utf-8.txt
- this command would return the information about the mentioned textfile, for example "Unicode text, UTF-8 text"

Then we learned finding and manipulating of text files on multiple different levels. There seemed to be commands that were built in to Bash and that didn’t do very complicated things (head, tail, wc, sort) and then there were comands that were actulally very diverse programs in their own right, where we only learned one or two aspects of (sed). And we had a brief look into the powerhouse of operations on text-based material; the regular expressions.

Specific contents of this part were about the commands with which it is possible to get these things done (sed, grep). We also learned about Posix as (among other things) an underlying language for referring to sets of characters.

### Regular expressions, examples of symbols

|Anchors|Quantifiers|Character classes|
|-------|-----------|-----------------|
| ^ | * | . |
| \A | + | (a\|b) |
| $ | ? | (...) |


## Credits and responsibility

All observations and opinions are those of the author.

![author](assets/img/me.jpg)

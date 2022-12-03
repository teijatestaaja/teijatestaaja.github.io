---
layout: default
---

## Command-line Tools for Linguists

This document is a description of what I have learned during the Command-line Tools for Linguists 2022. The course was organised by University of Helsinki as a web course. It is a course designed for students interested in command-line tools that can be used for example in language text file processsing. The course covered the following topics:

<img src="assets/images/syllabus.png" alt="Course syllabus" hspace="30" width="60%">

## Week 1

The first week was an introduction to command-line environments. The first task was to install [Windows Subsystem for Linux (WSL)](https://ubuntu.com/wsl) for your own computer. This was an easy task for me since I had just done the same thing when I started at my new project at work.

The course material provided introduction on the commands used for listing the contents of your current directory, changing your current directory, downloading content from the internet, displaying a text file using less, creating and removing files and directories,
copying, renaming and moving files, as well as opening and editing a file in text editor called emacs. Most of these commands, as well as different commands for quitting applications were familiar to me due to my previous studies in Computer Science, and I use them daily at my work.

However, I had not previously used the command for downloading content, even though it is a very simple command. Thus, I learned how to fetch books from [gutenberg.org](https://www.gutenberg.org/) using wget. For example, the following command fetches book "Don Quijote" in plain text format:

```
wget https://www.gutenberg.org/files/2000/2000-0.txt
```

## Week 2

The second week deepened understanding about the UNIX system as well as on working on a remote server using the programs ssh and scp. Again I was familiar with most of the commands used in UNIX for copying, moving and deleting files and folders, or how to visit the root of the system, or change the read and write premissions of a file. However, this week I learned how to compress a my_folder directory into compressed.tgz package using tar:

```
tar -czvf compressed.tgz my_folder
```

I also learned how to find the PID of a process and how to kill it, as well as how to run commands in the background.

```
ps aux               // list all processes
kill -9 process_id   // kill a certain process by giving the id
```

In addition, I learned how to form a remote connection to Puhti server and how to copy files to and from a server using scp.

```
from local to remote home dir:
scp  my_folder/life_of_bee.txt puhti:~

bring a copy from remote to local:
scp puhti:~/life_of_bee.txt .
```

## Week 3

## Week 4

## Week 5

## Week 6

## Final project

By doing the final project I learned how to
- set up a Ruby installation environment, solve problems during installation process and install Jekyll using it
- fork a public repository in GitHub
- write documents using markdown
- assess what I had learned during the course
- merge a development branch which master branch
- build and display my webpage using command
```
bundle exec jekyll serve
```

## In Conclusion

This course was one of the best and useful courses I have taken during the past ten years! I learned so much on this course. Even though I already knew how to use the basic command-line tools such as Windows PowerShell, Command Prompt or Git Bash, I also got to practise the skills acquired previously. Moreover, I learned the basic use of WSL (Ubuntu).

I also learned to form regular expressions at a basic level and how to use them to process text corpora with command-line tools. I learned how to run and install simple programs from the WSL, and I learned to write simple scripts. Finally, I learned to work on the server.

I can warmly recommend Command-line Tools for Linguists web course to anyone interested in processing language files with simple command-line tools. The course format was fantastic regarding students working full time. The course material was super good and the videos were really great and easy to follow.

# List of interesting links

- [Command-line for beginners](https://ubuntu.com/tutorials/command-line-for-beginners#1-overview)
- [Unix tutorial](https://people.ischool.berkeley.edu/~kevin/unix-tutorial/toc.html)
- [Project Gutenberg](https://www.gutenberg.org)
- [Tips for ssh and scp commands](https://acloudguru.com/blog/engineering/ssh-and-scp-howto-tips-tricks)
- [chmod command](https://www.tutorialspoint.com/unix_commands/chmod.htm)
- [Unix/Linux process management](https://www.tutorialspoint.com/unix/unix-processes.htm)
. [Compressing directories and files in Unix](https://help.dreamhost.com/hc/en-us/articles/360002747432-UNIX-commands-Compressing-directories-and-files)
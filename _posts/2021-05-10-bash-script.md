---
title: Linux Bash Intro
layout: post
date: '2021-05-10 22:53:47'
description: Cheat Sheet

tags:
- linux
---
![linxu_bash](/assets/img/bash_script.png)

The first step is often the hardest, but don’t let that stop you. If you’ve ever wanted to learn how to write a shell script but didn’t know where to start, this is your lucky day.

If this is your first time writing a script, don’t worry — shell scripting is not that complicated. That is, you can do some complicated things with shell scripts, but you can get there over time. If you know how to run commands at the command line, you can learn to write simple scripts in just 10 minutes. All you need is a text editor and an idea of what you want to do. Start small and use scripts to automate small tasks. Over time you can build on what you know and wind up doing more and more with scripts.

Top Bash Commands
Quick note: Anything encased in [ ] means that it’s optional. Some commands can be used without options or specifying files.
ls — List directory contents
ls is probably the most common command. A lot of times, you’ll be working in a directory and you’ll need to know what files are located there. The ls command allows you to quickly view all files within the specified directory.
Syntax: ls [option(s)] [file(s)]
Common options: -a, -l

echo — Prints text to the terminal window
echo prints text to the terminal window and is typically used in shell scripts and batch files to output status text to the screen or a computer file. Echo is also particularly useful for showing the values of environmental variables, which tell the shell how to behave as a user works at the command line or in scripts.
Syntax: echo [option(s)] [string(s)]
Common options: -e, -n

touch — Creates a file
touch is going to be the easiest way to create new files, but it can also be used to change timestamps on files and/or directories. You can create as many files as you want in a single command without worrying about overwriting files with the same name.
Syntax: touch [option(s)] file_name(s)
Common options: -a, -m, -r, -d

grep — Search
grep is used to search text for patterns specified by the user. It is one of the most useful and powerful commands. There are often scenarios where you’ll be tasked to find a particular string or pattern within a file, but you don’t know where to start looking — that’s where grep is extremely useful.
Syntax: grep [option(s)] pattern [file(s)]
Common options: -i, -c, -n
man — Print manual or get help for a command
The man command is your manual and is very useful when you need to figure out what a command does. For example, if you didn’t know what the command rmdir does, you could use the man command to find that out.
Syntax: man [option(s)] keyword(s)
Common options: -w, -f, -b
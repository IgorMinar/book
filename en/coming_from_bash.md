---
layout: content
title: Coming from Bash
prev: Plugins
next: END
link_prev: /en/plugins.html
link_next: /
---

| Bash        | Nu           | Task  |
| ------------- | ------------- | ----- |
| `ls`     | `ls` | Lists the files in the current directory |
| `ls <dir>`    | `ls <dir>`| Lists the files in the given directory |
| `ls pattern*` | `ls pattern*` | Lists files that match a given pattern |
| `ls -la` | `ls -f` | List files with all available information |
| `ls -d */` | `ls` | where type == Dir` | List directories |
| `cd <directory>` | `cd <directory>` | Change to the given directory |
| `cd` | `cd` | Change to the home directory |
| `mkdir <path>` | `mkdir <path>` | Creates the given path |
| `mkdir -p <path>` | `mkdir <path>` | Creates the given path, creating parents as necessary |
| `touch` | | Create a file |
| | `| save <filename.ext>` | Save structured data as a filetype (implied by extension) |
| | `| save --raw <path>` | Save string into a file |
| `cat <path>` | `open --raw <path>` | Display the contents of the given file |
| | `open <path>` | Read a file as structured data |
| `mv <source> <dest>` | `mv <source> <dest>` | Move file to new location |
| `cp <source> <dest>` | `cp <source> <dest>` | Copy file to new location |
| `cp -r <source> <dest>` | `cp -r <source> <dest>` | Copy directory to a new location, recursively |
| `rm <path>` | `rm <path>` | Remove the given file |
| | `rm -t <path>` | Move the given file to the system trash |
| `rm -rf <path>` | `rm -r <path>` | Recursively removes the given path |
| `chmod` | | Changes the file attributes |
| `man <command>` | `help <command>` | Get the help for a given command |
|  | `help commands` | List all available commands |
| `echo $PATH` | `echo $nu.path` | See the current path |
| `<update ~/.bashrc>` | `config --set [path [<dir1> <dir2> ...]]` | Update PATH permanently |
| `export PATH = $PATH:/usr/other/bin` | | Update PATH temporarily |
| `export` | `echo $nu.env` | List the current environment variables |
| `<update ~/.bashrc>` | `echo $nu.env | insert var value | config --set_into env` | Update environment variables permanently |
| `FOO=BAR ./bin` | | Update environment temporarily |
| `bash -c <commands>` | `nu -c <commands>` | Run a pipeline of commands (requires 0.9.1 or later) |
| `bash <script file>` | `nu <script file>` | Run a script file (requires 0.9.1 or later) |

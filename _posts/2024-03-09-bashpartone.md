---
title: "The Journey: Bash Shell Basics and Examples"
date: 2024-05-18
categories: [Programming, Bash]
tags: [Bash, Shell, Linux, Tutorial]
---

## What a Bash Shell 

Bash (Bourne Again SHell) is one of the most popular and widely used Unix shells on Linux operating systems. This shell provides a command-line interface that allows users to execute commands, scripts, and programs efficiently.

## Installing Bash

On most Linux distributions, Bash is installed by default. To check if Bash is installed, you can run the following command:

```bash
bash --version
```

If Bash is installed, you will see the output of the Bash version installed on your system.

## Running Basic Commands

Here are some basic commands that are commonly used in Bash:

### 1. `ls` - List Files and Directories

The `ls` command is used to list files and directories within the current directory.

```bash
ls
```

### 2. `cd` - Change Directory

The `cd` command is used to change the current working directory.

```bash
cd /path/to/directory
```

### 3. `pwd` - Print Working Directory

The `pwd` (print working directory) command is used to display the current working directory.

```bash
pwd
```

### 4. `echo` - Display Message in Terminal

The `echo` command is used to display a message or variable in the terminal.

```bash
echo "Hello, World!"
```

### 5. `touch` - Create an Empty File

The `touch` command is used to create a new empty file or update the timestamp of an existing file.

```bash
touch newfile.txt
```

## Variables in Bash

Variables in Bash are used to store data that can be reused. To define a variable, simply use the `=` sign without spaces.

```bash
NAME="Bash"
echo "Welcome to $NAME shell"
```

## Writing and Running Bash Scripts

A Bash script is a text file containing Bash commands that can be executed. These scripts typically have a `.sh` extension.

### Simple Bash Script Example

Create a file named `hello.sh` and add the following lines:

```bash
#!/bin/bash
# Simple script to display a message

echo "Hello, World!"
```

To run this script, follow these steps:

1. Make the script executable using the `chmod` command:

    ```bash
    chmod +x hello.sh
    ```

2. Run the script:

    ```bash
    ./hello.sh
    ```

The output will be:

```bash
Hello, World!
```

## Control Flow in Bash

Bash supports various control flow structures like `if`, `for`, and `while`.

### `if` Statement Example

```bash
#!/bin/bash
# Example of an if statement

NUMBER=10

if [ $NUMBER -gt 5 ]; then
    echo "Number is greater than 5"
else
    echo "Number is not greater than 5"
fi
```

### `for` Loop Example

```bash
#!/bin/bash
# Example of a for loop

for i in 1 2 3 4 5; do
    echo "Number: $i"
done
```

### `while` Loop Example

```bash
#!/bin/bash
# Example of a while loop

COUNTER=0

while [ $COUNTER -lt 5 ]; do
    echo "Counter: $COUNTER"
    COUNTER=$((COUNTER + 1))
done
```


# Hello World - Shell/Bash

### This program is for Mac and Linux only!

## Overview

Here we go! Technically, not many people would call this a program. A `script` would be more accurate. What's the difference? It's a little muddy in this case, lots of programs that just do a simple instruction could be considered `scripting`, but the bigger difference is that the script you run in this solution is using the direct tools built into the terminal as opposed to a programming language. Technically, you can take each instruction within `hello_world.sh` and you can run them directly within your terminal, the script just wraps them up nicely for you. This is important because its your first instruction into what scripting is meant to do: automate tasks in a [nearly, mostly] perfectly repeatable and predictable way.

## What You'll Learn/Practice

- Navigating within your working directory
- Writing basic terminal syntax into a shell script
- Running your script
- Verifying program output in the terminal
- Troubleshooting basic errors

## Procedure

Navigate to your directory of Shell solutions for this problem.

```
cd ~/programming/hello-worlds-solutions/shell
```

Make a new directory labeled `hello-world`

```
mkdir hello-world
```

Navigate to within this directory

```
cd hello-world
```

Create a file to hold your solution

```
touch hello_world.sh
```

Next, open Sublime Text on your computer, navigate to the directory, and open the file you just created.

In another tab, open `~/programming/hello-worlds/HelloWorld/Shell/hello_world.sh`

Type out the file contents to your solution file, save, it and then run the command below to tell your computer that the script should have permissions to run as an executable.

```
chmod +x hello_world.sh
```

In the command below, `.` refers to the current directory, which your computer interprets as meaning it should run the script within this directory. That's a little confusing, but it's just convention and nothing that you need to worry about too deeply right now. Just know that when you run `./<script_name>` you are saying "run the script within this directory. If you wanted to run a script in a totally different directory, you can! Just run `./path/to/<script>`. But I digress:

```
./hello_world.sh
```

If everything worked correctly, you should see output like below!

```
~/Dropbox/Programming/hello-worlds/HelloWorld/Shell - ./hello_world.sh 
Hello, World!
```

If it doesn't work, take a close look at the error reporting. Shell scripting is extremely powerful, but it's also old and low level. That means the errors might be a little confusing. Nevertheless, try Googling anything that goes wrong and amending a fix on your own, and if all else fails, check the solutions below.

<details>

  <summary>Click here to expand</summary>
  
  - `./hello_world.sh: line 2: unexpected EOF while looking for matching "`: You are missing a double quot somewhere in your script.
  - `command not found`: You likely mistyped the `echo` command. Take a second look.

</details>

## What Did We Just Do?

We told the computer to run a script, `hello_world.sh`. It contains a single instruction, to `echo` (aka print to the console) a single piece of text. You could do the same thing by just typing `echo "Hello, World\!"` and pressing enter. So why wouldn't you do that every time? Well that's sort of the point of scripting: to not repeat yourself and to know what's going to happen every time you run a script. This will get more meaningful when we get into bigger and more complicated scripts.

But for now, congrats! You've written your first Shell script.
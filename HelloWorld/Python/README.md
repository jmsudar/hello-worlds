# Hello World - Python

## Overview

This is it! A Python Hello, World! application. In this app, you will write a single-line Python program that prints "Hello, World!" to the console. That sounds simple (and it is) but don't let that fool you: it is programming. It is giving an explicit instruction to the computer and executing that instruction. If you do this, you have officially programmed! This is an important first step and your official induction into being a programmer.

## What You'll Learn/Practice

- Navigating within your working directory
- Writing basic Python syntax in a `.py` file
- Compiling and running a Python program
- Verifying program output in the terminal
- Troubleshooting basic errors

## Procedure

Navigate to your directory of Python solutions for this problem.

```
cd ~/programming/hello-worlds-solutions/python
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
touch hello_world.py
```

Next, open Sublime Text on your computer, navigate to the directory, and open the file you just created.

In another tab, open `~/programming/hello-worlds/HelloWorld/Python/hello_world.py`

Type out the file contents to your solution file, save, it and then compile and run the program.

In the command below, `python` is the instruction that tells your computer what to do (run Python) and `hello_world.py` is the argument you are passing in, literally telling the computer what to run with Python.

```
python hello_world.py
```

If everything worked correctly, you should see output like below!

```
~/Dropbox/Programming/hello-worlds/HelloWorld/Python - python hello_world.py 
Hello, World!
```

If it doesn't work, take a close look at the error reporting. Python is pretty friendly and it should give you pretty complete language for finding the solution. Start by trying the fix on your own:
- Look at what the output says and make your best attempt to fix it.
- Compare the content of you solution file with the content of the example in the cloned repo.
- Google the error message and see if someone else has solved it already.
- If all else fails, there are quite a few potential error solutions below. Expand the section and see if any cases match what you're seeing.

<details>

  <summary>Click here to expand</summary>
  
  - `SyntaxError: '(' was never closed`: You have an open parenthesis in your code file.
  - `SyntaxError: unterminated string literal (detected at line 2)`: You have an odd number of `"` characters in your code.
  - `IndentationError: unexpected indent`: One of the only gotchas, syntax-wise when it comes to Python is that it cares about spacing. It gets away without using things like curly brace characters the way Java does by using four spaces, literally four presses of the space bar, to determine the depth of blocks. This error means you have some spacing off. In the case of this example, you shouldn't really have any spaces since the instructions are only a single line. The other thing this could mean is you may have a tab character instead of four spaces. Yes, this actually matters, because the characters are different! To fix this and still be able to use the tab key instead of pressing space four times each time, here are some instructions within [Visual Studio Code](https://uchicago-cs.github.io/student-resource-guide/vscode/config.html#space-indentation) and [Sublime Text](https://www.sublimetext.com/docs/indentation.html).
  - `NameError: name 'prit' is not defined. Did you mean: 'print'?`: You misspelled the word `print`. Fix it and everything should work fine.

</details>

## What Did We Just Do?

We told the computer, using the cli, that we want it to run the `python` interpreter. The Python interpreter can actually run by itself, first off. If you type `python` and nothing else and press enter, the interpreter will open like below:

```
~/Dropbox/Programming/hello-worlds/HelloWorld/Python - python
Python 3.11.5 (main, Sep  9 2023, 13:35:08) [Clang 13.0.0 (clang-1300.0.29.30)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> 
```

At this line, I could actually run the exact same line as is in the `hello_world.py` file and it will run:

```
>>> print("Hello, World!")
Hello, World!
```

(as a quick aside, type `exit()` and press enter to close the interpreter.)

```
>>> exit()
~/Dropbox/Programming/hello-worlds/HelloWorld/Python -
```

So what does that mean with regards to the command we just ran? It means that when we type `python hello_world.py` and press enter, we tell the computer, "use the Python interpreter with a single argument, `hello_world.py`, which corresponds to a file with Python instructions in side of it. Python opens the file, reads the instruction, and writes "Hello, World!" to the console.

Congratulations, you have run your very first Python program!
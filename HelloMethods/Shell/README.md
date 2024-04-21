# Hello Methods - Shell

## Overview

Shell modularity time!

## What You'll Learn/Practice

- Writing your second Shell script, shoring up those lessons
- Writing a distinct method and calling it

## Procedure

Navigate to your Shell solutions directory, create a subdirectory for this lesson, then navigate inside that directory.

```
cd ~/programming/hello-worlds-solutions/shell
mkdir hello-methods
cd hello-methods
```

Create a file to hold your solution

```
touch hello_methods.sh
```

Next, open Sublime Text on your computer, navigate to the directory, and open the file you just created.

In another tab, open `~/programming/hello-worlds/HelloMethods/Shell/hello_methods.sh`

Type out the file contents to your solution file, save, it and then make it executable

```
chmod +x hello_methods/sh
```

Run your script

```
./hello_methods.sh
```

If everything worked correctly, you should see output like below!

```
~/Dropbox/Programming/hello-worlds/HelloMethods/Shell - ./hello_methods.sh       
Hello, World!
```

If something goes wrong, go through the same troubleshooting steps you tried last time. We really didn't change that much, so I'm not going to write out the troubleshooting tips again. If you're stuck, go back to the [README](/HelloWorld/Shell/README.md) troubleshooting section and work through things.

## What Did We Just Do?

We just created a method! Here's why that's important: we can call it many times. As many times as you need to. It will run every time it's called. Let's try an exercise related to that. Go back to your `hello_methods.sh` file and change the block to look like the below:

```
# Call the function
hello_world
hello_world
hello_world          
```

Now, compile and run it again. You should see output like the below:

```
~/Dropbox/Programming/hello-worlds/HelloMethods/Shell - ./hello_methods.sh       
Hello, World!
Hello, World!
Hello, World!
```

Do you see now? Writing a method lets us make _reusable_ behavior, and that is very important for writing and maintaining software. We will expand on this more over the next two lessons.
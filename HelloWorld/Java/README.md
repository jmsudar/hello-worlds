# Hello World - Java

## Overview

Alright, time for the big kids. Java is less friendly than Python, in that it requires closer attention be paid to syntax, and you might not get as well-formatted errors as you'd like, but this also has benefits: it's a little lower level which means things are more predictable, and its "write once run anywhere" philosophy, along with its price tag (free) helped Java become the defacto language for... pretty much everything in terms of web servers and the internet in general. All that being said, what matters is it's worth learning!

## What You'll Learn/Practice

- Navigating within your working directory
- Writing basic Java syntax in a `.java` file
- Compiling and running a Java program
- Verifying program output in the terminal
- Troubleshooting basic errors

## Procedure

Navigate to your directory of Java solutions for this problem.

```
cd ~/programming/hello-worlds-solutions/java
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
touch HelloWorld.java
```

Next, open Sublime Text on your computer, navigate to the directory, and open the file you just created.

In another tab, open `~/programming/hello-worlds/HelloWorld/Java/HelloWorld.java`

Type out the file contents to your solution file, save, it and then compile and run the program.

In the command below, `javac` is the instruction that tells your computer to use the Java compiler to... well, compile, the code file `HelloWorld.java`. The `;` character then signifies there's an additional command, in this case using `java` to run the compiled class that you produced: `HelloWorld`.

```
javac HelloWorld.java; java HelloWorld
```

If everything worked correctly, you should see output like below!

```
~/Dropbox/Programming/hello-worlds/HelloWorld/Java - javac HelloWorld.java; java HelloWorld
Hello, World!
```

If it doesn't work, take a close look at the error reporting. Java is matter of fact, but it's pretty complete as well. You should see the error descriptor for simple issues in your console output. Start by trying the fix on your own:
- Look at what the output says and make your best attempt to fix it.
- Compare the content of you solution file with the content of the example in the cloned repo.
- Google the error message and see if someone else has solved it already.
- If all else fails, there are quite a few potential error solutions below. Expand the section and see if any cases match what you're seeing.

<details>

  <summary>Click here to expand</summary>
  
  - `HelloWorld.java:4: error: unclosed string literal`: You forgot the second quotation mark somewhere in the file.
  - `HelloWorld.java:4: error: ')' or ',' expected`: Sort of like the above: you're missing a parenthesis.
  - `HelloWorld.java:4: error: ';' expected`: You need a semi-colon at the end of the indicated line, in this case line `4`.
  - `HelloWorld.java:2: error: class HellWorld is public, should be declared in a file named HellWorld.java`: In this case it's a typo in my class name, where I misspelled `HelloWorld` as `HellWorld` (yikes).
  - `HelloWorld.java:2: error: class, interface, enum, or record expected`: You misspelled a reserved word. In this case I intentionally misspelled `public` in the code file.
  - `HelloWorld.java:3: error: <identifier> expected`: Here I misspelled `String[]` as `String]` in my `main` declaration.
  - `HelloWorld.java:6: error: reached end of file while parsing`: Very common syntax error here: I forgot one of my curly brace (`{}`) characters. These tell Java where statements begin and end so they are very important.

  As you can see, there are _many_ potential syntax errors with Java. Fortunately, when you graduate to using an IDE instead of a text editor, many of these will be caught for you before compile-time. For now though it's important to learn the syntax and struggle through those errors.

</details>

## What Did We Just Do?

PHEW. A lot, relative to the other languages so far. We declared a Java class

```
public class HelloWorld {
```

We set its entry point as `main`, which is a very standard convention for Java. Basically it tells Java "everything that's within this block, do, in order" (remember that programming is simply giving specific instructions).

```
public static void main(String[] args) {
```

(Wait a second what's that `String[] args` mean!? Well that's going to be the focus of a later lesson, so don't worry about it yet).

Finally, we declared what we want to happen in `main`: we want to run our print command.

```
System.out.println("Hello, World!");
```

This command is saying take `System`, a Java library, and using its tool called `out`, which is for making output. Then, we use the command `println` which is short for "print line," and tell it what to print: `"Hello, World!"`.

After that, we ran the Java compiler with the command `javac`. If you look before and after running this command, you will see that there's a new file in our directory:

```
~/Dropbox/Programming/hello-worlds/HelloWorld/Java - ls                                    
HelloWorld.java	README.md
~/Dropbox/Programming/hello-worlds/HelloWorld/Java - javac HelloWorld.java 
~/Dropbox/Programming/hello-worlds/HelloWorld/Java - ls
HelloWorld.class	HelloWorld.java		README.md
```

`HelloWorld.class` appeared! This is our compiled code, which java can actually use to do a thing. So we then instructed Java to do the thing:

```
~/Dropbox/Programming/hello-worlds/HelloWorld/Java - java HelloWorld 
Hello, World!
```

And voila, the program is run! The only difference is that in the instructions above, you ran both `javac` and `java` on the same line. You don't have to do it that way, I just wanted to show it as another option to be aware of.

And congragts! You've Java'd!
# Hello, Worlds!

Welcome! This repository serves as a playground for anyone with an interest in software development with minimal background in the field. The name, `Hello, Worlds!` is a play on the classic [Hello, World!](https://en.wikipedia.org/wiki/%22Hello,_World!%22_program) outlined in _The C Programming Language_. For most programmers, myself included, printing "Hello, World!" to the terminal was the first programming achievement in the foothills of a software development mountain. It can be difficult, if you're just starting out and don't understand what's going on inside your phone, behind your favorite video game, or how Netflix/Facebook/Redfin/etc. serve an endless stream of content, to imagine how you go from "Hello, World!" to the top of the mountain. In reality, running a `Hello, World!` program accomplishes a couple important steps:

- It requires you to have a programming language and compiler installed
- It introduces you to programming syntax
- It forces you to compile and run custom software that _you_ made

The reason this repo is called `Hello, Worlds!` is because I intend to cover multiple programming languages. If the scope expands beyond just a `Hello, World!` program to solve other problems, they will either be solved across each language, or an explanation will be given for why it could not be solved in that language. The lesson here is that there are multiple ways to solve problems with programming. There is no right or wrong way, there are just solutions that fit the needs of your problem (or don't).

## Who is This For?

If you already have a background or experience in software development you will find the early problems here extremely basic. The goal here is to go from zero to sixty, and zero includes setting up a basic programming environment for the first time, which is not something most existing developers need to worry about.

If instead you want to learn programming, whether for curiosity or for career opportunities, this is meant to help you get started down the road.

An important note: the layout of this repo does not necessarily correspond to the layout of a production application repo. The intention here is to isolate each solved problem such that you can navigate to a subdirectory and compile/run a program on its own. In reality, with more complex software, you will find much larger repos, often packed full of dependencies, and with less detailed instructions than this on how to get started. That is not meant to intimidate nor to confuse, it's just something to be aware of as you move beyond this repo and into the broader software ecosystem.

## What is Programming?

You probably know some answer to this question already, but I'm calling it out here because there is one very important definition of programming that relates to the work done in this repo: computers are simply tools that follow very specific instructions, and programming is simply the act of setting those instructions. That's really it. There's plenty of science in the field that feels like magic because the achievements are so impactful, but really there's no magic at work here. The computer will follow its instructions exactly, because that is what computers do.

I'll say it again because it's so important to understanding what this repo is and does: _if you are programming a computer, you are giving it instructions to follow, and it will follow exactly the instructions you give it_, that is all.

## Glossary

To begin with, here are some key terms you may have heard but don't know your way around yet.

- `repository/repo`: This is a repository/repo. It's just a collection of code, or really just of information, meant to serve a purpose. That might be source code for a tool, a programming language, or an app. Either way, it's just a distinct collection of source code, stored in a source code manager.
- `directory`: This is the technical name for a file folder on a computer. Everything you do in this repo will involve navigating between file directories.
- `file extension`: File extensions tell a computer what type file something is, and through that how the computer should treat a file. The file extension `.py` for example tells the computer that `filename.py` is a Python file and that it should open it with the Python interpreter.
- `terminal/console/commamd-line interface/cli`: Both the terminal and console are referred to heavily throughout this repo. `Console` is a pretty general term, referring to how you interact with a computer via text instructions. When I say something will `print to the console` what I mean is the text will be written to the text interface you are using. The `terminal` is short for `terminal emulator`, and is the Linux and Mac tool for emulating a shell.
- `shell`: The Shell refers to the program that interprets bash scripting. Bash is simply the language used to write programs for the command line. So that means that if we are writing programs directly in the cli without using a language like Python or Java to write them, we are writing them in Bash and the shell is interpreting them.
- `graphical interface/graphical user interface/gui`: A GUI is just a graphical way to interact with a computer, and is the method of interaction you are probably most familiar with. It stands in direct contrast with the terminal/console. When you click through a file folder and double click on a file to use the program you want, you are using the GUI. The instructions within this repo are more console-based than GUI-based, but both are used.
- `source code`: Source code is the code that, when compiled, becomes an app or tool. Something we will hammer on throughout this project is: code is just instructions, that's all. You give your computer instructions to follow to solve a task. It really is that simple, and while complexity does appear as things get bigger and more collaborative, it's still just instructions and a machine at the end of the day.
- `source code manager/scm`: GitHub is a source code manager/SCM. Bitbucket is another one you may have heard of. Regardless, it's a place to store repos, and its purpose is to facilitate collaboration, eg. I am checking this code into GitHub as my SCM so that I can share it with you!
- `version control`: Version Control is the act is checking in changes to improve software in a way that can be rolled back if your changes accidentally make the software worse. Git is by far the industry standard, so all examples in this repo will use Git.
- `compile/compiled/compiler`: Whether you run a Hello, World! example in Python, Shell, or Java, the end result is the same: printing "Hello, World!" to your console. How!? Because what your computer actually uses isn't Python, Shell, or Java, it's machine-code. A compiler is what takes a higher level language and translates it into this machine code. You don't need to worry too much about that right now, just accept that that is what happens and what turns your nice, high-level code into gnarly, difficult to read machine code.
- `library`: A library is a collection of code that you can use to do things. A common refrain in programming is "don't repeat yourself," so when developers do something and decided they want to not have to create the stuff to do it again, they will make a library. This library is then usable within that language by anyone to whom they give access.
- `interpreter`: An interpreter turns code line by line into machine code. The line by line nature and difference vs. a compiler gives you detailed error reporting that can help you figure out what's going wrong with your code.
- `high-level language`: Generally speaking, the higher level a language is, the more forgiving the syntax and conventions are. Python, where you don't have to worry about special characters and curly braces, is higher level than Java. But Java, where you don't have to worrk about manually allocating and releasing memory space, is higher level than C++. C++, which already has object and class definitions, is higher level than C. And C is higher level than writing in direct machine language. No one writes in binary, btw.
- `text-editor`: It edits text. That's it. A text-editor is a simple program that allows you to manipulate the text in files and save your changes. That's all programming is at a mechanical level, because again, it's just giving instructions to a machine, so with your text-editor you are writing those instructions down.
- `integrated development environment/ide`: An IDE is a glorified text-editor with a ton of included tools. Visual Studio is an IDE. It differs from a text-editor in its feature richness. It will give you autocomplete, syntax highlighted, manage depdendencies, and even let you run and debug your program. This repo is meant to be used with a text-editor because it's meant to teach you the basics of syntax, but when you graduate to writing your own software you should start using an IDE from the get go.
- `reserved character`: A reserved character is a keyboard character that is used to denote something specific within a language, which means that it must be handled in a specific way. For example, in the terminal, `!` is a reserved character. That means that if we want to print "Hello, World!" in directly, we have to `escape` the `!` character, otherwise the computer will assess it to mean something specific and the program will not run correctly. To fix this, we escape it with the `\` character, and `!` becomes `\!`. You can try this yourself right now: open your terminal and run `echo "Hello, World\!"`. Now try it with `!` instead of `\!`. It gets weird, right? Don't worry, to get out of that prompt just hit `ctrl + c`.
- `executable`: This means a program or script that can be executed. This matters most in the content of Shell programming.
- `class`: Defining a class is complicated, because it also involves defining an object, and understanding objects is one of those things that comes in time. For now please just know that classes are compiled code that Java uses to perform tasks. When you compile your Java files, they are turned into classes.
- `argument`: An argument is just something additional that you pass to a program to change how it will run. If a program can "accept multiple arguments," it means that what will happen when it runs can be different or happen in multiple ways. This will be expanded on specifically in one of the later exercises.
- `collection`: A collection is just a group of things. There are many collections within programming like arrays, lists, sets, and so on, but the important part is that when you see a collection referenced later, it's just a group of things. If I were playing marbles, my bag of marbles, in the context of programming, would be my `collection`.
- `element`: An element is just one thing inside of a collection. If my collection were a bag of marbles, one individual marble would be an element.

## How Do I Use This Repo?

- 1. Read this whole file. It outlines conventions, makes sure you have the right things installed, then sets you loose on the problems.
- 2. Go through each problem in order, in each language. You may only want to learn one programming language, but the point of this is to hammer home that computers are just machines that take instruction, and to show you what's different with each type of instruction and why you would want one vs. another.
- 3. Use the terminal. It's intimidating but it is powerful. It is intensely powerful. Good lord you cannot imagine the power, just starting out as you are. The best professional developers use the terminal because once you get comfortable with it, it is easier, faster, and more accurate, and the difference between a junior and senior developer is almost always speed and accuracy.
- 4. Type each problem out for yourself in a simple text editor. Unless otherwise indicated, avoid using a rich IDE. You will probably make syntax mistakes, but that's okay, and it being okay is the point of all this. You are here to learn, and that includes learning how to diagnose and recover from mistakes. On top of that, having to handle the syntactic weirdness yourself will help to make it second nature, which will make you faster and more accurate in the long tun.
- 5. Run the included solution and your solution and compare. Each of the included examples will compile and run if you follow the instructions for setup and for completing the problem. After you've copied the solution and run your version, you should compare it to the included example to make sure you did the work correctly.
- 6. Use this as a jumping off point. This guides you up through multiple examples of how to do a thing. Once you've done the thing, you are officially qualified to do the thing again, differently. You should take this license and run with it, thinking of problems you would like to solve, trying them, and iterating on that to do more and more.

I hope that using this repo is a good experience and you leave it feeling a deeper understanding of how to be a software developer than when you started!

## Getting Started

### Setup

Let's go through the basic setup of a development environment on a Mac. The goal here is to make sure you have the basic tools necessary to go through the activities in this repo. The good news is that much of this stuff is already installed!

#### Homebrew

`Homebrew` or `brew` is a simple package manager for Mac computers. It automatically fetches programs and installs them for you. We're addressing it first because using brew will make everything else you have to do easier.

You can check if brew is installed with the command below. If it prints a version that means it's installed!
```
~/Dropbox/Programming/hello-worlds - brew --version
Homebrew 4.1.19
```

If brew isn't installed, follow the instructions on the [official homepage](https://docs.brew.sh/Installation), then verify your installation with `brew --version`.

#### Git

`Git` is version control software. You need it to clone this repo, and you will _definitely_ need it when you graduate to working on your own software.

Verify Git is installed by checking its version.
```
~/Dropbox/Programming/hello-worlds - git --version
git version 2.32.0 (Apple Git-132)
```

If it isn't installed, you can fix that with brew.
```
brew install git
```

#### Python3

First off: Python is a programming language and a runtime environment. The steps I am outlining here are to verify you have Python installed so that you can run Python programs.

Without getting two into the weeds, there are some major differences between Python version 2 and Python version 3. Python3 is gradually becoming the industry standard, so everything in these examples will be with Python3.

When you run `python --version` you want to see a version in the format `3.x.y`.
```
~/Dropbox/Programming/hello-worlds - python --version
Python 3.11.5
```

If you don't see that, run another brew command.
```
brew install python
```

#### Java

Java is also a programming language and runtime environment. It also comes pre-installed on most Mac machines. To begin with, type

```
java --version
```

If you see output similar to the below, you're golden.

```
~/Dropbox/Programming/hello-worlds - java --version
openjdk 21 2023-09-19
OpenJDK Runtime Environment Homebrew (build 21)
OpenJDK 64-Bit Server VM Homebrew (build 21, mixed mode, sharing)
```

Really the only thing to be concerned with is if your computer says Java is not a recognized command. There are many different versions of Java, but managing them gets messy so we are going to hold off on worrying about that until we need to. For now, just have _a_ version of Java, and if you don't see one, run

```
brew install java
```

#### Sublime Text

If you'd rather use a different text editor, go for it! Otherwise, use this command to install Sublime Text. You will use this got writing/copying your versions of the solutions.
```
brew install --cask sublime-text
```

#### Visual Studio Code

Visual Studio is a great IDE that will help you to work more effectively when you are working on more complex software. Bonus points you can install it with brew as well.
```
brew install --cask visual-studio-code
```

### How to Use The Terminal

Entire books exist on how to improve your [Kung Fu](https://youtu.be/NOb7JXV1T1Q?si=8v8UXcE9abhMiXE0&t=31) in the terminal. All the same, it's important for you to understand how to use the terminal if you want to seriously learn software development. With that in mind, let's go over the very basics.

To begin with: there are a lot of copy-pasted examples in here. That's important because I'm showing you exactly what appears in my terminal when I run these commands. Your output will be different but at least a little similar. That doesn't mean anything is wrong, just something to expect.

The terminal, first of all, is just another way to interface with your computer. What happens and what you do in the terminal is exactly the same as what happens and what you do when using the graphical interface, it's just presented differently and happens a little more directly. This means it _is_ possible to do something scary like accidentally deleting a file, but following the instructions here is perfectly safe.

To open your terminal on a Mac, you can either open your `Applications/Utilities` folder and open the `Terminal` application, or you can press `Command + Space Bar` and start typing Terminal.

Bonus points: `Command + Tab` will quickly flip between open apps on your computer. This will be helpful as you work through the basic terminal commands as you can easily tab to and from your web browser and the terminal.

Some basic commands:
- `pwd`: print working directory. This will print out to the terminal the path of the directory you are currently in. You can think of that as which file folder you currently have open. This is the beginning of how you interact with a console vs. the GUI. When you want to navigate to something on your desktop, you click on a folder, go into it, click into a subfolder, and so on. Those two terms, `folder` and `directory` are interchangeable here. When you `print working directory` you are simply printing to the console what subfolder you are in. 
```
~/Dropbox/Programming/hello-worlds - pwd
/Users/jmsudar/Dropbox/Programming/hello-worlds
```
- `ls`: list. This prints out the contents of your current directory. Think of it like having the file folder open in your file explorer and looking at the contents.
```
~/Dropbox/Programming/hello-worlds - ls
HelloWorld	LICENSE		README.md
```
- `cd`: change directory. This is how you navigate from directory to directory, like double clicking on a file folder in the graphical interface. `cd <directory name>` will change your working directory to `<directory name>`. `cd <directory name>/<subdirectory name>` will leapfrog you straight into `<subdirectory name>`. `cd ..` will move you up one directory, while `cd ../..` which move you up two directories.
```
~/Dropbox/Programming/hello-worlds - pwd
/Users/jmsudar/Dropbox/Programming/hello-worlds
~/Dropbox/Programming/hello-worlds - cd ../..
~/Dropbox - pwd
/Users/jmsudar/Dropbox
~/Dropbox - cd Programming/hello-worlds 
~/Dropbox/Programming/hello-worlds - pwd
/Users/jmsudar/Dropbox/Programming/hello-worlds
```
- `touch`: creates a new file. `touch <filename>` will create a new, empty file of name `<filename>`.
```
~/Dropbox/Programming/hello-worlds - ls
HelloWorld	LICENSE		README.md
~/Dropbox/Programming/hello-worlds - touch example.txt
~/Dropbox/Programming/hello-worlds - ls
HelloWorld	LICENSE		README.md	example.txt
```
- `mkdir`: make directory. This is how you create a new file folder within your working directory.
```
~/Dropbox/Programming/hello-worlds - ls    
HelloWorld	LICENSE		README.md
~/Dropbox/Programming/hello-worlds - mkdir example
~/Dropbox/Programming/hello-worlds - ls
HelloWorld	LICENSE		README.md	example
```
- `rm`: remove, aka delete. `rm <file name>` will delete a `<file name>` _permanently_. It won't go into your Trash or Recycle Bin, it'll just poof, be gone. This means you have to be a little careful with this because if you delete the wrong file you will lose it. That's just something you will have to get used to though; being a professional software developer means understanding implications and constraints like this and working within them. If you want to delete a directory instead of a file, you need to use `rm -r <directory name>`.
```
~/Dropbox/Programming/hello-worlds - ls
HelloWorld	LICENSE		README.md	example.txt
~/Dropbox/Programming/hello-worlds - rm example.txt 
~/Dropbox/Programming/hello-worlds - ls
HelloWorld	LICENSE		README.md
```
- `[tab]`: I'm referring here to the tab key on your computer. Hitting it will make your computer try to autocomplete what you've typed. This is useful both if you don't want to type a really long filename, and because letting the computer complete a filename for you makes it less like you do something wrong due to a typo.
- `~`: The tilde character means your home directory. On a Mac, that means `cd ~/example` will navigate you to `/Users/your-name/example`.

### Put It All Together

You've installed all your dependencies, so let's do the pre-reqs to get things working:
- 1. Navigate to your home directory
- 2. Create a directory to hold your work
- 3. Create a directory to hold your solutions to the problems for each language
- 4. Clone this git repository

type out and run each of the commands below in the terminal

```
cd ~
```

```
mkdir programming
```

```
mkdir hello-worlds-solutions
```

```
mkdir hello-worlds-solutions/python
```

```
mkdir hello-worlds-solutions/shell
```

```
mkdir hello-worlds-solutions/java
```

```
git clone git@github.com:jmsudar/hello-worlds.git
```

### Conventions and Other Considerations

There are just a couple other things to think about before you start the problems.

Given that software development is collaborative by nature, there are conventions to follow that make the work more predictable and easier to follow from person to person. I'll enumerate on some of them here.

#### Naming

```
There are only two hard things in Computer Science: cache invalidation and naming things.

-- Phil Karlton
```

There are lots of really weird names for things in software, but there's also 50+ years of history and convention around this naming, so you should expect to learn some of it as you dig more into software, weirdness and all. The naming is also there for a reason a lot of the time. I used the word `enumerate` up above, and you will likely see that word at some point in your software journey. It refers to a very specific thing: establishing the number and order of a collection. Given that the [nature of programming](#what-is-programming) is to follow instructions exactly, if you are doing a task that requires you to establish the number and order of a collection to do a thing, `enumeration` could be an important concept to know. Being a professional software developer never means you know exactly what will happen in every case, more than you know the patterns, the tools, and the general expectations of how a program, yours or someone else's, will work, because you are trying to solve a specific problem.

#### Capitalization

Casing (uppercase and lowercase letters), hyphen and underscore placement, and file extensions are all also important things to know, and the examples here follow the conventions established for each language. For example, Python programs are in `snake_case`, meaning there is an underscore between words, and additionally each filename is all in lowercase.

#### Commenting

Comments are lines of code that will not be actioned by the compiler. This means that you can use comments to leave plain language instruction in your code. This is critically important: it helps other people understand what you're trying to do, but also it helps future-you understand what you were trying to do. You would be shocked how quickly you can forget what your work does and why after you stop staring at it for even a couple days.

Comments can also be used to call out tricky or gotcha sections of code that might not be immediately apparent to someone.

Commented lines are denoted by the use of a special character. In Python, commenting a single line begins with a `#` character, so `# This is a comment and would be ignored by the Python compiler`. Multi-line comments in Python can be wrapped in triple quotations `'''like this '''`.

#### Other Files In This Repo.

There are some other files in this repo that don't correspond to the problems you are working on, but they're plenty important all the same.

- `LICENSE`: All software is licensed for use in some way or another. With something prorietary like Microsoft Office, you are typically licensed to use it as an individual or group and are required to follow the rules Microsoft outlines for how you can use it. This is how companies protect themselves from piracy and from being liable if their tool is used for something criminal. Open-source developers also need licenses, primarily for that liability issue. It would chill the collaborative nature of software development if you could wind up in court over someone else abusing your use case and committing a crime. This repo uses the `Gnu Public License 3.0`, which opens it for use to anyone for non-commercial applications and protects me from someone using my good work here for evil.
- `README.md`: You're reading it right now! A README is where, by convention, you put the documentation necessary to understand how to use a repo. Another common README file you will see a lot is `CONTRIBUTING.md`, which outlines how other people can contribute to your work, what are conventions, et cetera. The `.md` is a file extension which indicates the file is written in `markdown`. Markdown is ironically a markup language. It doesn't give instructions to a computer like a program file does, but it does tell other programs like Visual Studio Code, your web browser, or a text editor like Sublime Text how to present the information in the file. Just as an aside: the conventional name, `README`, is a throwback to before people had GUIs to navigate files and directories. Back then you would print `ls`, see a bunch of filenames that wouldn't make natural sense, so a big bold README in your console gave you a clear place to start. There are some things in programming that are weird because they're weird, but most conventions exist for a practical reason, and this is one of them.
- `.gitignore`: We are using Git for version control. A `.gitignore` file tells Git which files not to include when it is doing its job, versioning. This prevents little local files that the operating system uses for background tasks from being stored, but also keeps the repo clean, avoiding any clutter from files that are built as part of the compiling process.
- `.github/workflows/*`: I am using GitHub Actions to handle some of the chores that go into maintaining a repo, such as tagging versions, making a changelog, and creating a release. The files in this directory instruct the GitHub Actions platform on what to do to complete these chores. This is part of a larger process called Continuous Integration and Continuous Deployment, or CI/CD. CI/CD is a very important part of modern professional software development. Large companies could not function without it, or they could (and did for years) but it would be much harder and much more error prone. For now, simple know that CI/CD exists and you may need to use it some day.

## The Problems

These are the problems solved within this repo.

Open the solution in each language and follow the instructions in the README within each subdirectory to solve the problems.

#### Hello, World!

Let's dig into it. The classic Hello, World! problem is solved here in

- [Python](/HelloWorld/Python/)
- [Java](/HelloWorld/Java/)
- [Shell](/HelloWorld/Shell/)

#### Hello, Methods!

Reusability is programming gospel. This module introduces you to the very beginning of reusability by showing you how to break behavior out into distinct, reusable functions (also known as `methods`.)

- [Overview](/HelloMethods/)
- [Python](/HelloMethods/Python/)
- [Java](/HelloMethods/Java/)
- [Shell](/HelloMethods/Shell/)

## Additional Resources

One of the great things about software development and engineering, vs. other engineering disciplines, is that if you have a computer and an internet connection you have everything you need to get started. Compare that to electrical or mechanical engineering, where along with specialized equipment you need a certification, and the opportunities are self-evident.

Software development is inherently collaborative. As such, plenty of people other than me have made resources to help developers get started, learn, and solve problems. Here are some other resources you should consider to expand beyond what you find here.

#### The University of Washington

Critically important note: I am not a Husky, Go Cougs! That being said, the University of Washington posts some of  their introductory computer science course materials online. I used the posted materials for their CSE 142 class to learn the basics of Java and it looks like the homeworks at least are [still available](https://courses.cs.washington.edu/courses/cse142/22sp/homework.shtml).

#### Harvard

Harvard, AKA "a school in Boston," offers many of their courses for free. If you want a certificate of completion, you have to pay, but if you're just looking for practice, this [Introduction to Python Programming](https://cs50.harvard.edu/python/2022/) would be a great starting point! If you want to dig deeper than that, you can browse their [catalog of courses](https://pll.harvard.edu/catalog?topics%5B715%5D=715&max_price=&start_date=&keywords=).

#### Your Public Library

Many public libraries have resources for online learning, and this may include excellent resources like LinkedIn Learning. If you are in the Seattle area, for example, and you have your library card, check out their [online learning](https://www.spl.org/online-resources/online-learning) section.

#### DotNet Playbook

I'm calling [dotnetplaybook.com](https://dotnetplaybook.com/) out specifically because I find his solutions and explanations to be clear, easy to follow, and unafraid of asking questions like "Which is better, WebSockets or SignalR?" That may sound like nonsense right now, but it's a good resource for later in your journey to become a developer.

#### Vim Adventures

If you really want to up your Fu, Vim is a powerful but intimidating text editor. The best method I've found for learning Vim is the [Vim Adventures](https://vim-adventures.com/) online video game. Early on, learning Vim can be frustrating, so you should minimize exposure to it until you're more comfortable with the fundamentals, but later on if you find yourself in an operations tangential role, it is invaluable.

### Who am I?

I am a self-taught developer who benefitted from several generous mentors and endless online resources as I worked to transition to a career in technology. I hope to contribute to that knowledge base and pay forward the generosity I received.
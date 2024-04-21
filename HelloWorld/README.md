# Hello, World!

Here we go! In this lesson you are writing a Hello World application in multiple languages. This application will perform a single task executing an instruction in its `main` block.

First, let's go over what that means, then let's go over the similarities and differences in how this will run across the languages. We will do this with every lesson in this repo.

### What's main?

When you run an application, it has to know _something_ in terms of how to set itself up and how to run. You are giving instructions to the computer, but you're not telling the computer how to run a Java, Python, or any other program; the computer already knows how to do that by using the runtime environment for each of those languages. How though? Primarily through convention: the designers of the programming language determined that a common place to start was required, and it just so happens that a `main` block became a convention in many cases. Whatever you put in `main` is what will run when your application starts up.

## What's the Same?

- In each application, a single line, "Hello, World!" will be written to the console
- Each application performs the step directly in the `main` processing block of the application

## What's Different?

- Each application will use different syntax. Pay close attention here: each syntax needs to be correct or your app won't compile
- The structure of each app will be different as each programming language has different conventions

## Glossary

- `main`: refers in this case to the entry point for the application. `main` is usually a block of code that the computer knows to run when an application is invoked.
- `entry point`: This is the technical term for the role of the `main` block. Technically, another block could be set to run by default instead of `main`, and then it would be the `entry point`. It really is exactly what it sounds like: an `entry point` is where the programming runtime will enter your app and begin processing instructions.
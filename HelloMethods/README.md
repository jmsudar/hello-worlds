# Hello, Methods!

So time for a small confession: when I said that programming is the act of giving explicit instructions to a computer, that was true, however, it also misses some of the art and finesses of programming. If I want to write a program that accomplishes thirty similar tasks, I could certainly write out all thirty tasks. In reality however, that wouldn't be very efficient, and it certainly wouldn't be fun. That E word though, efficiency, is important: the reason programming is a high-paid career is because programmers are able to leverage computing power to be, or to make things, efficient. If you create a program that takes as much time to write as it would doing all the tasks manually, you are not being very efficient. On top of that, if you write something that is so specific and brittle that you can't update it, you're not only being inefficient, you're probably at a point where you can't even work.

To get around this, programmers try to write their code generally, and most importantly, **in a way that can be reused**. In this problem, we are going to work on the foundations of reusable programming.

### Leveling Up the Instructions

The instructions for this set of apps are going to start getting a little more complicated! At this point you've practiced navigating around the terminal, so some instructions are now going to be multi-line instead of single-line. The reason for this is you now know enough about how to use the terminal to understand that you are doing each of these lines distinctly.

Congrats on your first programming level up!

### Methods, Functions, Units

All three of the terms above refer to the same thing: a distinct piece of code that can be `called ` by another piece of code. This is incredibly powerful: it means that you can define behavior for your program, and you can do that behavior as many times as you need to, whenever you need to. This is the very _essence_ of software development; it allows you to engineer complex flows that can be combined and leveraged and reused to accomplish complex things.

But at first this is going to seem pretty basic, so bear with me: all that's going to happen in this first exercise is you're going to take your behavior, the printing of "Hello, World!" to the console, and you're going to move it from the `main` functionality and into its own method. Then, you're going to call it from `main`.

### So what, what does that get us?

Well, you'll see! The short answer is: not much, yet. You'll see that this adds a little more extensibility to your program, but you won't really see the benefits of this change for a lesson or two. When you do though, I guarantee there will be a real _click_ moment.

## What's the Same?

- Each application will use a single method to define their behavior
- Each method that defines behavior will be called within `main`

## What's Different?

- Once again, syntax and convention differs in how to define a method
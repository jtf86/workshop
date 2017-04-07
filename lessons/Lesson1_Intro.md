## Hello World!

Welcome to the Intro to Programming Workshop at Epicodus. This workshop is designed to give you a chance to experience working with some of the basic tools used in everyday web development.

It doesn't matter if you've have some experience coding before, or if this is your first time sitting down to build a project. By completing this workshop you'll get a feel for what goes into building a basic website, and a bit of what attending Epicodus as a student is all about.

<hr>

## The workshop

We'll begin by building a simple HTML webpage. Once that's complete, we'll add some CSS styling.

Once our page is complete, we'll look to make it interactive by using a bit of JavaScript.

Finally, we'll learn how to use Git, a piece of industry standard version control software, to track our changes, and store our project remotely.

Our workshop will conclude with a wrap-up presentation and a short Q&A with some members of the Epicodus teaching staff.

<hr>

## Today's project

**Goal for the day**: Build an interactive website we could use to track our programming goals.

### Tools

Let's get familiar with the tools we'll be using today.

### Your friendly neighborhood text editor - Atom

Every web developer has a selection of tools they like to use when they're building their applications. What they have in common is the use of a robust text editor. The text editor's job is to open the files, and let the developer edit them, just the way you would edit an essay in school, or an email at work.

Here at Epicodus we use a free, open-source text editor named **Atom**. You can download it for free at [atom.io](https://atom.io/). If you're using an iMac at Epicodus, Atom is already installed and ready for you.

### The Terminal

The second tool every developer uses is a flexible **Terminal** or **Command Line** program. A Terminal is a line-by-line command interface to the developers computer. It's a powerful tool that can do simple things like create and open files, and carry out more complicated tasks like building projects, managing complicated framework dependencies and running server instances.

<hr>

### Let's get started!

Let's start by opening our **Terminal** program. You should see information similar to the following at the top of the terminal, as well as a flashing cursor.

```
Last login: Thu Apr  6 14:09:51 on ttys001
epicodus-5:~ epicodus$
```

The terminal runs at a single location on the computer, just like a file or image within the folders on your desktop. With the cursor on the terminal, enter the following command to find out where the terminal is currently running.

```
pwd
```

Press `Enter`.

You'll see the terminal return the current location, `/Users/epicodus` or similar. Let's use a command to move to the desktop and begin creating our project.

```
cd Desktop
```

The command `cd` means *change directory* and moves the location where the terminal will run. Use `pwd` again to see that we're now located at `/Users/epicodus/Desktop` or similar. The prompt in front of the cursor has also changed its text. This is a good way to keep track of where you are on your computer and within your project.

Follow along with the following commands to create your new project. Press `Enter` after each command.

* `mkdir My_Project` This will create a new folder, or directory on the desktop with the name *My_Project*. You can use any name you like, but we'll stick with this one.
* `touch My_Project/index.html` This will create a new file within the *My_Project* directory called *index.html*. It's the first file we'll be editing today.
* `cd My_Project` This will change our Terminal location to within our new directory.
* `atom .` This will tell Atom to open our new directory and get ready to write some code!

<hr>

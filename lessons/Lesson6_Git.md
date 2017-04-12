### Git and GitHub

Professional web and software developers have a wide range of tools at their disposal to help build, monitor, and collaborate on projects. One of the most common types of software is called **version control software**. The goal of good version control software is to take micro-snapshots, frequently, as a project is being built. This helps track little changes along the way, and makes it easier if you need to go back to an old version, see how something was done "back when it was working" or something like that. Good version control software also has many other uses. One is the ability to move projects around from machine to machine using the Terminal.

The most common version control software in use is called **Git**. It's easy to access via the command line or Terminal, and ties easily to one of the most common open-source code-sharing websites, **GitHub**. Our goal in this section is to help you get your code saved with Git, and hosted on GitHub so that you can view your code, or even visit your site from any computer.

Let's open the Terminal and enter a few commands. Git is complex software, that does a lot more than we need it for today. Stick to these commands, and you can't go wrong.

Make sure you're in the My_Project directory with `pwd`, then enter the following.

```
git init
```

```
git config user.name your_name (use quotes if you want to use a multiple word name)
```

```
git config user.email your_email
```

You're now set up as the author of this project.

Now we need to create a GitHub account for you. Good news, they're free, and are a staple of the developer's life. You can create an account at [github.com](http://github.com). After creating the account you'll need to visit the email address you provided, and click the link in the confirmation email GitHub has sent you.

Pick a good user name! As a developer, it might end up on your resume! GitHub also functions as a social network for developers. You can connect with people, collaborate on projects, and even find cool new libraries and tools to use.

Once you successfully register for a GitHub account, you should see a welcome message like this:




![github-welcome-message](https://www.dropbox.com/s/8e6wtzn9cd8yqpt/github-welcome-message.png?raw=1)

Now that you have an account, let's create a **repository** on GitHub. A **repository** is like creating a place to store and single project on your GitHub account. To create a new repository (almost always called a **repo**) select the `+` option in the upper-right corner of the GitHub welcome page. Then, select _New repository_ from the dropdown menu, as seen in the image below:



![create-new-repo-option](https://www.dropbox.com/s/hiz25kedobp9rom/create-new-repo.png?raw=1)

This should take you to a screen that looks like this:



![create-new-repo-screen](https://www.dropbox.com/s/qudmr5c02jpdl64/create-new-repo%20%281%29.png?raw=1)

When it asks for the name of the repo, use something easy to identify, like *workshop_project*. You don't need to alter any of the other options here, besides your _Repository name_. After entering a name, click the _Create repository_ button. This should take you to a page that looks like this:




![new-empty-repository](https://www.dropbox.com/s/jraymcr8zs3wyzq/new-empty-repo.png?raw=1)

Now that we have a GitHub account we need to link the copy of our  project saved to our computer to our new repo we've just created for it on GitHub. Copy that new URL GitHub has given you, and move back to the Terminal.



![new-github-repo-url](https://www.dropbox.com/s/463r27alnadjr2x/github-repo-url.png?raw=1)

Enter the following line into the terminal.

```
git remote add github your_URL
```

This is setting up something called a **remote** within GitHub. A remote is simply an address of a repo.

Next, enter the following commands.

```
git add .
```

```
git commit -m "add workshop project to git"
```

This will tell Git to collect all the work we've done today, and add it to a package, called a **commit**. That commit is the thing we're going to send to our repo on GitHub.

Finally, you can enter the following:

```
git push github master
```

Git will ask you to enter your username and password for GitHub, just to verify that you have the right to store your project there.

Once you've entered your password, Git will send your the local version of your project from your computer to your repo you've just created on GitHub. You can view the files online by refreshing your repo.


![project-files-on-github](https://www.dropbox.com/s/73qzc24wc5wq4ln/project-successfully-pushed-to-github.png?raw=1)

Let's take one last step. Let's let GitHub host our project, live, online.

Within your repo, click *Settings* at the top.



![github-repo-settings-option](https://www.dropbox.com/s/n674x9avuu6nipd/repo-settings-option.png?raw=1)

In the settings area, scroll down until you see a box labelled GitHub Pages. Within this box, you'll see a dropdown reading _None_. From that, select *master branch*. Then click Save.



![publishing-to-gh-pages](https://www.dropbox.com/s/as1za3ja40yqlcn/Screen%20Shot%202017-04-07%20at%205.17.33%20PM.png?raw=1)

It may take a minute to compile, but you can now scroll down to see the URL of your new hosted site! Try it out!



![github-pages-url](https://www.dropbox.com/s/4tzqf8cv1a0hv0n/Screen%20Shot%202017-04-07%20at%205.19.14%20PM.png?raw=1)

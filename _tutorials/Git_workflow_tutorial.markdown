---
layout: page
title: Git Workflow
permalink: /Git Workflow/
---

## What is GIT?

[Git](https://git-scm.com/) is a Git is a **free** and **open-source distributed version control system** that allows you as a technical writer to collaborate on projects. Think of Git as a document tracker. Rather than using the UI **(the clicking bits on the webpage)** on [GitHub](https://github.com/), you can use a terminal on a code editor like [Visual Studio Code](https://code.visualstudio.com/) to send your documents to your GitHub repository. 

That's it! That's all you need to know to get started. 

In plain English, when you write a document on **Word**, name it, save it to your cloud. Everyone on your team can access it if you permit them. The only difference is that the primary document won't get modified because everyone is working on an isolated version of the word document. So, technically, your team's edits do not exist until **you** all agree on the changes to the main document. As far as Git is concerned,  your edits don't matter until you **tell** Git they do.

### Set up a Github account 

- Set up a [GitHub](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home) account. 
- Create a [Repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository).

After creating a Github account, go to your repository to create a new file and save it. Type in some text, and submit your changes. 

### Set up Visual Studio Code 

1. Download and install [Visual Studio Code](https://code.visualstudio.com/).
2. Check to make sure Git is on your computer, open the **command prompt** application, and type `git --version.` The version type will show up. If the version type does not return, then you need to install [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

### Create a Folder from Visual Studio Code
1. Open Visual studio.
2. Go to **file>** **open folder>** **documents** and create a new folder called **projects**.
3. Select **folder**. You are now in your newly created VS code called **project**.

### Clone your repository to your computer 
1. Go to Github, and go to the repository you created earlier.
2. Select **add file>**. Select **create new file**.
3. Type `this is easy, it's not so bad, I am awesome for even getting this far`
4. Scroll down, under **commit new file**, select **commit new file**.
5. Select the **code** drop-down menu, and copy the link that shows up. 
6. Go back to VS code. We are going to the **Terminal** to clone the remote repository - in lay terms; we will copy and paste the contents of the repository to your **projects** folder
7. Go to **Terminal** **>** **New Terminal**. A panel just opened up on your bottom screen. 
8. On the right panel options, select **bash**.

Think of your Git commands as you think of how you interact with a UI when saving a file. Think of steps you would take to save and upload a file to the could. 
1. Open a text editor
2. Type in some words 
3. Select **save as**
4. Name the File 
5. Choose a location 
6. Select **save**

In this case, we have done this on GitHub, but we want to work on our computers because there could be other teams working on the same repository, and we don't want to mess things up for others.

In the Terminal, the first line of code will look like this `peach@mario NIN64 ~/Documents/Projects (master)`. That's your computer name, your file directory. 

### Git

`git clone` is used to create a copy of remote repositories, in this case, the repository you just created on GitHub.

1. Type `git clone` and paste the link you copied from your repository after it.
2. Type `git branch`. The **terminal** will return `(main)$ git branch* main`. 
3. In VS code, navigate to the **test** file, and add some text `this is not so bad. It is making sense`.
4. Save your changes with `crtl+s`.
5. Go to the **terminal** and type `git status`.
6. Read the message in the **terminal**. What does it say? Get familiar with the returned messages in the **terminal**.
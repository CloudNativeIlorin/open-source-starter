# Clone the Project 💻

You've forked the project. Now it's time to get a copy of your fork onto your computer.

This process is called **cloning**.

Don't worry if you've never used the terminal before. We'll go step by step.

---

## What does "clone" mean?

A **clone** is a copy of a GitHub repository on your computer.

For example, you now have:

```text
GitHub
   ↓
Your fork of open-source-starter
   ↓
Your computer
```

This allows you to make changes to the project on your computer and later send those changes back to GitHub.

### Fork vs Clone

These two words are easy to mix up.

**Fork** = creates your own copy of a repository on GitHub.

**Clone** = downloads that copy from GitHub to your computer.

So the usual flow is:

```text
CNI repository
     ↓
    Fork
     ↓
Your GitHub repository
     ↓
   Clone
     ↓
Your computer
```

---

## Before you start

You'll need:

* A GitHub account
* Your fork of `open-source-starter`
* Git installed on your computer

If you haven't installed Git yet, go back to [Git Basics](./04-git-basics.md).

You can check whether Git is installed by opening your terminal and running:

```bash
git --version
```

If Git is installed, you'll see something similar to:

```text
git version 2.x.x
```

The exact version doesn't matter.

---

## Step 1: Open your fork

Go to your GitHub profile and open the fork you created in the previous lesson.

Make sure you're looking at **your fork**, not the original CNI repository.

Your repository URL should look something like:

```text
https://github.com/YOUR-USERNAME/open-source-starter
```

Replace `YOUR-USERNAME` with your actual GitHub username.

---

## Step 2: Copy the repository URL

On your fork's GitHub page:

1. Click **Code**.
2. Make sure **HTTPS** is selected.
3. Copy the repository URL.

It should look like:

```text
https://github.com/YOUR-USERNAME/open-source-starter.git
```

Keep this URL handy. We'll use it in the next step.

---

## Step 3: Open your terminal

A terminal is simply a way to interact with your computer by typing commands.

### Windows

You can use:

* Git Bash
* PowerShell
* Windows Terminal

If you installed Git for Windows, **Git Bash** is a good option for following this guide.

### macOS

You can use:

* Terminal
* iTerm2

### Linux

You can use:

* Your preferred terminal application

---

## Step 4: Choose where to keep the project

Before cloning, move into the folder where you want your project to live.

For example:

```bash
cd Desktop
```

This means:

> "Move into my Desktop folder."

You can use another folder if you'd prefer.

If you're not comfortable with `cd` yet, that's okay. The important thing is understanding that Git will create the project folder wherever you run the clone command.

---

## Step 5: Clone your fork

Run:

```bash
git clone https://github.com/YOUR-USERNAME/open-source-starter.git
```

Replace `YOUR-USERNAME` with your GitHub username.

For example:

```bash
git clone https://github.com/janedoe/open-source-starter.git
```

Git will download your repository and create a folder called:

```text
open-source-starter
```

You'll see output showing Git downloading the project.

---

## Step 6: Move into the project

Once cloning is complete, run:

```bash
cd open-source-starter
```

You're now inside the project folder.

You can check this by running:

```bash
git status
```

You should see something similar to:

```text
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
```

Don't worry if your message looks slightly different.

The important thing is that Git recognizes the folder as a repository.

---

## What just happened?

You have now connected three things:

```text
CNI's repository
       ↓
Your fork on GitHub
       ↓
Your local copy on your computer
```

Your local copy knows where your GitHub fork lives.

Git calls that remote repository **origin**.

You can see it by running:

```bash
git remote -v
```

You'll see something similar to:

```text
origin  https://github.com/YOUR-USERNAME/open-source-starter.git (fetch)
origin  https://github.com/YOUR-USERNAME/open-source-starter.git (push)
```

This tells Git where to get updates from and where to send your changes.

---

## A common mistake

Make sure you clone **your fork**, not the original CNI repository.

### Your fork

```text
https://github.com/YOUR-USERNAME/open-source-starter.git
```

### CNI's original repository

```text
https://github.com/cloud-native-ilorin/open-source-starter.git
```

For this beginner workflow, you should clone **your fork**.

Why?

Because you'll be making changes there first.

Later, you'll send those changes to CNI through a **Pull Request**.

---

## You've cloned the project 🎉

At this point you should have:

* Your fork on GitHub
* A local copy on your computer
* Git connected to your fork

The next step is to create a **branch**.

Don't worry — a branch is much simpler than it sounds.

We'll explain it in the next lesson.

---

**Next:** [Create a Branch →](./07-create-a-branch.md)

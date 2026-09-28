# Git Basics 🧑🏾‍💻

You've heard about Git.

You've heard about GitHub.

Now let's understand **Git** a little better.

Don't worry — you don't need to become a Git expert to make your first contribution.

We'll only focus on the things you actually need to get started.

---

## What Is Git?

Git is a tool that helps you **track changes to files**.

Imagine you're working on a document.

You make a change.

Then another change.

Then you realize that something you changed earlier was actually better.

Without a way to track your work, it can become difficult to know:

* What changed?
* Who changed it?
* When did it change?
* What did the file look like before?
* Can I go back to an earlier version?

Git helps solve this problem.

It keeps a history of your work.

---

# Why Do Open-Source Projects Use Git?

Open-source projects are usually worked on by many people.

Imagine 20 people working on the same project.

One person is fixing a bug.

Another is adding a feature.

Someone else is improving documentation.

Another person is working on something completely different.

Git helps everyone keep track of their changes without everyone having to work directly on the same version at the same time.

That's why Git is so important in open source.

---

# Git Is Not GitHub

This is worth repeating.

**Git ≠ GitHub**

Git is the version control tool.

GitHub is a platform that allows people to host Git repositories and collaborate around them.

A simple way to think about it:

```text
Git
↓
Tracks your changes

GitHub
↓
Helps you share and collaborate on those changes
```

You'll use them together, but they are different things.

---

# 🖥️ Do I Need to Use the Terminal?

Eventually, we'll show you how to use Git from the command line.

But don't panic when you see a terminal.

A terminal is simply a way of interacting with your computer by typing commands.

For example:

```bash
pwd
```

This asks your computer:

> "Where am I right now?"

And:

```bash
ls
```

asks:

> "What files and folders are here?"

That's it.

The terminal might look intimidating at first, but you'll get comfortable with it by using it.

---

# Installing Git

Before you can use Git from your computer, you need to install it.

## Windows

Download Git from the official Git website.

➡️ [Download Git for Windows](https://git-scm.com/download/win)

After installing it, open **Git Bash**.

You can also use PowerShell or another terminal, but we'll use Git Bash in our examples because it works well for beginners.

## macOS

You can install Git using the official installer or through tools such as Homebrew.

➡️ [Git downloads](https://git-scm.com/downloads)

## Linux

Git is available through most Linux package managers.

For example, on Ubuntu:

```bash
sudo apt install git
```

If you're unsure how to install Git on your operating system, don't worry.

You can ask the CNI community for help.

---

# Check If Git Is Installed

Open your terminal and run:

```bash
git --version
```

You should see something similar to:

```text
git version 2.x.x
```

The exact version number may be different.

If you see a Git version, you're ready.

---

# ⚙️ Configure Git

Before making commits, Git needs to know who you are.

You'll normally configure your name and email once on your computer.

Run:

```bash
git config --global user.name "Your Name"
```

Replace `Your Name` with your name.

For example:

```bash
git config --global user.name "John Doe"
```

Then configure your email:

```bash
git config --global user.email "your-email@example.com"
```

Use the email address associated with your GitHub account, or an appropriate GitHub-provided privacy email if you prefer.

You can check your settings with:

```bash
git config --global --list
```

---

# 📁 What Is a Git Repository?

A Git repository is a project that Git is tracking.

When you clone an existing GitHub project, you get a copy of its repository on your computer.

You can then make changes to it and use Git to keep track of those changes.

---

# 🔄 The Basic Git Workflow

Most of the time, you'll follow a process something like this:

```text
Get the project
     ↓
Create a branch
     ↓
Make changes
     ↓
Check your changes
     ↓
Commit your changes
     ↓
Push your changes
```

Let's break down the important commands.

---

# 📥 `git clone`

`git clone` downloads a Git repository to your computer.

For example:

```bash
git clone https://github.com/USERNAME/REPOSITORY.git
```

This creates a local copy of the repository.

We'll use this properly in the next guide.

---

# 🌿 `git branch`

Branches allow you to work on changes separately from the main project.

You can see your branches with:

```bash
git branch
```

You can create a new branch with:

```bash
git branch my-first-contribution
```

But there's a shorter way to create **and switch to** a new branch:

```bash
git switch -c my-first-contribution
```

We'll use this later.

---

# 🔍 `git status`

This is one of the most useful Git commands.

Run:

```bash
git status
```

It tells you what is happening in your repository.

For example, it can tell you:

* Which branch you're on
* Which files you've changed
* Which files are new
* Which changes haven't been committed

If you're ever unsure about what's happening, try:

```bash
git status
```

Think of it as asking Git:

> **"What's going on right now?"**

---

# ➕ `git add`

After making changes, you need to tell Git which changes you want to include in your next commit.

For one file:

```bash
git add filename.md
```

For example:

```bash
git add README.md
```

To add all changed files:

```bash
git add .
```

The `.` means the current directory.

Don't worry if this doesn't completely make sense yet. You'll see it in practice soon.

---

# 💾 `git commit`

A commit saves a snapshot of your changes in Git's history.

For example:

```bash
git commit -m "Improve the README"
```

The part inside the quotation marks is the commit message.

Try to make commit messages describe what you changed.

For example:

```text
Fix typo in GitHub guide
```

is more useful than:

```text
changes
```

---

# 📤 `git push`

A commit saves your changes locally.

But your changes aren't automatically on GitHub.

That's where `git push` comes in.

```bash
git push
```

This sends your committed changes from your computer to the remote repository on GitHub.

Think of it like:

```text
Your computer
     │
     │ git push
     ▼
GitHub
```

---

# 📥 `git pull`

Sometimes other people make changes to a project while you're working.

`git pull` gets the latest changes from the remote repository and brings them into your local repository.

```bash
git pull
```

You'll learn more about this as you start working with real projects.

---

# 🔎 `git diff`

You can use:

```bash
git diff
```

to see changes you've made that Git hasn't staged yet.

This is useful when you want to check your work before committing it.

---

# 🧠 The Commands You Need First

Don't try to memorize every Git command.

For your first contribution, these are the important ones:

| Command         | What it does                     |
| --------------- | -------------------------------- |
| `git clone`     | Downloads a repository           |
| `git status`    | Shows what's happening           |
| `git switch -c` | Creates and switches to a branch |
| `git add`       | Prepares changes for a commit    |
| `git commit`    | Saves a snapshot of your changes |
| `git push`      | Sends your changes to GitHub     |
| `git pull`      | Gets new changes from GitHub     |
| `git diff`      | Shows your changes               |

You'll become familiar with these through practice.

---

# 🧩 A Small Example

Imagine you have cloned a project and want to fix a typo.

You might do:

```bash
git switch -c fix-typo
```

Make your change.

Then:

```bash
git status
```

Check what changed.

Then:

```bash
git add .
```

Prepare the change.

Then:

```bash
git commit -m "Fix typo in documentation"
```

Save the change.

Then:

```bash
git push -u origin fix-typo
```

Send your branch to GitHub.

After that, you can open a Pull Request on GitHub.

That's the basic workflow we'll eventually use.

---

# ⚠️ Don't Copy Commands You Don't Understand

It's tempting to find a Git command online and paste it into your terminal.

Try not to do that blindly.

If you don't understand what a command does, **ask first**.

Some Git commands can change or delete things in your working directory.

Throughout this guide, we'll explain what each command does before asking you to use it.

---

# 🌱 You Don't Need to Know Git Before Starting

Remember why we're here.

You're not expected to become a Git expert.

We're learning enough to participate in open-source projects.

The best way to learn Git is to use it.

And that's what we're going to do next.

---

# 🚀 What's Next?

Now that you understand the basics of Git, we're going to start working with an actual repository.

You'll learn how to **fork the CNI Open Source Starter repository** and create your own copy.

➡️ **[Your First Fork](05-your-first-fork.md)**

This is where the theory starts becoming practical.

---

## 💡 Remember

You don't need to memorize Git commands.

Understand what you're trying to accomplish, then use the commands that help you get there.

**Learn a little. Try it. Make mistakes. Try again.**

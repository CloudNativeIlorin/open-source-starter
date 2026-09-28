# What Is GitHub? 🐙

If you've never used GitHub before, the first thing you should know is:

**You don't need to understand everything about GitHub before you start.**

We'll take it one step at a time.

---

## So, What Is GitHub?

GitHub is a platform where people can **store projects, collaborate with others, track changes, and contribute to open-source projects.**

Think of it as a place where a group of people can work on a project together, even when they're in different places.

For example, imagine CNI is working on a guide.

One person writes it.

Another person notices a mistake.

Someone else improves the explanation.

Another person adds an example.

GitHub gives everyone a way to work together without overwriting each other's work.

---

# GitHub vs Git

You will hear these two words a lot:

**Git** and **GitHub**.

They are related, but they are not the same thing.

### Git

Git is a **version control system**.

It helps you keep track of changes made to files over time.

Imagine you're writing a document.

You make a change.

Then another change.

Then another.

Git helps keep a history of those changes so you can see what happened and work safely with other people.

### GitHub

GitHub is a platform built around Git.

It gives people a place to:

* Store Git repositories
* Collaborate
* Review changes
* Track issues
* Discuss ideas
* Manage projects
* Contribute to open-source projects

A simple way to remember it:

> **Git is the tool. GitHub is a platform where people use Git to collaborate.**

---

# 📁 What Is a Repository?

You'll hear the word **repository**, or simply **repo**, a lot.

A repository is basically a project space.

It can contain:

* Code
* Documentation
* Images
* Configuration files
* Guides
* Other project files

For example, this project you're currently reading is stored inside a GitHub repository.

Our repository is:

```text
open-source-starter
```

Inside it, we have things like:

```text
README.md
CONTRIBUTING.md
docs/
```

So when someone says:

> "Check the repository."

They're basically saying:

> "Go to the project's GitHub space."

---

# 🐛 What Is an Issue?

An **Issue** is a way to communicate about something that needs attention in a project.

For example:

> "The installation instructions are confusing."

Someone could create an issue explaining the problem.

Another example:

> "Can we add a dark mode?"

That could also be an issue.

Issues can be used for:

* Reporting bugs
* Suggesting improvements
* Asking questions
* Discussing ideas
* Requesting features
* Tracking tasks

Think of an issue as a conversation or task around something related to the project.

---

# 🍴 What Is a Fork?

A **fork** is your own copy of someone else's repository on GitHub.

Let's say Cloud Native Ilorin has a repository called:

```text
open-source-starter
```

You want to make changes to it.

You may not have permission to directly change the original repository.

So you can **fork** it.

GitHub creates a copy under your own account.

For example:

```text
Cloud Native Ilorin
        │
        │ fork
        ▼
Your GitHub account
```

You can then make changes to your copy.

Later, you can ask the original project to include your changes.

That's where a Pull Request comes in.

We'll explain that shortly.

---

# 🌿 What Is a Branch?

A **branch** is a separate line of work inside a repository.

Imagine the main project is a road:

```text
=============================
          main
```

You want to work on something without changing the main project immediately.

So you create another path:

```text
=============================
          main
              \
               \============= your-work
```

You can make your changes on your branch without affecting the main branch.

Once your work is ready, you can propose adding those changes to the main project.

---

# 💾 What Is a Commit?

A **commit** is a saved set of changes.

Imagine you've edited a file.

You changed three things:

* Fixed a spelling mistake
* Added an explanation
* Added an example

You can create a commit that records those changes.

A commit also usually has a message explaining what you changed.

For example:

```text
Fix spelling mistakes in the GitHub guide
```

Think of a commit as a checkpoint in your work.

---

# 📤 What Is a Pull Request?

This is one of the most important concepts you'll learn.

A **Pull Request**, usually called a **PR**, is a request to merge your changes into another branch or repository.

Imagine you fork the CNI project.

You make some improvements.

Now you want CNI to look at your changes.

You open a Pull Request.

You're essentially saying:

> "I've made these changes. Please review them and consider adding them to the project."

Other contributors can then:

* Review your changes
* Ask questions
* Suggest improvements
* Approve the changes

If everything looks good, the changes can be merged.

---

# 🔄 The Basic GitHub Contribution Flow

You'll see this process again and again.

For example:

```text
Find a project
     ↓
Fork the repository
     ↓
Clone your fork
     ↓
Create a branch
     ↓
Make your changes
     ↓
Commit your changes
     ↓
Push your branch
     ↓
Open a Pull Request
     ↓
Project maintainers review it
     ↓
Make changes if needed
     ↓
Your contribution gets merged 🎉
```

Don't worry if this looks complicated.

**You are not expected to remember it yet.**

We'll walk through every step later.

---

# 👀 What Does "Maintainer" Mean?

You'll also hear the word **maintainer**.

A maintainer is someone who helps take care of a project.

Depending on the project, maintainers might:

* Review contributions
* Manage issues
* Make releases
* Guide the project's direction
* Help the community
* Keep the project healthy

When you submit a Pull Request, a maintainer or another contributor may review your work.

---

# 🏠 A Simple Example

Let's put everything together.

Imagine CNI has a repository called:

```text
open-source-starter
```

You notice a spelling mistake in one of the guides.

You want to fix it.

You could:

### Step 1

Fork the repository.

You now have your own copy.

### Step 2

Create a branch.

For example:

```text
fix-spelling
```

### Step 3

Make the change.

You fix the spelling mistake.

### Step 4

Commit the change.

For example:

```text
Fix spelling mistake in GitHub guide
```

### Step 5

Push your branch to GitHub.

### Step 6

Open a Pull Request.

You tell the project:

> "I fixed this spelling mistake. Please review my change."

### Step 7

Someone reviews your change.

They may approve it or suggest an improvement.

### Step 8

The change gets merged.

🎉 **You just contributed to an open-source project.**

It was a small contribution, but it is still a real contribution.

---

# 🧠 Don't Try to Memorize Everything

At this point, you only need to understand the basic ideas.

| Term         | Simple meaning                                 |
| ------------ | ---------------------------------------------- |
| Git          | Tracks changes to files                        |
| GitHub       | Platform for collaborating around Git projects |
| Repository   | A project's space                              |
| Issue        | A discussion, problem, task or request         |
| Fork         | Your GitHub copy of another repository         |
| Branch       | A separate line of work                        |
| Commit       | A saved set of changes                         |
| Pull Request | A request to review and merge your changes     |
| Maintainer   | Someone who helps maintain a project           |

We'll use these terms throughout the rest of this journey.

If you forget something, come back to this page.

---

# 🚀 What's Next?

Now that you understand the basic GitHub concepts, we'll introduce **Git** itself.

You don't need to be a command-line expert.

We'll start with only the Git concepts and commands you actually need for your first contribution.

➡️ **[Git Basics](04-git-basics.md)**

---

## 💡 Remember

You don't need to understand every part of GitHub before contributing.

You just need to understand the next step.

We'll learn the rest as we go.

**One step at a time.**

# Commit and Push Your Changes 🚀

You've made your first change.

Now we need to save that change with Git and send it to your GitHub fork.

There are two separate steps:

```text
Commit → save your changes in Git
Push   → send those commits to GitHub
```

Let's go through them one at a time.

---

## Commit vs Push

These two words can sound confusing at first.

### Commit

A **commit** records a snapshot of your changes in your local Git repository.

Think of it like saying:

> "I'm happy with this change. Save this version."

### Push

A **push** sends your local commits to your repository on GitHub.

Think of it like saying:

> "Send my saved changes to GitHub."

So:

```text id="1cnzq7"
Your computer
     │
     │ commit
     ▼
Local Git history
     │
     │ push
     ▼
Your GitHub fork
```

---

## Step 1: Check your changes

Before committing anything, run:

```bash
git status
```

You should see something like:

```text
On branch add-my-name

Changes not staged for commit:
  modified:   CONTRIBUTORS.md
```

If you want to double-check the actual changes, run:

```bash
git diff
```

Make sure everything looks correct before continuing.

---

## Step 2: Stage your change

Git doesn't automatically include every changed file in your next commit.

We first need to tell Git which changes we want to commit.

Run:

```bash
git add CONTRIBUTORS.md
```

This stages the file.

You can think of staging as putting the change into a box labelled:

> "Include this in my next commit."

---

## Step 3: Check the status again

Run:

```bash
git status
```

You should now see something similar to:

```text
Changes to be committed:
  modified:   CONTRIBUTORS.md
```

The file is now ready to be committed.

---

## Step 4: Create your commit

Now create the commit:

```bash
git commit -m "Add my name to contributors"
```

The part inside the quotation marks is your **commit message**.

A commit message should briefly explain what the commit does.

For example:

```text
Add my name to contributors
```

is better than:

```text
changes
```

because someone looking at the project history can immediately understand what you changed.

---

## Step 5: Check your status

Run:

```bash
git status
```

You should see something similar to:

```text
On branch add-my-name
nothing to commit, working tree clean
```

This means your changes have been committed locally.

But they aren't on GitHub yet.

That's where **push** comes in.

---

# Push Your Changes to GitHub

Now we're going to send your commit to your GitHub fork.

Run:

```bash
git push -u origin add-my-name
```

Let's break that command down.

### `git push`

Tells Git:

> "Send my commits to a remote repository."

### `origin`

`origin` is the name Git gave to your GitHub fork when you cloned it.

You can check it with:

```bash
git remote -v
```

### `add-my-name`

This is the branch we're pushing.

### `-u`

This connects your local branch with the branch on GitHub.

You usually won't need to include `-u` the next time you push to this branch.

---

## What happens next?

Git will upload your commit to your GitHub fork.

You may see output similar to:

```text
Enumerating objects...
Counting objects...
Writing objects...
To https://github.com/YOUR-USERNAME/open-source-starter.git
 * [new branch]      add-my-name -> add-my-name
```

The exact output will be different for everyone.

---

## Check GitHub

Go back to your GitHub fork in your browser.

You should now see your branch:

```text
add-my-name
```

Your change is now on GitHub.

🎉 You just pushed your first contribution!

---

## The workflow so far

You've now learned:

```text
Fork
 ↓
Clone
 ↓
Create a branch
 ↓
Make a change
 ↓
git add
 ↓
git commit
 ↓
git push
```

There's one final step before your contribution can become part of the CNI project.

You need to tell CNI:

> "I've made this change. Can you review it?"

That's done with a **Pull Request**.

---

## What if Git asks you to sign in?

The first time you push, GitHub may ask you to authenticate.

That's normal.

Follow GitHub's authentication instructions.

If you're using GitHub through HTTPS, you may be asked to authenticate through your browser or another GitHub-supported method.

**Don't put your GitHub password directly into a Git command.**

If authentication doesn't work, stop and check the error message rather than repeatedly trying random commands.

---

## What if you get an error?

Don't panic.

Git errors are normal, even for experienced developers.

If you get an error, copy the error message and look at what it says.

For example:

```text
Permission denied
```

usually means GitHub isn't accepting your authentication or you don't have permission to push to that repository.

That's different from an error in your code.

You can also ask someone in the CNI community for help.

Learning how to read Git errors is part of learning Git.

---

## One important habit

Don't blindly copy commands without understanding what they do.

For this lesson, remember:

```text
git add      → choose what to commit
git commit   → save a snapshot locally
git push     → send commits to GitHub
```

You'll use these commands constantly as you contribute to open source.

---

## You're almost there 🎉

Your change is now sitting on your GitHub fork.

The original CNI repository hasn't been changed.

That's intentional.

Next, you'll open a **Pull Request** asking CNI to review your change.

**Next:** [Open a Pull Request →](./10-open-a-pull-request.md)

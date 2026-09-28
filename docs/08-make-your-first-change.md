# Make Your First Change 🎉

You've forked the project, cloned it to your computer, and created your own branch.

Now you're ready to make your **first contribution**.

And no, you don't need to write code.

For this first contribution, you're simply going to add your name to the project's contributors list.

---

## What are we changing?

Earlier, we created a file called:

```text
CONTRIBUTORS.md
```

This file contains the names of people who have contributed to the project.

You're going to add yourself to that list.

---

## Step 1: Open the project

Open the `open-source-starter` folder on your computer.

Inside it, you should see something similar to:

```text
open-source-starter/
│
├── README.md
├── CONTRIBUTING.md
├── CONTRIBUTORS.md
├── CODE_OF_CONDUCT.md
│
└── docs/
```

Your project may contain additional files. That's okay.

---

## Step 2: Open `CONTRIBUTORS.md`

Open:

```text
CONTRIBUTORS.md
```

You can use any text editor you are comfortable with.

For example:

* Visual Studio Code
* Notepad
* Sublime Text
* Cursor
* Any other text editor

You don't need a special coding editor just to complete this task.

---

## Step 3: Find the Contributors section

You should see something similar to:

```md
## Contributors

- Cloud Native Ilorin — [@cloud-native-ilorin](https://github.com/cloud-native-ilorin)
```

Under the CNI entry, add your own name.

Use this format:

```md
- Your Name — [@your-github-username](https://github.com/your-github-username)
```

For example, if your name is Jane Doe and your GitHub username is `janedoe`:

```md
- Cloud Native Ilorin — [@cloud-native-ilorin](https://github.com/cloud-native-ilorin)
- Jane Doe — [@janedoe](https://github.com/janedoe)
```

Replace the example with your own name and GitHub username.

---

## Step 4: Save the file

Save `CONTRIBUTORS.md`.

That's it.

You just made a change to an open-source project.

But we're not done yet.

The change currently exists **only on your computer**.

We need to tell Git about it and send it to your GitHub fork.

---

## Step 5: Check what changed

Open your terminal inside the `open-source-starter` folder.

Run:

```bash
git status
```

You should see something similar to:

```text
On branch add-my-name

Changes not staged for commit:
  modified:   CONTRIBUTORS.md
```

This is Git telling you:

> "I noticed that you changed `CONTRIBUTORS.md`."

---

## Step 6: Look at your change

You can ask Git to show you exactly what changed:

```bash
git diff
```

You should see your new line highlighted in the output.

For example:

```diff
+ - Jane Doe — [@janedoe](https://github.com/janedoe)
```

The `+` means that line was added.

This is a useful habit.

Before committing your work, take a moment to check what Git thinks you changed.

---

## What if `git status` doesn't show the change?

First, make sure:

1. You saved the file.
2. You're inside the correct `open-source-starter` folder.
3. You're on the `add-my-name` branch.

You can check the branch with:

```bash
git branch
```

You should see:

```text
* add-my-name
  main
```

If everything looks correct, run:

```bash
git status
```

again.

---

## Why is this a contribution?

You might be thinking:

> "I only added my name. Does that really count?"

Yes.

You're learning the same workflow used for much larger contributions:

```text
Make a change
     ↓
Check the change
     ↓
Commit it
     ↓
Push it
     ↓
Open a Pull Request
     ↓
Get it reviewed
     ↓
Merge
```

The change itself is small.

The **workflow** is what you're learning.

Once you understand this process, you can use it to:

* Fix documentation
* Correct a typo
* Add a tutorial
* Improve an example
* Report or fix a bug
* Add code
* Improve tests
* Add translations
* Update configuration
* And much more

---

## You made your first open-source change 🎉

Take a moment to appreciate this.

You started with:

> "I don't know how open source works."

Now you've:

* Created a GitHub account
* Found an open-source project
* Forked a repository
* Cloned it
* Created a branch
* Changed a project file

The next step is to **commit your change**.

A commit is basically Git's way of recording a snapshot of the work you've done.

**Next:** [Commit and Push Your Changes →](./09-commit-and-push.md)

# Open a Pull Request 🔄

You've made your change, committed it, and pushed it to your GitHub fork.

Now it's time to send your change to the CNI project for review.

This is called a **Pull Request**, often shortened to **PR**.

---

## What is a Pull Request?

A Pull Request is a way of saying:

> "I've made some changes. Can you review them and consider adding them to the project?"

It does **not** mean your changes are automatically added.

The project maintainers get a chance to:

* Review your changes
* Ask questions
* Suggest improvements
* Request changes
* Approve the contribution
* Merge it into the project

This is how collaboration happens in open source.

---

## Your contribution so far

Here's what you've done:

```text id="cvn9j2"
CNI repository
      ↓
     Fork
      ↓
Your GitHub fork
      ↓
    Clone
      ↓
Your computer
      ↓
Create branch
      ↓
Make your change
      ↓
   Commit
      ↓
    Push
      ↓
Your GitHub fork
```

Now we're going to create the Pull Request:

```text id="7lq9yx"
Your fork
    ↓
Pull Request
    ↓
CNI repository
```

---

# Step 1: Open your fork on GitHub

Go to your `open-source-starter` repository on GitHub.

You should see your recently pushed branch.

GitHub may show a message or button asking you to create a Pull Request for your recently pushed branch.

If you see something like:

**Compare & pull request**

click it.

If you don't see it, that's okay.

You can create a Pull Request manually.

---

# Step 2: Start the Pull Request

Click:

**Pull requests**

Then click:

**New pull request**

GitHub will show you two sides:

```text id="y2q6x7"
base repository     ←     head repository

CNI project               Your fork
```

The exact wording can vary slightly depending on GitHub's current interface.

The important thing is getting the direction right.

You want:

```text id="4m1k3j"
YOUR BRANCH
     ↓
CNI's main branch
```

For example:

```text id="v7ypq1"
base: cloud-native-ilorin/open-source-starter
      main

compare: your-username/open-source-starter
         add-my-name
```

**This is very important.**

You are asking CNI to pull your changes **from your branch into CNI's `main` branch**.

---

# Step 3: Check the changes

Before creating the Pull Request, GitHub will show you the files and changes included.

Look through them.

You should see the change you made to:

```text id="8s8u7y"
CONTRIBUTORS.md
```

You should see your new contributor entry.

For example:

```diff id="z6hj4c"
+ - Jane Doe — [@janedoe](https://github.com/janedoe)
```

If you see unrelated changes that you didn't intend to make, **don't create the Pull Request yet**.

Go back and check your branch.

---

# Step 4: Give your Pull Request a title

Your Pull Request title should briefly explain what you're contributing.

For this exercise, use something like:

```text id="7gn1tc"
Add my name to contributors
```

A good title makes it easy for maintainers to understand what the Pull Request is about.

Compare:

❌

```text
My first PR
```

with:

✅

```text
Add my name to contributors
```

The second one tells the maintainer exactly what changed.

---

# Step 5: Write a short description

The description gives the maintainer a little more context.

For your first contribution, you can keep it simple.

For example:

```text id="a2v9fz"
## What did you change?

Added my name and GitHub username to CONTRIBUTORS.md.

## Why?

This is my first contribution to the CNI Open Source Starter project.
```

You don't need to write a long explanation.

As your contributions become more complex, your Pull Request descriptions can become more detailed.

---

# Step 6: Create the Pull Request

Once you've checked everything:

Click:

**Create pull request**

🎉

You've officially opened your first Pull Request.

---

# What happens now?

Your Pull Request is now visible to the CNI project maintainers.

They can review your changes.

You may see a page showing something like:

```text
Add my name to contributors

Open

your-username wants to merge 1 commit into
cloud-native-ilorin:main
from
your-username:add-my-name
```

The exact layout may differ, but the idea is the same.

Your contribution is now waiting for review.

---

# Don't worry if someone asks you to make changes

This is completely normal.

A maintainer might say:

> "Could you change the formatting?"

or:

> "Please put your name alphabetically."

or:

> "Can you fix this link?"

That doesn't mean you failed.

**Code review and contribution review are normal parts of open source.**

You make the requested change on your branch, commit it, and push again.

Your Pull Request automatically updates.

You don't need to create another Pull Request.

---

# What if your Pull Request is approved?

If the maintainers are happy with your contribution, they can merge it.

Your change will then become part of the CNI project.

The journey looks like this:

```text id="h8i7n2"
Make a change
      ↓
Commit
      ↓
Push
      ↓
Pull Request
      ↓
Review
      ↓
Approved
      ↓
Merged 🎉
```

And that's your first open-source contribution.

---

# What if your Pull Request is rejected?

Don't take it personally.

A Pull Request can be closed for many reasons.

For example:

* The change isn't needed anymore
* Someone else already fixed the issue
* The contribution doesn't fit the project
* The approach needs to be changed
* The project has different requirements

A closed Pull Request is still a learning experience.

You can ask for feedback and use what you learned in your next contribution.

---

# A Pull Request is a conversation

One of the most important things to understand is that a Pull Request isn't just a button.

It's a place where contributors and maintainers can work together.

You can:

* Explain your approach
* Ask questions
* Respond to feedback
* Make additional commits
* Discuss alternatives
* Learn from experienced contributors

That's one of the things that makes open source different from simply uploading code somewhere.

---

# Your first contribution

If your Pull Request gets merged, take a moment to celebrate.

You started with:

> "I don't know how open source works."

And now you've:

* Found an open-source project
* Forked it
* Cloned it
* Created a branch
* Made a change
* Committed it
* Pushed it
* Opened a Pull Request
* Gone through review

That's a real contribution.

🎉 **Welcome to open source!**

---

## What's next?

Getting your first Pull Request merged is only the beginning.

In the next lesson, we'll explain what happens **after you open a Pull Request** — including reviews, requested changes, approvals, merging, and what you should do after your contribution is accepted.

**Next:** [What Happens Next? →](./11-what-happens-next.md)

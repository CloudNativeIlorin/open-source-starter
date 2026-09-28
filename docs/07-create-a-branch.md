# Create a Branch 🌿

You've cloned the project and now have it on your computer.

Before making any changes, we're going to create a **branch**.

If you've never used branches before, don't worry. The idea is simple.

---

## What is a branch?

A branch is a separate workspace for making changes without directly changing the main version of the project.

Think of it like making a copy of a document before editing it.

The main project stays untouched while you work on your changes.

```text
main
 │
 └── your branch
       │
       ├── your changes
       └── your commits
```

When you're happy with your changes, you can propose adding them to the main project through a **Pull Request**.

---

## Why do we use branches?

Imagine 10 people are contributing to the same project.

If everyone made changes directly to `main`, things could get messy very quickly.

Instead, each person can work on their own branch:

```text
main
 ├── add-contributor
 ├── fix-typo
 ├── improve-docs
 └── update-design
```

Everyone can work independently.

The project maintainers can then review each person's changes before they become part of `main`.

---

## Step 1: Check which branch you're currently on

Inside your `open-source-starter` folder, run:

```bash
git branch
```

You should see something similar to:

```text
* main
```

The `*` tells you which branch you're currently on.

---

## Step 2: Create your branch

For your first contribution, we're going to add your name to the contributors list.

Create a branch called:

```text
add-my-name
```

Run:

```bash
git switch -c add-my-name
```

You should see something similar to:

```text
Switched to a new branch 'add-my-name'
```

That's it.

You've created your first branch.

---

## Step 3: Check your branch

Run:

```bash
git branch
```

You should now see:

```text
* add-my-name
  main
```

The `*` is now beside `add-my-name`.

That means you're working on your new branch.

---

## What did we just do?

Before:

```text
main
```

After:

```text
main
  \
   add-my-name
```

Your new branch started from `main`.

Any changes you make now will happen on `add-my-name`.

The `main` branch remains unchanged.

---

## Branch names

You can choose different names depending on what you're working on.

For example:

```text
add-my-name
fix-typo
update-readme
improve-documentation
add-tutorial
fix-broken-link
```

A good branch name should tell people what you're working on.

For your first contribution, `add-my-name` is perfectly fine.

---

## A small but important habit

Before you start working, always check which branch you're on.

Run:

```bash
git branch
```

If you see:

```text
* add-my-name
```

you're good to go.

If you see:

```text
* main
```

you're on the main branch.

Don't make your contribution there.

Switch to your working branch first.

---

## You're ready to make your first change 🎉

You now have:

```text
GitHub
   │
   └── Your fork
          │
          ↓
      Your computer
          │
          ↓
      add-my-name
          │
          ↓
     Your changes
```

The next step is where things become real.

You'll open `CONTRIBUTORS.md`, add your name, and make your first contribution to the project.

**Next:** [Make Your First Change →](./08-make-your-first-change.md)

# Contributing

This is how we work with GitHub in this project. Please follow these steps every time.

## First time only

Clone the repository and go into the folder:

```bash
git clone https://github.com/BEH-77/Schola.git
cd Schola
```

## Before starting any change

Switch to `main` and make sure your local copy is up to date:

```bash
git checkout main
git pull
```

## Making a change

Never work directly on `main`. Create your own branch and work in it:

```bash
git switch -c yourname/short_description
```

Name your branch with your name, a slash, and a short description of the change. For example: `badr/add_login_page`.

Test your code on your computer before pushing it.

## Saving and pushing your work

```bash
git add .
git commit -m "Short description of what you changed"
git push -u origin yourname/short_description
```

The `-u` is only needed the first time you push a new branch. After that, `git push` is enough.

## Opening a pull request

1. Go to the repository on GitHub.
2. Click "Compare & pull request" for your branch.
3. Write a short description of what you changed and why.
4. Ask a teammate to review it.
5. Once it is approved, merge it into `main`.

## After your pull request is merged

Update your local copy so you have the latest code:

```bash
git checkout main
git pull
```

## Rules

- Always run `git pull` on `main` before creating a new branch.
- One branch per change, and keep branches small.
- Do not commit passwords, tokens, or `.env` files.
- If a push is rejected, run `git pull` and try again.
- If you get a merge conflict, ask for help before deleting anything.
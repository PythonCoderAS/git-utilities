# Git Utilities

These are small shell scripts I have created to make tedious git procedures not so terrible.

In order to include these scripts into your flow, add the `bin` directory to your `PATH` environment variable.

Shortcut: Any executable in `PATH` starting with `git-$name` can be called via `git $name`.

# Scripts

## git-autocommit

Small script that:

- Adds all files to be comitted

- Makes a commit using either the predefined message of `Updated` or a supplied message (which must be in quotes)

- Pushes the new commit

This script was intended to quickly deploy changes to heroku when using the git repo deploy method.

## git-full-restore

Small script to quickly remove all changes from a file and restore it to the last commit. This includes if the files are
staged or not.

## git-rebase-all

Script that will pull in the latest copy of `origin/master`, and then rebase all other local branches around
origin/master. It will abort a rebase if it encounters merge conflicts. This is very useful to rebase all branches upon
a merge occuring to the origin/master branch.
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
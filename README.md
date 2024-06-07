# git-helper
A collection of bash scripts that help speed up CLI git operations.
All scripts and installed in the /usr/bin folder 

## update-git
Running the `update-git` command in your terminal will push your current working directory to the server after adding new changes and prompting the user for a commit message. You can also just add the commit message after the command by encapsulating it in double quotes.

```bash
Example:

update-git "This is a commit message."
```

## pull-repo

Running the `pull-repo` command in your terminal will pull a specific repo of a prefixed group using the flag `-l` followed by the suffix name of the repo. You can change the prefix with the `-s` flag. By default the prefix is set to `ctos`.

The script will then search locations for the repo in some predetermined locations. This command can be run from any folder in the home user directory.

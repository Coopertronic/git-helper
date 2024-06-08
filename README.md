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

Running the `pull-repo` command in your terminal will pull a specific repo of a prefixed group using the flag `-n` followed by the suffix name of the repo. You can change the prefix with the `-s` flag. By default the prefix is set to `ctos`.

The script will then search locations for the repo in some predetermined locations. This command can be run from any folder in the home user directory.

```bash
Example:

pull-repo -n ctos-side-repo -s install
```

## update-repo

Running the `update-repo` command will commit a specific repo of a prefixed group using the flag `-n` followed by the suffix name of the repo. The commit message is added using the `-c` flag followed by you commit message in double quotes. You can change the prefix with the `-s` flag. By default the prefix is set to `ctos`.

The script will then search locations for the repo in some predetermined locations. This command can be run from any folder in the home user directory.

```bash
Example:

update-repo -n side-repo -s ctos -c "My commit message"
```

## clone-repo

Running the `clone-repo` command will clone a GitHub repo from a predefined author. The `-s` flag is used to switch to using `HTTPS` instead of the default `SSH`, this is useful if you are cloning something to use rather than something that you are developing. You should use the `-a` flag to tell the script the name of the author of the repo, by default this is set to `Coopertronic`.

The script will will search for the repo on GitHub and clone it to your current directory.

```bash
Example:

clone-repo -n git-helper -s -a Coopertronic
```

## clone-aur

Running the `clone-aur` command will simply clone a `PKGBUILD` from the `AUR` that is stated after the command.

```bash
Example:

clone-aur scummvm-git
```


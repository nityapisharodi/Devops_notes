## Quick notes on Git command lines

### Git Installation & Configuration

* git --version  : Checks if Git is already installed and what its version is.

* To install git, download the git installer for the respective OS. In case of mac:
        - Ensure that [Homebrew](https://brew.sh/) and [Xcode](https://developer.apple.com/xcode/) is installed.
        - You can also use a [binary installer](https://sourceforge.net/projects/git-osx-installer/) for git to avoid installing Homebrew or Xcode. 
          However since it is a third party app, mac can block the installation due to security check.
          
* $ git config.    : Enables to customise your git environment.
        - Setting Identity:
                  $ git config --global user.name "your name"
                  $ git config --global user.email your email address
        - Setting editor:
                  $ git config --global core.editor emacs / "code --wait" (for VS code)
        - Setting default branch name:
                  $ git config --global init.defaultBranch main
  
### Git basic command line actions

* $ git init <directory>.       : creates empty git repository
* $ git clone                   : makes a copy of an existing repository in GitHub.com to a local machine.
* $ git add  <directory>.       : Stage all changes in <directory> / <file> for next commit.
* $ git commit -m "message"     : Commit the change with appropriate message.
* $ git status                  : Lists the status of all the files (staged, unstaged or untracked)
* $ git remote add <name> <url> : Create a new connection to a remote repo.
* $ git branch                  : Lists all the branches in the repository
* $ git checkout                : Sets to work on a particular tree.
* $ git merge <branch>.         : Merge branch into the current/base or any other repository branch.
* $ git pull <remote>           : Fetch the copy of the current branch and merge it into the local copy.
* $ git push <remote> <branch>  : Push the branch commited in a local repository to <remote> along with necessary commits and objects.
* $ git log                     : Displays entire commit history

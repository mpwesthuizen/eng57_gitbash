# GitBash and GitHub README

This repo covers the following concepts/tools:
- Bash
- Git Bash
- Git Hub
- Issues and Troubleshooting

## Bash
Bash is a command line/shell language used in Linux terminals. It is also compatible with macOS (however Apple has replaced it with zsh as a default shell). Window's shell language is powershell.

_Note: macOS and linux distros share some similar functionality due to fact that the kernels/codebases have some similarities in structure. For a time macOS used bash and it worth noting that zsh, even as Apple attempts to move away from bash, is still similar to bash._
 
We can use it to create files, navigate our computer or run programs.

References:
- https://itsfoss.com/mac-linux-difference/

- https://www.gnu.org/software/bash/

- https://superuser.com/questions/806922/what-is-the-differences-between-ms-dos-powershell-in-windows

- https://www.theverge.com/2019/6/4/18651872/apple-macos-catalina-zsh-bash-shell-replacement-features

#### Basic Bash Commands
- ls : lists current directory
- rm : removes a file/directory
- .. : navigates back a folder
- cd : changes directory
- mkdir :creates new directory
- atom . :opens atom editor in folder
- code : opens vs code editor in folder
- -a : shows hidden files/folders


## Git
Git is a powerful version control used by developers globally and commonplace in industry.
It can go backwards in time and forwards.
It can also create separate branches (or universes) to allow us to experiment.

#### Basic GitBash Commands
- git init : Used to intialise a repo on the local machine. You should be in the directory to run this one.

- git status : This shows the tracked files on the machine and the status of the files IE. tracked, staged or committed.
 
- git log : Shows the commit history, master branches, and origin.

- git checkout master
- git checkout <commit hash>
- git remote -- v
- git diff
- git push origin master

- git commit -m '<Meaningful message>'

- git add <file>


References:
- https://itsfoss.com/mac-linux-difference/

- https://www.gnu.org/software/bash/

##Git Hub
description

creating repo's

ssh keys vs login

#### Pushing
where the local repo pushes up to the github repo.

- git push 
- git push <location>

#### Pulling
Where the github repo pulls from the local repo.

#### Cloning
Cloning is the way to copy a repo to your local folders you are go to start by going to the repo on github.com and hitting the clone button on the top right of the repo page then go to the terminal and accessing the directory you want to make your copy and run the git clone command with the copied repo https or ssh key.

command:
- git clone <repo>

#### Branching
Branching is used to allow collaborators to create seperate branches where developments can take place without conflicting with the master branch. This is useful as it means that the master branch can always contain working code that can still be in production whilst alterations (that break code) can be made seperately and then merged later when code is fully function. It helpful to think of the master branch as a Production environment and the branches as UAT environments.

##### Commands needed to create branch and add changes:

- git checkout remote -b <name of branch>
Note: when checking out of master into branch git will bring any pending stages and commits.

- git add and git commit
- git push origin <branch name>

#### Merging
Go to branched repo on github.com after committing a recent branch. Select the pull and merge request in project files, then fill out the commit messages and hit merge. This will merge new feature of the branch to the master branch so everyone can use it.

#### Forking
This is a github action that copies the whole repo to your account.


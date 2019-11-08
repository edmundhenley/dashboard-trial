```bash
# Set up a new project "dashboard-trial" on GitHub using GH's UI
# Chose a Python .gitignore, and an MIT licence 

# Setup for GitHub user account
(base) root@jupyter-edmundhenley:/home/jovyan# cd Edmund
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund# #git config --global user.name "[name]"
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund# #git config --global user.email "[email address]"
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund# git config --global color.ui auto

# Cloned project
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund# git clone https://github.com/edmundhenley/dashboard-trial.git
Cloning into 'dashboard-trial'...
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund# cd dashboard-trial/
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean

# Moved initial scripts into working copy
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# cd ..
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund# mkdir dashboard-trial/setup_reminders
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund# mv setup_reminders/* dashboard-trial/setup_reminders/
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund# rmdir setup_reminders/
rmdir: failed to remove 'setup_reminders/': Directory not empty
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund# ls -al setup_reminders/
total 12
drwxr-xr-x 3 root root 4096 Nov  8 16:45 .
drwxr-xr-x 5 root root 4096 Nov  8 16:39 ..
drwxr-xr-x 2 root root 4096 Nov  8 16:34 .ipynb_checkpoints
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund# rm setup_reminders/.ipynb_checkpoints/
rm: cannot remove 'setup_reminders/.ipynb_checkpoints/': Is a directory
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund# rm -rf setup_reminders/.ipynb_checkpoints/
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund# rmdir setup_reminders/
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund# mv Ed_dashboard_trial.ipynb dashboard-trial/Ed_dashboard-trial.ipynb

# Staged changes
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund# cd dashboard-trial/
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        Ed_dashboard-trial.ipynb
        setup_reminders/

nothing added to commit but untracked files present (use "git add" to track)
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git add -A
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   Ed_dashboard-trial.ipynb
        new file:   setup_reminders/conda_setup.txt
        new file:   setup_reminders/git_setup.txt

# Committed changes locally
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git commit
[master e0dece1] Add the initial notebook
 3 files changed, 314 insertions(+)
 create mode 100644 Ed_dashboard-trial.ipynb
 create mode 100644 setup_reminders/conda_setup.txt
 create mode 100644 setup_reminders/git_setup.txt
 
# Pushed changes up to master on GitHub
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git branch -v -a
* master                e0dece1 [ahead 1] Add the initial notebook
  remotes/origin/HEAD   -> origin/master
  remotes/origin/master e0e9504 Initial commit
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git push origin master
Username for 'https://github.com': edmundhenley
Password for 'https://edmundhenley@github.com': 
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 16 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 4.22 KiB | 1.05 MiB/s, done.
Total 6 (delta 0), reused 0 (delta 0)
To https://github.com/edmundhenley/dashboard-trial.git
   e0e9504..e0dece1  master -> master
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean

(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git status  # Made some changes
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   setup_reminders/git_setup.txt

no changes added to commit (use "git add" and/or "git commit -a")
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git difftool  # Made some changes

This message is displayed because 'diff.tool' is not configured.
See 'git difftool --tool-help' or 'git help config' for more details.
'git difftool' will now attempt to use one of the following tools:
kompare emerge vimdiff

Viewing (1/1): 'setup_reminders/git_setup.txt'
Launch 'vimdiff' [Y/n]? Y
2 files to edit

(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git add .
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   setup_reminders/git_setup.txt

(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git mv setup_reminders/conda_setup.txt setup_reminders/conda_setup.md
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git mv setup_reminders/git_setup.txt setup_reminders/git_setup.md
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        renamed:    setup_reminders/conda_setup.txt -> setup_reminders/conda_setup.md
        renamed:    setup_reminders/git_setup.txt -> setup_reminders/git_setup.md

(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git commit
[master c1c42fb] Change setup files to markdown format
 2 files changed, 0 insertions(+), 0 deletions(-)
 rename setup_reminders/{conda_setup.txt => conda_setup.md} (100%)
 rename setup_reminders/{git_setup.txt => git_setup.md} (100%)
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git push origin masterUsername for 'https://github.com': edmundhenley
Password for 'https://edmundhenley@github.com': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 449 bytes | 224.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/edmundhenley/dashboard-trial.git
   c6cc607..c1c42fb  master -> master

# Rename to markdown format, and push up
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git mv setup_reminders/conda_setup.txt setup_reminders/conda_setup.md
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git mv setup_reminders/git_setup.txt setup_reminders/git_setup.md
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        renamed:    setup_reminders/conda_setup.txt -> setup_reminders/conda_setup.md
        renamed:    setup_reminders/git_setup.txt -> setup_reminders/git_setup.md

(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git commit
[master c1c42fb] Change setup files to markdown format
 2 files changed, 0 insertions(+), 0 deletions(-)
 rename setup_reminders/{conda_setup.txt => conda_setup.md} (100%)
 rename setup_reminders/{git_setup.txt => git_setup.md} (100%)
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git push origin masterUsername for 'https://github.com': edmundhenley
Password for 'https://edmundhenley@github.com': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 449 bytes | 224.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/edmundhenley/dashboard-trial.git
   c6cc607..c1c42fb  master -> master

# Set up a develop branch, so I can use GitFlow: https://nvie.com/posts/a-successful-git-branching-model/
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git branch -v -a
* master                6b4b611 Use markdown in setup files
  remotes/origin/HEAD   -> origin/master
  remotes/origin/master 6b4b611 Use markdown in setup files
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean

(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git checkout -b develop
Switched to a new branch 'develop'
(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git branch -v -a
* develop               6b4b611 Use markdown in setup files
  master                6b4b611 Use markdown in setup files
  remotes/origin/HEAD   -> origin/master
  remotes/origin/master 6b4b611 Use markdown in setup files

(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git push --set-upstream origin develop
Username for 'https://github.com': edmundhenley
Password for 'https://edmundhenley@github.com': 
Total 0 (delta 0), reused 0 (delta 0)
remote: 
remote: Create a pull request for 'develop' on GitHub by visiting:
remote:      https://github.com/edmundhenley/dashboard-trial/pull/new/develop
remote: 
To https://github.com/edmundhenley/dashboard-trial.git
 * [new branch]      develop -> develop
Branch 'develop' set up to track remote branch 'develop' from 'origin'.

(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git branch -v -a
* develop                6b4b611 Use markdown in setup files
  master                 6b4b611 Use markdown in setup files
  remotes/origin/HEAD    -> origin/master
  remotes/origin/develop 6b4b611 Use markdown in setup files
  remotes/origin/master  6b4b611 Use markdown in setup files

(base) root@jupyter-edmundhenley:/home/jovyan/Edmund/dashboard-trial# git status
On branch develop
Your branch is up to date with 'origin/develop'.

nothing to commit, working tree clean


```

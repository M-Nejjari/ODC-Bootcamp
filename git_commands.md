Microsoft Windows [version 10.0.22631.4460]
(c) Microsoft Corporation. Tous droits réservés.

C:\Users\moham>echo "# ODC-Bootcamp" >> README.md

C:\Users\moham>git init
Reinitialized existing Git repository in C:/Users/moham/.git/

C:\Users\moham>git add read.me
fatal: pathspec 'read.me' did not match any files

C:\Users\moham>git add readme.md

C:\Users\moham>git commit -m "first commit"
[main 674ce59] first commit
 2 files changed, 10 insertions(+)
 create mode 100644 OneDrive/Bureau/S4/DSA/coRep/branchme.md
 create mode 100644 OneDrive/Bureau/S4/DSA/coRep/test.py

C:\Users\moham>git branch -m main

C:\Users\moham>git remote add origin https://github.com/M-Nejjari/ODC-Bootcamp.git
error: remote origin already exists.

C:\Users\moham>

C:\Users\moham>git remote -v
origin  https://github.com/M-Nejjari/ODC-branching.git (fetch)
origin  https://github.com/M-Nejjari/ODC-branching.git (push)
prod    https://github.com/M-Nejjari/prod.git (fetch)
prod    https://github.com/M-Nejjari/prod.git (push)

C:\Users\moham>git push -u origin main
To https://github.com/M-Nejjari/ODC-branching.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/M-Nejjari/ODC-branching.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

C:\Users\moham>git clone https://github.com/M-Nejjari/ODC-Bootcamp.git
Cloning into 'ODC-Bootcamp'...
warning: You appear to have cloned an empty repository.

C:\Users\moham>cd
C:\Users\moham

C:\Users\moham>cd ODC-Bootcamp

C:\Users\moham\ODC-Bootcamp>mkdir TASK1

C:\Users\moham\ODC-Bootcamp>echo "This is the tak one read me file" > TASK1/readme.md

C:\Users\moham\ODC-Bootcamp>git add TASK1/readme.md

C:\Users\moham\ODC-Bootcamp>git commit -m "adding the readme file after making the task1 folder"
[main (root-commit) e9a26ca] adding the readme file after making the task1 folder
 1 file changed, 1 insertion(+)
 create mode 100644 TASK1/readme.md

C:\Users\moham\ODC-Bootcamp>git push origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Writing objects: 100% (4/4), 315 bytes | 315.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/M-Nejjari/ODC-Bootcamp.git
 * [new branch]      main -> main

C:\Users\moham\ODC-Bootcamp>git checkout -b dev
Switched to a new branch 'dev'

C:\Users\moham\ODC-Bootcamp>nano test.txt
'nano' n’est pas reconnu en tant que commande interne
ou externe, un programme exécutable ou un fichier de commandes.

C:\Users\moham\ODC-Bootcamp>echo "tthis is a test " > test.tx

C:\Users\moham\ODC-Bootcamp>echo "this is a test" > test.txt

C:\Users\moham\ODC-Bootcamp>git add text.txt
fatal: pathspec 'text.txt' did not match any files

C:\Users\moham\ODC-Bootcamp>git add test.txt

C:\Users\moham\ODC-Bootcamp>git commit -m "this is a test branche"
[dev 9806ffb] this is a test branche
 1 file changed, 1 insertion(+)
 create mode 100644 test.txt

C:\Users\moham\ODC-Bootcamp>git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


C:\Users\moham\ODC-Bootcamp>git push --set-upstream origin dev
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 302 bytes | 302.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/M-Nejjari/ODC-Bootcamp/pull/new/dev
remote:
To https://github.com/M-Nejjari/ODC-Bootcamp.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

C:\Users\moham\ODC-Bootcamp>

C:\Users\moham\ODC-Bootcamp>git checkout -b Nejjari_new-feature
Switched to a new branch 'Nejjari_new-feature'

C:\Users\moham\ODC-Bootcamp>echo "this is the new feature read me file" > readme.md

C:\Users\moham\ODC-Bootcamp>git add
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Turn this message off by running
hint: "git config advice.addEmptyPathspec false"

C:\Users\moham\ODC-Bootcamp>git add readme.md

C:\Users\moham\ODC-Bootcamp>git commit -m "this is the new feature commit"
[Nejjari_new-feature 8b73aa6] this is the new feature commit
 1 file changed, 1 insertion(+)
 create mode 100644 readme.md

C:\Users\moham\ODC-Bootcamp>git push -u Nejjari_new-feature
fatal: 'Nejjari_new-feature' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

C:\Users\moham\ODC-Bootcamp>git push -u origin Nejjari_new-feature
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 361 bytes | 361.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'Nejjari_new-feature' on GitHub by visiting:
remote:      https://github.com/M-Nejjari/ODC-Bootcamp/pull/new/Nejjari_new-feature
remote:
To https://github.com/M-Nejjari/ODC-Bootcamp.git
 * [new branch]      Nejjari_new-feature -> Nejjari_new-feature
branch 'Nejjari_new-feature' set up to track 'origin/Nejjari_new-feature'.

C:\Users\moham\ODC-Bootcamp>git status
On branch Nejjari_new-feature
Your branch is up to date with 'origin/Nejjari_new-feature'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test.tx

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\moham\ODC-Bootcamp>echo ".*" > .gitignore

C:\Users\moham\ODC-Bootcamp>git add .gitignore

C:\Users\moham\ODC-Bootcamp>git push
Everything up-to-date

C:\Users\moham\ODC-Bootcamp>git commit
[Nejjari_new-feature 3882682] this is the git ignore configuration commit
 1 file changed, 1 insertion(+)
 create mode 100644 .gitignore

C:\Users\moham\ODC-Bootcamp>git status
On branch Nejjari_new-feature
Your branch is ahead of 'origin/Nejjari_new-feature' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test.tx

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\moham\ODC-Bootcamp>git status --ignored
On branch Nejjari_new-feature
Your branch is ahead of 'origin/Nejjari_new-feature' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test.tx

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\moham\ODC-Bootcamp>git oush
git: 'oush' is not a git command. See 'git --help'.

The most similar command is
        push

C:\Users\moham\ODC-Bootcamp>git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 373 bytes | 373.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/M-Nejjari/ODC-Bootcamp.git
   8b73aa6..3882682  Nejjari_new-feature -> Nejjari_new-feature

C:\Users\moham\ODC-Bootcamp>git push origin dev
Everything up-to-date

C:\Users\moham\ODC-Bootcamp>git checkout dev
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

C:\Users\moham\ODC-Bootcamp>git pull origin dev
From https://github.com/M-Nejjari/ODC-Bootcamp
 * branch            dev        -> FETCH_HEAD
Already up to date.

C:\Users\moham\ODC-Bootcamp>git merge Nejjari_new-feature
Updating 9806ffb..3882682
Fast-forward
 .gitignore | 1 +
 readme.md  | 1 +
 2 files changed, 2 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 readme.md

C:\Users\moham\ODC-Bootcamp>git commit
On branch dev
Your branch is ahead of 'origin/dev' by 2 commits.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test.tx

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\moham\ODC-Bootcamp>git push
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/M-Nejjari/ODC-Bootcamp.git
   9806ffb..3882682  dev -> dev

C:\Users\moham\ODC-Bootcamp>git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

C:\Users\moham\ODC-Bootcamp>git pull origin main
From https://github.com/M-Nejjari/ODC-Bootcamp
 * branch            main       -> FETCH_HEAD
Already up to date.

C:\Users\moham\ODC-Bootcamp>git merge dev
Updating e9a26ca..3882682
Fast-forward
 .gitignore | 1 +
 readme.md  | 1 +
 test.txt   | 1 +
 3 files changed, 3 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 readme.md
 create mode 100644 test.txt

C:\Users\moham\ODC-Bootcamp>git commit
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test.tx

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\moham\ODC-Bootcamp>git push
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/M-Nejjari/ODC-Bootcamp.git
   e9a26ca..3882682  main -> main

C:\Users\moham\ODC-Bootcamp>git checkout Nejjari_new-feature
Switched to branch 'Nejjari_new-feature'
Your branch is up to date with 'origin/Nejjari_new-feature'.

C:\Users\moham\ODC-Bootcamp>echo "this is new text added " > test.txt

C:\Users\moham\ODC-Bootcamp>git add test.txt

C:\Users\moham\ODC-Bootcamp>git commit test.txt
Aborting commit due to empty commit message.

C:\Users\moham\ODC-Bootcamp>git push
Everything up-to-date

C:\Users\moham\ODC-Bootcamp>git push origin Nejjari_new-feature
Everything up-to-date

C:\Users\moham\ODC-Bootcamp>notepad test.txt

C:\Users\moham\ODC-Bootcamp>git add test.txt

C:\Users\moham\ODC-Bootcamp>git commit
Aborting commit due to empty commit message.

C:\Users\moham\ODC-Bootcamp>git push
Everything up-to-date

C:\Users\moham\ODC-Bootcamp>git push origin Nejjari_new-feature
Everything up-to-date

C:\Users\moham\ODC-Bootcamp>echo "this is the second modification to the read me " >>readme.md

C:\Users\moham\ODC-Bootcamp>git add readme.md

C:\Users\moham\ODC-Bootcamp>git commit -m "modification to the read me file"
[Nejjari_new-feature 9d9804a] modification to the read me file
 2 files changed, 2 insertions(+), 1 deletion(-)

C:\Users\moham\ODC-Bootcamp>git push origin Nejjari_new--feature
error: src refspec Nejjari_new--feature does not match any
error: failed to push some refs to 'https://github.com/M-Nejjari/ODC-Bootcamp.git'

C:\Users\moham\ODC-Bootcamp>git push origin Nejjari_new-feature
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 460 bytes | 460.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/M-Nejjari/ODC-Bootcamp.git
   3882682..9d9804a  Nejjari_new-feature -> Nejjari_new-feature

C:\Users\moham\ODC-Bootcamp>git revert head
[Nejjari_new-feature 01ce105] Revert "modification to the read me file"
 2 files changed, 1 insertion(+), 2 deletions(-)

C:\Users\moham\ODC-Bootcamp>git push origin Nejjari_new-feature
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 453 bytes | 453.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/M-Nejjari/ODC-Bootcamp.git
   9d9804a..01ce105  Nejjari_new-feature -> Nejjari_new-feature

C:\Users\moham\ODC-Bootcamp>git log
commit 01ce105f0415f915240e0373dccb61daa305d1cd (HEAD -> Nejjari_new-feature, origin/Nejjari_new-feature)
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 11:56:42 2024 +0100

    Revert "modification to the read me file"

    This reverts commit 9d9804a7f342df9c98744ae865eb8974372233f5.

commit 9d9804a7f342df9c98744ae865eb8974372233f5
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 11:55:37 2024 +0100

    modification to the read me file

commit 3882682e71fe3d06db3b5d9a520e244d397b1c58 (origin/main, origin/dev, main, dev)
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 11:15:17 2024 +0100

    this is the git ignore configuration commit

commit 8b73aa66ba8e46dac3f3e8dd9ccb30c5966b6076
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 10:55:39 2024 +0100

    this is the new feature commit

commit 9806ffb8c38a21e7311bd777c9e7cb033c94b914
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 10:45:27 2024 +0100

    this is a test branche

commit e9a26ca4021fa6d87f0a5905c9178dd5fedec6df
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 10:35:02 2024 +0100

    adding the readme file after making the task1 folder

C:\Users\moham\ODC-Bootcamp>

C:\Users\moham\ODC-Bootcamp>nano log.txt
'nano' n’est pas reconnu en tant que commande interne
ou externe, un programme exécutable ou un fichier de commandes.

C:\Users\moham\ODC-Bootcamp>echo " " > og.txt

C:\Users\moham\ODC-Bootcamp>echo " " > log.txt

C:\Users\moham\ODC-Bootcamp>notepad log.txt

C:\Users\moham\ODC-Bootcamp>git add log.txt

C:\Users\moham\ODC-Bootcamp>git commit -m "adding log"
[Nejjari_new-feature 5aae4a6] adding log
 1 file changed, 37 insertions(+)
 create mode 100644 log.txt

C:\Users\moham\ODC-Bootcamp>git push origin main
Everything up-to-date

C:\Users\moham\ODC-Bootcamp>git --set-upstream origin main
unknown option: --set-upstream
usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--config-env=<name>=<envvar>] <command> [<args>]

C:\Users\moham\ODC-Bootcamp>git push -u origin main
Everything up-to-date
branch 'main' set up to track 'origin/main'.

C:\Users\moham\ODC-Bootcamp>git add log.txt

C:\Users\moham\ODC-Bootcamp>git commit -m "adding a log file"
On branch Nejjari_new-feature
Your branch is ahead of 'origin/Nejjari_new-feature' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        og.txt
        test.tx

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\moham\ODC-Bootcamp>git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 739 bytes | 739.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/M-Nejjari/ODC-Bootcamp.git
   01ce105..5aae4a6  Nejjari_new-feature -> Nejjari_new-feature

C:\Users\moham\ODC-Bootcamp>git log
commit 5aae4a6d31bb9afa657788fd13c1164e075e6a87 (HEAD -> Nejjari_new-feature, origin/Nejjari_new-feature)
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 12:03:22 2024 +0100

    adding log

commit 01ce105f0415f915240e0373dccb61daa305d1cd
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 11:56:42 2024 +0100

    Revert "modification to the read me file"

    This reverts commit 9d9804a7f342df9c98744ae865eb8974372233f5.

commit 9d9804a7f342df9c98744ae865eb8974372233f5
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 11:55:37 2024 +0100

    modification to the read me file

commit 3882682e71fe3d06db3b5d9a520e244d397b1c58 (origin/main, origin/dev, main, dev)
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 11:15:17 2024 +0100

    this is the git ignore configuration commit

commit 8b73aa66ba8e46dac3f3e8dd9ccb30c5966b6076
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 10:55:39 2024 +0100

    this is the new feature commit

commit 9806ffb8c38a21e7311bd777c9e7cb033c94b914
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 10:45:27 2024 +0100

    this is a test branche

commit e9a26ca4021fa6d87f0a5905c9178dd5fedec6df
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 10:35:02 2024 +0100

    adding the readme file after making the task1 folder

C:\Users\moham\ODC-Bootcamp>
C:\Users\moham\ODC-Bootcamp>git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

C:\Users\moham\ODC-Bootcamp>git pull origin main
From https://github.com/M-Nejjari/ODC-Bootcamp
 * branch            main       -> FETCH_HEAD
Already up to date.

C:\Users\moham\ODC-Bootcamp>git merge Nejjari_new-feature
Updating 3882682..5aae4a6
Fast-forward
 log.txt | 37 +++++++++++++++++++++++++++++++++++++
 1 file changed, 37 insertions(+)
 create mode 100644 log.txt

C:\Users\moham\ODC-Bootcamp>git branch -d Nejjari_new-feature
Deleted branch Nejjari_new-feature (was 5aae4a6).

C:\Users\moham\ODC-Bootcamp>git push origin --delete Nejjari_new-feature
To https://github.com/M-Nejjari/ODC-Bootcamp.git
 - [deleted]         Nejjari_new-feature

C:\Users\moham\ODC-Bootcamp>Microsoft Windows [version 10.0.22631.4460]
(c) Microsoft Corporation. Tous droits réservés.

C:\Users\moham>echo "# ODC-Bootcamp" >> README.md

C:\Users\moham>git init
Reinitialized existing Git repository in C:/Users/moham/.git/

C:\Users\moham>git add read.me
fatal: pathspec 'read.me' did not match any files

C:\Users\moham>git add readme.md

C:\Users\moham>git commit -m "first commit"
[main 674ce59] first commit
 2 files changed, 10 insertions(+)
 create mode 100644 OneDrive/Bureau/S4/DSA/coRep/branchme.md
 create mode 100644 OneDrive/Bureau/S4/DSA/coRep/test.py

C:\Users\moham>git branch -m main

C:\Users\moham>git remote add origin https://github.com/M-Nejjari/ODC-Bootcamp.git
error: remote origin already exists.

C:\Users\moham>

C:\Users\moham>git remote -v
origin  https://github.com/M-Nejjari/ODC-branching.git (fetch)
origin  https://github.com/M-Nejjari/ODC-branching.git (push)
prod    https://github.com/M-Nejjari/prod.git (fetch)
prod    https://github.com/M-Nejjari/prod.git (push)

C:\Users\moham>git push -u origin main
To https://github.com/M-Nejjari/ODC-branching.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/M-Nejjari/ODC-branching.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

C:\Users\moham>git clone https://github.com/M-Nejjari/ODC-Bootcamp.git
Cloning into 'ODC-Bootcamp'...
warning: You appear to have cloned an empty repository.

C:\Users\moham>cd
C:\Users\moham

C:\Users\moham>cd ODC-Bootcamp

C:\Users\moham\ODC-Bootcamp>mkdir TASK1

C:\Users\moham\ODC-Bootcamp>echo "This is the tak one read me file" > TASK1/readme.md

C:\Users\moham\ODC-Bootcamp>git add TASK1/readme.md

C:\Users\moham\ODC-Bootcamp>git commit -m "adding the readme file after making the task1 folder"
[main (root-commit) e9a26ca] adding the readme file after making the task1 folder
 1 file changed, 1 insertion(+)
 create mode 100644 TASK1/readme.md

C:\Users\moham\ODC-Bootcamp>git push origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Writing objects: 100% (4/4), 315 bytes | 315.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/M-Nejjari/ODC-Bootcamp.git
 * [new branch]      main -> main

C:\Users\moham\ODC-Bootcamp>git checkout -b dev
Switched to a new branch 'dev'

C:\Users\moham\ODC-Bootcamp>nano test.txt
'nano' n’est pas reconnu en tant que commande interne
ou externe, un programme exécutable ou un fichier de commandes.

C:\Users\moham\ODC-Bootcamp>echo "tthis is a test " > test.tx

C:\Users\moham\ODC-Bootcamp>echo "this is a test" > test.txt

C:\Users\moham\ODC-Bootcamp>git add text.txt
fatal: pathspec 'text.txt' did not match any files

C:\Users\moham\ODC-Bootcamp>git add test.txt

C:\Users\moham\ODC-Bootcamp>git commit -m "this is a test branche"
[dev 9806ffb] this is a test branche
 1 file changed, 1 insertion(+)
 create mode 100644 test.txt

C:\Users\moham\ODC-Bootcamp>git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


C:\Users\moham\ODC-Bootcamp>git push --set-upstream origin dev
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 302 bytes | 302.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/M-Nejjari/ODC-Bootcamp/pull/new/dev
remote:
To https://github.com/M-Nejjari/ODC-Bootcamp.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

C:\Users\moham\ODC-Bootcamp>

C:\Users\moham\ODC-Bootcamp>git checkout -b Nejjari_new-feature
Switched to a new branch 'Nejjari_new-feature'

C:\Users\moham\ODC-Bootcamp>echo "this is the new feature read me file" > readme.md

C:\Users\moham\ODC-Bootcamp>git add
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Turn this message off by running
hint: "git config advice.addEmptyPathspec false"

C:\Users\moham\ODC-Bootcamp>git add readme.md

C:\Users\moham\ODC-Bootcamp>git commit -m "this is the new feature commit"
[Nejjari_new-feature 8b73aa6] this is the new feature commit
 1 file changed, 1 insertion(+)
 create mode 100644 readme.md

C:\Users\moham\ODC-Bootcamp>git push -u Nejjari_new-feature
fatal: 'Nejjari_new-feature' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

C:\Users\moham\ODC-Bootcamp>git push -u origin Nejjari_new-feature
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 361 bytes | 361.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'Nejjari_new-feature' on GitHub by visiting:
remote:      https://github.com/M-Nejjari/ODC-Bootcamp/pull/new/Nejjari_new-feature
remote:
To https://github.com/M-Nejjari/ODC-Bootcamp.git
 * [new branch]      Nejjari_new-feature -> Nejjari_new-feature
branch 'Nejjari_new-feature' set up to track 'origin/Nejjari_new-feature'.

C:\Users\moham\ODC-Bootcamp>git status
On branch Nejjari_new-feature
Your branch is up to date with 'origin/Nejjari_new-feature'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test.tx

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\moham\ODC-Bootcamp>echo ".*" > .gitignore

C:\Users\moham\ODC-Bootcamp>git add .gitignore

C:\Users\moham\ODC-Bootcamp>git push
Everything up-to-date

C:\Users\moham\ODC-Bootcamp>git commit
[Nejjari_new-feature 3882682] this is the git ignore configuration commit
 1 file changed, 1 insertion(+)
 create mode 100644 .gitignore

C:\Users\moham\ODC-Bootcamp>git status
On branch Nejjari_new-feature
Your branch is ahead of 'origin/Nejjari_new-feature' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test.tx

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\moham\ODC-Bootcamp>git status --ignored
On branch Nejjari_new-feature
Your branch is ahead of 'origin/Nejjari_new-feature' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test.tx

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\moham\ODC-Bootcamp>git oush
git: 'oush' is not a git command. See 'git --help'.

The most similar command is
        push

C:\Users\moham\ODC-Bootcamp>git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 373 bytes | 373.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/M-Nejjari/ODC-Bootcamp.git
   8b73aa6..3882682  Nejjari_new-feature -> Nejjari_new-feature

C:\Users\moham\ODC-Bootcamp>git push origin dev
Everything up-to-date

C:\Users\moham\ODC-Bootcamp>git checkout dev
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

C:\Users\moham\ODC-Bootcamp>git pull origin dev
From https://github.com/M-Nejjari/ODC-Bootcamp
 * branch            dev        -> FETCH_HEAD
Already up to date.

C:\Users\moham\ODC-Bootcamp>git merge Nejjari_new-feature
Updating 9806ffb..3882682
Fast-forward
 .gitignore | 1 +
 readme.md  | 1 +
 2 files changed, 2 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 readme.md

C:\Users\moham\ODC-Bootcamp>git commit
On branch dev
Your branch is ahead of 'origin/dev' by 2 commits.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test.tx

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\moham\ODC-Bootcamp>git push
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/M-Nejjari/ODC-Bootcamp.git
   9806ffb..3882682  dev -> dev

C:\Users\moham\ODC-Bootcamp>git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

C:\Users\moham\ODC-Bootcamp>git pull origin main
From https://github.com/M-Nejjari/ODC-Bootcamp
 * branch            main       -> FETCH_HEAD
Already up to date.

C:\Users\moham\ODC-Bootcamp>git merge dev
Updating e9a26ca..3882682
Fast-forward
 .gitignore | 1 +
 readme.md  | 1 +
 test.txt   | 1 +
 3 files changed, 3 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 readme.md
 create mode 100644 test.txt

C:\Users\moham\ODC-Bootcamp>git commit
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test.tx

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\moham\ODC-Bootcamp>git push
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/M-Nejjari/ODC-Bootcamp.git
   e9a26ca..3882682  main -> main

C:\Users\moham\ODC-Bootcamp>git checkout Nejjari_new-feature
Switched to branch 'Nejjari_new-feature'
Your branch is up to date with 'origin/Nejjari_new-feature'.

C:\Users\moham\ODC-Bootcamp>echo "this is new text added " > test.txt

C:\Users\moham\ODC-Bootcamp>git add test.txt

C:\Users\moham\ODC-Bootcamp>git commit test.txt
Aborting commit due to empty commit message.

C:\Users\moham\ODC-Bootcamp>git push
Everything up-to-date

C:\Users\moham\ODC-Bootcamp>git push origin Nejjari_new-feature
Everything up-to-date

C:\Users\moham\ODC-Bootcamp>notepad test.txt

C:\Users\moham\ODC-Bootcamp>git add test.txt

C:\Users\moham\ODC-Bootcamp>git commit
Aborting commit due to empty commit message.

C:\Users\moham\ODC-Bootcamp>git push
Everything up-to-date

C:\Users\moham\ODC-Bootcamp>git push origin Nejjari_new-feature
Everything up-to-date

C:\Users\moham\ODC-Bootcamp>echo "this is the second modification to the read me " >>readme.md

C:\Users\moham\ODC-Bootcamp>git add readme.md

C:\Users\moham\ODC-Bootcamp>git commit -m "modification to the read me file"
[Nejjari_new-feature 9d9804a] modification to the read me file
 2 files changed, 2 insertions(+), 1 deletion(-)

C:\Users\moham\ODC-Bootcamp>git push origin Nejjari_new--feature
error: src refspec Nejjari_new--feature does not match any
error: failed to push some refs to 'https://github.com/M-Nejjari/ODC-Bootcamp.git'

C:\Users\moham\ODC-Bootcamp>git push origin Nejjari_new-feature
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 460 bytes | 460.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/M-Nejjari/ODC-Bootcamp.git
   3882682..9d9804a  Nejjari_new-feature -> Nejjari_new-feature

C:\Users\moham\ODC-Bootcamp>git revert head
[Nejjari_new-feature 01ce105] Revert "modification to the read me file"
 2 files changed, 1 insertion(+), 2 deletions(-)

C:\Users\moham\ODC-Bootcamp>git push origin Nejjari_new-feature
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 453 bytes | 453.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/M-Nejjari/ODC-Bootcamp.git
   9d9804a..01ce105  Nejjari_new-feature -> Nejjari_new-feature

C:\Users\moham\ODC-Bootcamp>git log
commit 01ce105f0415f915240e0373dccb61daa305d1cd (HEAD -> Nejjari_new-feature, origin/Nejjari_new-feature)
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 11:56:42 2024 +0100

    Revert "modification to the read me file"

    This reverts commit 9d9804a7f342df9c98744ae865eb8974372233f5.

commit 9d9804a7f342df9c98744ae865eb8974372233f5
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 11:55:37 2024 +0100

    modification to the read me file

commit 3882682e71fe3d06db3b5d9a520e244d397b1c58 (origin/main, origin/dev, main, dev)
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 11:15:17 2024 +0100

    this is the git ignore configuration commit

commit 8b73aa66ba8e46dac3f3e8dd9ccb30c5966b6076
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 10:55:39 2024 +0100

    this is the new feature commit

commit 9806ffb8c38a21e7311bd777c9e7cb033c94b914
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 10:45:27 2024 +0100

    this is a test branche

commit e9a26ca4021fa6d87f0a5905c9178dd5fedec6df
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 10:35:02 2024 +0100

    adding the readme file after making the task1 folder

C:\Users\moham\ODC-Bootcamp>

C:\Users\moham\ODC-Bootcamp>nano log.txt
'nano' n’est pas reconnu en tant que commande interne
ou externe, un programme exécutable ou un fichier de commandes.

C:\Users\moham\ODC-Bootcamp>echo " " > og.txt

C:\Users\moham\ODC-Bootcamp>echo " " > log.txt

C:\Users\moham\ODC-Bootcamp>notepad log.txt

C:\Users\moham\ODC-Bootcamp>git add log.txt

C:\Users\moham\ODC-Bootcamp>git commit -m "adding log"
[Nejjari_new-feature 5aae4a6] adding log
 1 file changed, 37 insertions(+)
 create mode 100644 log.txt

C:\Users\moham\ODC-Bootcamp>git push origin main
Everything up-to-date

C:\Users\moham\ODC-Bootcamp>git --set-upstream origin main
unknown option: --set-upstream
usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--config-env=<name>=<envvar>] <command> [<args>]

C:\Users\moham\ODC-Bootcamp>git push -u origin main
Everything up-to-date
branch 'main' set up to track 'origin/main'.

C:\Users\moham\ODC-Bootcamp>git add log.txt

C:\Users\moham\ODC-Bootcamp>git commit -m "adding a log file"
On branch Nejjari_new-feature
Your branch is ahead of 'origin/Nejjari_new-feature' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        og.txt
        test.tx

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\moham\ODC-Bootcamp>git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 739 bytes | 739.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/M-Nejjari/ODC-Bootcamp.git
   01ce105..5aae4a6  Nejjari_new-feature -> Nejjari_new-feature

C:\Users\moham\ODC-Bootcamp>git log
commit 5aae4a6d31bb9afa657788fd13c1164e075e6a87 (HEAD -> Nejjari_new-feature, origin/Nejjari_new-feature)
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 12:03:22 2024 +0100

    adding log

commit 01ce105f0415f915240e0373dccb61daa305d1cd
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 11:56:42 2024 +0100

    Revert "modification to the read me file"

    This reverts commit 9d9804a7f342df9c98744ae865eb8974372233f5.

commit 9d9804a7f342df9c98744ae865eb8974372233f5
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 11:55:37 2024 +0100

    modification to the read me file

commit 3882682e71fe3d06db3b5d9a520e244d397b1c58 (origin/main, origin/dev, main, dev)
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 11:15:17 2024 +0100

    this is the git ignore configuration commit

commit 8b73aa66ba8e46dac3f3e8dd9ccb30c5966b6076
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 10:55:39 2024 +0100

    this is the new feature commit

commit 9806ffb8c38a21e7311bd777c9e7cb033c94b914
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 10:45:27 2024 +0100

    this is a test branche

commit e9a26ca4021fa6d87f0a5905c9178dd5fedec6df
Author: M-nejjari <nejjari_mohamed@outlook.com>
Date:   Wed Nov 20 10:35:02 2024 +0100

    adding the readme file after making the task1 folder

C:\Users\moham\ODC-Bootcamp>
C:\Users\moham\ODC-Bootcamp>git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

C:\Users\moham\ODC-Bootcamp>git pull origin main
From https://github.com/M-Nejjari/ODC-Bootcamp
 * branch            main       -> FETCH_HEAD
Already up to date.

C:\Users\moham\ODC-Bootcamp>git merge Nejjari_new-feature
Updating 3882682..5aae4a6
Fast-forward
 log.txt | 37 +++++++++++++++++++++++++++++++++++++
 1 file changed, 37 insertions(+)
 create mode 100644 log.txt

C:\Users\moham\ODC-Bootcamp>git branch -d Nejjari_new-feature
Deleted branch Nejjari_new-feature (was 5aae4a6).

C:\Users\moham\ODC-Bootcamp>git push origin --delete Nejjari_new-feature
To https://github.com/M-Nejjari/ODC-Bootcamp.git
 - [deleted]         Nejjari_new-feature

C:\Users\moham\ODC-Bootcamp>
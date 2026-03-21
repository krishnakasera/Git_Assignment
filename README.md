# Git_Assignment
Microsoft Windows [Version 10.0.26200.7840]
(c) Microsoft Corporation. All rights reserved.

C:\Users\krish\OneDrive\Desktop\git-project>git init
Reinitialized existing Git repository in C:/Users/krish/OneDrive/Desktop/git-project/.git/

C:\Users\krish\OneDrive\Desktop\git-project>git commit m-"my first repo "
error: pathspec 'm-my first repo ' did not match any file(s) known to git

C:\Users\krish\OneDrive\Desktop\git-project>git commit -m " my first repo"
[master (root-commit) b539c72]  my first repo
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 index.txt

C:\Users\krish\OneDrive\Desktop\git-project>git add .

C:\Users\krish\OneDrive\Desktop\git-project> git branch feature

C:\Users\krish\OneDrive\Desktop\git-project>git checkot feature
git: 'checkot' is not a git command. See 'git --help'.

The most similar command is
        checkout

C:\Users\krish\OneDrive\Desktop\git-project>git checkout feature
D       index.txt
Switched to branch 'feature'

C:\Users\krish\OneDrive\Desktop\git-project>git branch
* feature
  master

C:\Users\krish\OneDrive\Desktop\git-project>git branch main

C:\Users\krish\OneDrive\Desktop\git-project>git branch
* feature
  main
  master

C:\Users\krish\OneDrive\Desktop\git-project>git add .

C:\Users\krish\OneDrive\Desktop\git-project>git commit -m "my changes"
[feature 1de5d4b] my changes
 2 files changed, 1 insertion(+)
 create mode 100644 demo.txt
 delete mode 100644 index.txt

C:\Users\krish\OneDrive\Desktop\git-project>git checkout main 
Switched to branch 'main'

C:\Users\krish\OneDrive\Desktop\git-project>git pull origin main
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

C:\Users\krish\OneDrive\Desktop\git-project>git pull origin main
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

C:\Users\krish\OneDrive\Desktop\git-project>  

C:\Users\krish\OneDrive\Desktop\git-project>git remote -v

C:\Users\krish\OneDrive\Desktop\git-project>git remote add origin https://github.com/krishnakasera/Git_Assignment.git

C:\Users\krish\OneDrive\Desktop\git-project>git remote -v
origin  https://github.com/krishnakasera/Git_Assignment.git (fetch)
origin  https://github.com/krishnakasera/Git_Assignment.git (push)

C:\Users\krish\OneDrive\Desktop\git-project>git pull origin main
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 7 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (7/7), 2.54 KiB | 99.00 KiB/s, done.
From https://github.com/krishnakasera/Git_Assignment
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
fatal: refusing to merge unrelated histories

C:\Users\krish\OneDrive\Desktop\git-project>merge branch feature
'merge' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\krish\OneDrive\Desktop\git-project>git merge branch feature
merge: branch - not something we can merge

C:\Users\krish\OneDrive\Desktop\git-project>git add .

C:\Users\krish\OneDrive\Desktop\git-project>git commit -m "Resolved merge conflict"
On branch main
nothing to commit, working tree clean

C:\Users\krish\OneDrive\Desktop\git-project>git branch
  feature
* main
  master

C:\Users\krish\OneDrive\Desktop\git-project>git checkout feature
Switched to branch 'feature'

C:\Users\krish\OneDrive\Desktop\git-project>git branch
* feature
  main
  master

C:\Users\krish\OneDrive\Desktop\git-project>git checkout main
Switched to branch 'main'

C:\Users\krish\OneDrive\Desktop\git-project>git pull origin main
From https://github.com/krishnakasera/Git_Assignment
 * branch            main       -> FETCH_HEAD
fatal: refusing to merge unrelated histories

C:\Users\krish\OneDrive\Desktop\git-project>git pull origin main --allow-unrelated-histories      
From https://github.com/krishnakasera/Git_Assignment
 * branch            main       -> FETCH_HEAD
Merge made by the 'ort' strategy.
 README.md | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

C:\Users\krish\OneDrive\Desktop\git-project>git push origin main
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (5/5), 538 bytes | 538.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/krishnakasera/Git_Assignment.git
   3c744ba..d02da25  main -> main

C:\Users\krish\OneDrive\Desktop\git-project>git merge feature
error: The following untracked working tree files would be overwritten by merge:
        demo.txt
Please move or remove them before you merge.
Aborting
Merge with strategy ort failed.

C:\Users\krish\OneDrive\Desktop\git-project>git add demo.txt

C:\Users\krish\OneDrive\Desktop\git-project>git commit -m "Save local file before merge"
[main f076aaf] Save local file before merge
 1 file changed, 1 insertion(+)
 create mode 100644 demo.txt

C:\Users\krish\OneDrive\Desktop\git-project>git merge feature
Merge made by the 'ort' strategy.
 index.txt | 0
 1 file changed, 0 insertions(+), 0 deletions(-)
 delete mode 100644 index.txt

C:\Users\krish\OneDrive\Desktop\git-project>git branch
  feature
* main
  master

C:\Users\krish\OneDrive\Desktop\git-project>git checkout main
Already on 'main'

C:\Users\krish\OneDrive\Desktop\git-project>git checkout feature
Switched to branch 'feature'

C:\Users\krish\OneDrive\Desktop\git-project>git branch
* feature
  main
  master

C:\Users\krish\OneDrive\Desktop\git-project>git checkout main
Switched to branch 'main'

C:\Users\krish\OneDrive\Desktop\git-project>git pull origin main
From https://github.com/krishnakasera/Git_Assignment
 * branch            main       -> FETCH_HEAD
Already up to date.

C:\Users\krish\OneDrive\Desktop\git-project>git merge feature --no-edit
Already up to date.

C:\Users\krish\OneDrive\Desktop\git-project>git push origin main
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (7/7), 766 bytes | 383.00 KiB/s, done.
Total 7 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/krishnakasera/Git_Assignment.git
   d02da25..b412683  main -> main

C:\Users\krish\OneDrive\Desktop\git-project>git log --oneline --graph
*   b412683 (HEAD -> main, origin/main) Merge branch 'feature'
|\
| * 1de5d4b (feature) my changes
* | f076aaf Save local file before merge
* |   d02da25 Merge branch 'main' of https://github.com/krishnakasera/Git_Assignment
|\ \
| |/
|/|
| * 3c744ba Delete File.txt
| * 921e196 Create File.txt
| * 5769b77 Initial commit
:...skipping...
*   b412683 (HEAD -> main, origin/main) Merge branch 'feature'
|\
| * 1de5d4b (feature) my changes
* | f076aaf Save local file before merge
* |   d02da25 Merge branch 'main' of https://github.com/krishnakasera/Git_Assignment
|\ \
| |/
|/|
| * 3c744ba Delete File.txt
| * 921e196 Create File.txt
| * 5769b77 Initial commit
* b539c72 (master)  my first repo
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
(END)
*   b412683 (HEAD -> main, origin/main) Merge branch 'feature'
|\
| * 1de5d4b (feature) my changes
* | f076aaf Save local file before merge
* |   d02da25 Merge branch 'main' of https://github.com/krishnakasera/Git_Assignment
|\ \
| |/
|/|
| * 3c744ba Delete File.txt
| * 921e196 Create File.txt
| * 5769b77 Initial commit
* b539c72 (master)  my first repo
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
(END)
*   b412683 (HEAD -> main, origin/main) Merge branch 'feature'
|\
| * 1de5d4b (feature) my changes
* | f076aaf Save local file before merge
* |   d02da25 Merge branch 'main' of https://github.com/krishnakasera/Git_Assignment
|\ \
| |/
|/|
| * 3c744ba Delete File.txt
| * 921e196 Create File.txt
| * 5769b77 Initial commit
:
*   b412683 (HEAD -> main, origin/main) Merge branch 'feature'
|\
| * 1de5d4b (feature) my changes
* | f076aaf Save local file before merge
* |   d02da25 Merge branch 'main' of https://github.com/krishnakasera/Git_Assignment
|\ \
| |/
|/|
| * 3c744ba Delete File.txt
| * 921e196 Create File.txt
| * 5769b77 Initial commit
* b539c72 (master)  my first repo
~
~
| * 3c744ba Delete File.txt
| * 921e196 Create File.txt
| * 5769b77 Initial commit
* b539c72 (master)  my first repo
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
(END)
*   b412683 (HEAD -> main, origin/main) Merge branch 'feature'
|\
| *





    1de5d4b (feature) my changes
* | f076aaf Save local file before merge
* |   d02da25 Merge branch 'main' of https://github.com/krishnakasera/Git_Assignment
|\ \  
*   b412683 (HEAD -> main, origin/main) Merge branch 'feature'
|\
| * 1de5d4b (feature) my changes
* | f076aaf Save local file before merge
* |   d02da25 Merge branch 'main' of https://github.com/krishnakasera/Git_Assignment
|\ \
| |/
|/|
| * 3c744ba Delete File.txt
| * 921e196 Create File.txt
| * 5769b77 Initial commit
* b539c72 (master)  my first repo
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
(END)
*   b412683 (





             HEAD -> main, origin/main) Merge branch 'feature'
|\  
| * 1de5d4b (feature) my changes
* | f076aaf Save local file before merge
* |   d02da25 Merge branch 'main' of https://github.com/krishnakasera/Git_Assignment
|\ \  
| |/
|/|
| * 3c744ba Delete File.txt
| * 921e196 Create File.txt
| * 5769b77 Initial commit
* b539c72 (master)  my first repo
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
(END)
*   b412683 (HEAD -> main, origin/main) Merge branch 'feature'
|\
| * 1de5d4b (feature) my changes
* | f076aaf Save local file before merge
* |   d02da25 Merge branch 'main' of https://github.com/krishnakasera/Git_Assignment
|\ \
| |/
|/|
| * 3c744ba Delete File.txt
| * 921e196 Create File.txt
| * 5769b77 Initial commit
* b539c72 (master)  my first repo
~
~
~
~
~
~
~
~
~
~
~
~
(END)
*   b412683 (HEAD -> main, origin/main) Merge branch 'feature'
|\
| * 1de5d4b (feature) my changes
* | f076aaf Save local file before merge
* |   d02da25 Merge branch 'main' of https://github.com/krishnakasera/Git_Assignment
|\ \
| |/
|/|
| * 3c744ba Delete File.txt
| * 921e196 Create File.txt
| * 5769b77 Initial commit
* b539c72 (master)  my first repo
~
~
~
~
~
~
~
~
~
~
~
*   b412683 (HEAD -> main, origin/main) Merge branch 'feature'
|\
| * 1de5d4b (feature) my changes
* | f076aaf Save local file before merge
* |   d02da25 Merge branch 'main' of https://github.com/krishnakasera/Git_Assignment
|\ \
| |/
|/|
| * 3c744ba Delete File.txt
| * 921e196 Create File.txt
| * 5769b77 Initial commit
* b539c72 (master)  my first repo
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
(END)
*   b412683 (HEAD -> main, origin/main) Merge branch 'feature'
|\
| * 1de5d4b (feature) my changes
* | f076aaf Save local file before merge
* |   d02da25 Merge branch 'main' of https://github.com/krishnakasera/Git_Assignment
|\ \  
| |/  
|/|   
| * 3c744ba Delete File.txt
| * 921e196 Create File.txt
| * 5769b77 Initial commit
* b539c72 (master)  my first repo
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
(END)

# GIT EXERCISES

## Buddle 1

### Exercise 1

```bash
   AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/Gym-Git-Exercise-Solutions (main)
$ ls
README.md

AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/Gym-Git-Exercise-Solutions (main)
$ git add .

AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/Gym-Git-Exercise-Solutions (main)
$ ls
README.md

AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/Gym-Git-Exercise-Solutions (main)
$ git status
On branch main


AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/Gym-Git-Exercise-Solutions (main)

AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/Gym-Git-Exercise-Solutions/nelson_at_TG (main)
$ ls

AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/Gym-Git-Exercise-Solutions/nelson_at_TG (main)
$ cd ..

AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/nelson_at_TG (master)
$ ls

AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/nelson_at_TG (master)
$ git branch -m main

AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/nelson_at_TG (main)
$ code day1.txt

AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/nelson_at_TG (main)

Date:   Tue Jul 11 11:25:52 2023 +0200

    Commit 1

AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/nelson_at_TG (main)
(main)
$ git remote add origin https://github.com/NelHim/the_gym.git
                                                                      (main)
AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/nelson_at_TG
(main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 257 bytes | 128.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/NelHim/the_gym.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.                          (main)

AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/nelson_at_TG
(main)                                                                (main)
$ git branch dev

AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/nelson_at_TG
(main)
(main)
$ git checkout dev
Switched to branch 'dev'

AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/nelson_at_TG (dev)
$ git branch test

AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/nelson_at_TG (dev)
$ git checkout test
Switched to branch 'test'

AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/nelson_at_TG (test)
$ git checkout dev
Switched to branch 'dev'

AMAZON@DESKTOP-HHT6NIQ MINGW64 ~/Desktop/The Gym Program/nelson_at_TG (dev)
$ git branch -d test
Deleted branch test (was c69ab60).
```



### Exercise 2


```bash
User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ code home.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git add .

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git stash
Saved working directory and index state WIP on main: 454e14f Excercise 1

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ code about.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git add .

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git stash
Saved working directory and index state WIP on main: 454e14f Excercise 1

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git stash list
stash@{0}: WIP on main: 454e14f Excercise 1
stash@{1}: WIP on main: 454e14f Excercise 1

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ code team.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git add .

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git stash
Saved working directory and index state WIP on main: 454e14f Excercise 1

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git stash list
stash@{0}: WIP on main: 454e14f Excercise 1
stash@{1}: WIP on main: 454e14f Excercise 1
stash@{2}: WIP on main: 454e14f Excercise 1

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (b6cf1cd25571b36dac7ff74bbbe6d28d10a1a34c)

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git stash pop stash@{2}
fatal: log for 'stash' only has 2 entries

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git stash list
stash@{0}: WIP on main: 454e14f Excercise 1
stash@{1}: WIP on main: 454e14f Excercise 1

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (e8fa90b26c74fdfd9114342bb65f1627caee4009)      

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html


User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git add .

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git commit -m "unstashed files"
[main d6be1f3] unstashed files
 2 files changed, 22 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 512 bytes | 512.00 KiB/s, done.      
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
To https://github.com/NelHim/Gym-Git-Exercise-Solutions.git
   454e14f..d6be1f3  main -> main

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git stash list
stash@{0}: WIP on main: 454e14f Excercise 1

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git stash pop stash@{0}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (4cdb949ec46fa726ddfe17d6c431d3f563b6e08c)      

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git reset

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git status

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ ls
about.html  home.html  README.md  team.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ code README.md

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$
```


## Bundle 2

### Exercise 1

```bash
User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ ls
about.html  home.html  README.md  team.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ code services.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git status
On branch ft/bundle-2
Untracked files:
  (use "git add <file>..." to include in what will be committed)  
        services.html
        team.html

nothing added to commit but untracked files present (use "git add" to track)

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git add services.html 

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git status
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   services.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)  
        team.html


User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git commit -m "Created services file"
[ft/bundle-2 8ec20cc] Created services file
 1 file changed, 11 insertions(+)
 create mode 100644 services.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use    

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking 
upstream, see 'push.autoSetupRemote' in 'git help config'.        


User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git push origin ft/bundle-2 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 437 bytes | 437.00 KiB/s, done.      
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/NelHim/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/NelHim/Gym-Git-Exercise-Solutions.git       
 * [new branch]      ft/bundle-2 -> ft/bundle-2

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/bundle-2)
$

```

### Exercise 2

```bash 
User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git pull
Already up to date.

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git checkout -b ft/servie-redesign
Switched to a new branch 'ft/servie-redesign'

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/servie-redesign)
$ code services.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/servie-redesign)
$ git status
On branch ft/servie-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)      
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a") 

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/servie-redesign)
$ git add .

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/servie-redesign)
$ git commit -m "Update services"
[ft/servie-redesign f7a7b51] Update services
 1 file changed, 1 insertion(+)

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/servie-redesign)
$ git push origin ft/servie-redesign 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 337 bytes | 337.00 KiB/s, done.      
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/servie-redesign' on GitHub by visiting:
remote:      https://github.com/NelHim/Gym-Git-Exercise-Solutions/pull/new/ft/servie-redesign
remote:
To https://github.com/NelHim/Gym-Git-Exercise-Solutions.git       
 * [new branch]      ft/servie-redesign -> ft/servie-redesign     

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/servie-redesign)
$ git branch
  dev
  ft/bundle-2

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git push origin ft/service-redesign 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 337 bytes | 337.00 KiB/s, done.      
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/NelHim/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote:
To https://github.com/NelHim/Gym-Git-Exercise-Solutions.git       
 * [new branch]      ft/service-redesign -> ft/service-redesign   

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git checkout main 
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)      
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a") 

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git add  .

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   services.html


User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git commit -m "Modified services"
[main 0cbd912] Modified services
 1 file changed, 1 insertion(+)

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 356 bytes | 356.00 KiB/s, done.      
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/NelHim/Gym-Git-Exercise-Solutions.git       
   eabad58..0cbd912  main -> main

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git checkout ft/
ft/bundle-2           ft/service-redesign

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git checkout ft/
ft/bundle-2           ft/service-redesign

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git checkout ft/service-redesign 
Switched to branch 'ft/service-redesign'

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git status
On branch ft/service-redesign
nothing to commit, working tree clean

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result. 

MERGING)
$ git merge
fatal: You have not concluded your merge (MERGE_HEAD exists).
Please, commit your changes before you merge.

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/service-redesign|MERGING)
$ git merge
fatal: You have not concluded your merge (MERGE_HEAD exists).
Please, commit your changes before you merge.

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/service-redesign|MERGING)
$ git status
On branch ft/service-redesign
All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)


User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/service-redesign|MERGING)
$ git add .

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/service-redesign|MERGING)
$ git status
On branch ft/service-redesign
All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)


User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/service-redesign|MERGING)
$ git commit -m "Completed the merging"
[ft/service-redesign d2b5de2] Completed the merging

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git status
On branch ft/service-redesign
nothing to commit, working tree clean

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use    

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git push origin ft/service-redesign
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 225 bytes | 225.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/NelHim/Gym-Git-Exercise-Solutions.git
   f7a7b51..d2b5de2  ft/service-redesign -> ft/service-redesign

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/service-redesign)
$

```


## Bundle 3

### Exercise 1

```bash 

  User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git checkout ft/team-page
error: pathspec 'ft/team-page' did not match any file(s) known to git   

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/team-page)
$ code team.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/team-page)
$ git status
On branch ft/team-page
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   team.html

no changes added to commit (use "git add" and/or "git commit -a")       

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/team-page)
$ git add .

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/team-page)
$ git status
On branch ft/team-page
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   team.html


User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/team-page)
$ git commit -m "Team file"
[ft/team-page 1a28c1b] Team file
 1 file changed, 1 insertion(+), 1 deletion(-)

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/team-page)
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking       
upstream, see 'push.autoSetupRemote' in 'git help config'.


User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/team-page)
$ git push --set-upstream origin ft/team-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 293 bytes | 293.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.   
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting: 
remote:      https://github.com/NelHim/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/NelHim/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/team-page)
$ git checkout main 
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git checkout ft/team-page 
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/team-page)
$ git log
commit 1a28c1b2135beac3fe26c5630225bc3112152a7b (HEAD -> ft/team-page, origin/ft/team-page)
Author: NelHim <n.himbaza@alustudent.com>
Date:   Fri Jul 28 11:14:40 2023 +0200

    Team file

commit db3f69d037035caa647c18dcec9aca619e6b077d (origin/main, origin/HEAD, main, ft/contact-page)
Author: NelHim <n.himbaza@alustudent.com>
Date:   Thu Jul 27 11:35:13 2023 +0200

    Bundle 2 Exercise 2

commit 0cbd9120fcd29ca408d27a810af2c66129dccd57
Author: NelHim <n.himbaza@alustudent.com>
Date:   Thu Jul 27 11:24:19 2023 +0200

    Modified services

commit eabad580a49a0c6e1c5761443919e0efeee4a3c9

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/team-page)
$ git checkout ft/contact-page 
Switched to branch 'ft/contact-page'

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git cherry-pick 1a28c1b2135beac3fe26c5630225bc3112152a7b
[ft/contact-page 40f3013] Team file
 Date: Fri Jul 28 11:14:40 2023 +0200
 1 file changed, 1 insertion(+), 1 deletion(-)

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/contact-page)
$ code contact.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git log
commit 40f301336a6a123a9ad2848da044ffacddc7f1bc (HEAD -> ft/contact-page)
Author: NelHim <n.himbaza@alustudent.com>
Date:   Fri Jul 28 11:14:40 2023 +0200

    Team file

commit db3f69d037035caa647c18dcec9aca619e6b077d (origin/main, origin/HEAD, main)
Author: NelHim <n.himbaza@alustudent.com>
Date:   Thu Jul 27 11:35:13 2023 +0200

    Bundle 2 Exercise 2

commit 0cbd9120fcd29ca408d27a810af2c66129dccd57
Author: NelHim <n.himbaza@alustudent.com>
Date:   Thu Jul 27 11:24:19 2023 +0200

    Modified services

commit eabad580a49a0c6e1c5761443919e0efeee4a3c9

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git status
On branch ft/contact-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)        
        contact.html

nothing added to commit but untracked files present (use "git add" to track)

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git add .

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git commit -m "create the contact page"
[ft/contact-page 308fa5e] create the contact page
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git status
On branch ft/contact-page
nothing to commit, working tree clean

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking       
upstream, see 'push.autoSetupRemote' in 'git help config'.


User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/contact-page)
$   git push --set-upstream origin ft/contact-page
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 12 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 735 bytes | 735.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.   
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/NelHim/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/NelHim/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/faq-page)
$ code faq.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git status
On branch ft/faq-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)        
        faq.html

nothing added to commit but untracked files present (use "git add" to track)

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git add .

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git commit -m "Create the faq page"
[ft/faq-page 70f1230] Create the faq page
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking       
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 478 bytes | 478.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/NelHim/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/NelHim/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git revert 1a28c1b2135beac3fe26c5630225bc3112152a7b

hint: Waiting for your editor to close the file...

                                                   Vim: Error reading input, exiting...
Vim: Finished.
error: There was a problem with the editor 'vi'.
Please supply the message using either -m or -F option.

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git status
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   team.html


User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git add .


User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git commit -m "reverted the last commit of the ft/team-page"
[ft/faq-page 885c44d] reverted the last commit of the ft/team-page
 1 file changed, 1 insertion(+), 1 deletion(-)

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 327 bytes | 327.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/NelHim/Gym-Git-Exercise-Solutions.git
   70f1230..885c44d  ft/faq-page -> ft/faq-page


```


### Exercise 2

```bash

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git checkout ft/faq-page 
Switched to branch 'ft/faq-page'
Your branch is up to date with 'origin/ft/faq-page'.


User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git branch ft/home-page-redesign

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git branch
  dev
  ft/bundle-2
  ft/contact-page
* ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
  main

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git checkout main 
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ ld
bash: ld: command not found

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ ls
about.html  home.html  README.md  services.html  team.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ code about.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   about.html

no changes added to commit (use "git add" and/or "git commit -a")       

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git add .

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git commit -m "modified about.html"
[main 5b41576] modified about.html
 1 file changed, 1 insertion(+), 1 deletion(-)

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git push
To https://github.com/NelHim/Gym-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/NelHim/Gym-Git-Exercise-Solutions.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git pull
remote: Enumerating objects: 10, done.
remote: Counting objects: 100% (10/10), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (6/6), 2.03 KiB | 69.00 KiB/s, done.
From https://github.com/NelHim/Gym-Git-Exercise-Solutions
   5855544..443aa35  main       -> origin/main
Merge made by the 'ort' strategy.
 contact.html  | 11 +++++++++++
 faq.html      | 11 +++++++++++
 services.html |  2 +-
 team.html     |  2 +-
 4 files changed, 24 insertions(+), 2 deletions(-)
 create mode 100644 contact.html
 create mode 100644 faq.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 9, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 12 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 640 bytes | 640.00 KiB/s, done.
Total 5 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.   
To https://github.com/NelHim/Gym-Git-Exercise-Solutions.git
   443aa35..a591e6b  main -> main
Switched to branch 'ft/home-page-redesign'

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.      

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git status
On branch ft/home-page-redesign
nothing to commit, working tree clean

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ code home.html 

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git status
On branch ft/home-page-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory) 
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")       

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git add .

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git commit -m #
error: switch `m' requires a value

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git commit -m "modified the home.html"
[ft/home-page-redesign d972ef9] modified the home.html
 1 file changed, 1 insertion(+), 1 deletion(-)

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git push
fatal: The current branch ft/home-page-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign

To have this happen automatically for branches without a tracking       
upstream, see 'push.autoSetupRemote' in 'git help config'.


User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$  git push --set-upstream origin ft/home-page-redesign
Enumerating objects: 5, done.
d 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.   
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/NelHim/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote:
To https://github.com/NelHim/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign     
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.

```


## Bundle 4

### Exercise 1

```bash

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git remote add git-copy https://github.com/NelHim/git-exercise-clone.git

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git remote
git-copy
origin

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ ls
about.html    faq.html   README.md      team.html
contact.html  home.html  services.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ code home.html

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)      
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a") 

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git add .

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git commit -m "Updated home page"
[main b77db7f] Updated home page
 1 file changed, 7 insertions(+), 1 deletion(-)

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 366 bytes | 366.00 KiB/s, done.      
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/NelHim/Gym-Git-Exercise-Solutions.git       
   451c39c..b77db7f  main -> main

User@DESKTOP-68G4IPC MINGW64 ~/Desktop/The Gym Program/week3/Gym-Git-Exercise-Solutions (main)
$ git push git-copy 
Enumerating objects: 85, done.
Counting objects: 100% (85/85), done.
Delta compression using up to 12 threads
Compressing objects: 100% (82/82), done.
Writing objects: 100% (85/85), 15.93 KiB | 2.27 MiB/s, done.      
Total 85 (delta 44), reused 5 (delta 0), paDelta compression using up to 12 threads   
Compressing objects: 100% (82/82), done.   
e.
To https://github.com/NelHim/git-exercise-clone.git
 * [new branch]      main -> main

```

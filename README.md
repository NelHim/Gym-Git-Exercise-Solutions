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

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

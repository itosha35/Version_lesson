PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git log --oneline
c6f834f (HEAD -> main, origin/main) HW_1 for GIT added
8d43d84 seconde change
1649fda Changed
ce6e705 Create README.md
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git add .
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git commit -m "one more commit"
[main c01aeb9] one more commit
 1 file changed, 5 insertions(+), 1 deletion(-)
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git status
On branch main
nothing to commit, working tree clean
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git log
commit c01aeb9b8043adee425c993d7bf26e2c7879aa1f (HEAD -> main)
Author: unknown <itosha35@gmail.com>
Date:   Wed Jul 5 23:50:21 2023 +0300
    one more commit
commit c6f834f878b20c861a7cfa1db7240c670197b55a (origin/main)
Author: unknown <itosha35@gmail.com>
Date:   Wed Jul 5 21:05:22 2023 +0300
Date:   Wed Jul 5 23:50:21 2023 +0300

    one more commit
commit c6f834f878b20c861a7cfa1db7240c670197b55a (origin/main)
Author: unknown <itosha35@gmail.com>
Date:   Wed Jul 5 21:05:22 2023 +0300
    HW_1 for GIT added
commit 8d43d84b99db22799354d3c35b690db2e2bf6afd
Date:   Wed Jul 5 20:59:11 2023 +0300
    seconde change
commit 1649fda6deac585a0b4571666fb9bdf9ac24e471
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git diff 8d43 1649 README.md
diff --git a/README.md b/README.md
index cd22fd0..40f61d3 100644
--- a/README.md
+++ b/README.md
@@ -1,6 +1,3 @@
 # Version_lesson
 geekbrains repository for educational needs
 Bla-bla-bla
-
-
-Added some more and some new
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git diff c01ae 1649
deleted file mode 100644
index 1f81eef..0000000
+++ /dev/null
@@ -1,81 +0,0 @@
-PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git init
-On branch master
-No commits yet
-Untracked files:
-  (use "git add <file>..." to include in what will be committed)
-        README.md
-nothing added to commit but untracked files present (use "git add" to track)
-PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git commit -m "Readme added to local"
-commit 0ef118164f8b2dd89a7125b0bbf1923217d21f92 (HEAD -> master)
-Author: unknown <itosha35@gmail.com>
-    Readme added to local
-PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git branch master
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git status
On branch main
nothing to commit, working tree clean
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git blame README.md
^ce6e705 (Anton   2023-07-05 20:45:13 +0300  1) # Version_lesson
^ce6e705 (Anton   2023-07-05 20:45:13 +0300  2) geekbrains repository for educational needs
1649fda6 (unknown 2023-07-05 20:53:25 +0300  3) Bla-bla-bla
8d43d84b (unknown 2023-07-05 20:59:11 +0300  4)
c01aeb9b (unknown 2023-07-05 23:50:21 +0300  5) asfasdfasdfsadfsd
c01aeb9b (unknown 2023-07-05 23:50:21 +0300  6) asdf
8d43d84b (unknown 2023-07-05 20:59:11 +0300  7)
c01aeb9b (unknown 2023-07-05 23:50:21 +0300  8) sadf
c01aeb9b (unknown 2023-07-05 23:50:21 +0300  9) asdfasdf
c01aeb9b (unknown 2023-07-05 23:50:21 +0300 10) Added some more and some
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git checkout 8d43d8 README.md
Updated 1 path from 088d6a4
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git log
commit c01aeb9b8043adee425c993d7bf26e2c7879aa1f (HEAD -> main)
Author: unknown <itosha35@gmail.com>
Date:   Wed Jul 5 23:50:21 2023 +0300
    one more commit
commit c6f834f878b20c861a7cfa1db7240c670197b55a (origin/main)
Author: unknown <itosha35@gmail.com>
Date:   Wed Jul 5 21:05:22 2023 +0300
Author: unknown <itosha35@gmail.com>
Date:   Wed Jul 5 20:59:11 2023 +0300
    seconde change
commit 1649fda6deac585a0b4571666fb9bdf9ac24e471
Author: unknown <itosha35@gmail.com>
Date:   Wed Jul 5 20:53:25 2023 +0300
    Changed
Author: Anton <120050806+itosha35@users.noreply.github.com>
Date:   Wed Jul 5 20:45:13 2023 +0300
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git checkout 8d43 README.md
Updated 0 paths from 088d6a4
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git status
On branch main
Changes to be committed:
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git add .
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git commit -m "ONE MORE afetr REVERT"
[main 6f292b7] ONE MORE afetr REVERT
 1 file changed, 3 insertions(+), 5 deletions(-)
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git revert --no-commit 6f292b7
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git status
On branch main
You are currently reverting commit 6f292b7.
  (all conflicts fixed: run "git revert --continue")
  (use "git revert --skip" to skip this patch)
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git restore README.md
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git status
On branch main
You are currently reverting commit 6f292b7.
  (all conflicts fixed: run "git revert --continue")
  (use "git revert --abort" to cancel the revert operation)
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git clean -f
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git status
On branch main
You are currently reverting commit 6f292b7.
  (all conflicts fixed: run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md

PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git log
commit 6f292b72bd00e021b2f161d0b079f0cc6dab0ab4 (HEAD -> main)
Author: unknown <itosha35@gmail.com>
Date:   Wed Jul 5 23:58:07 2023 +0300

    ONE MORE afetr REVERT

commit c01aeb9b8043adee425c993d7bf26e2c7879aa1f
Author: unknown <itosha35@gmail.com>
Date:   Wed Jul 5 23:50:21 2023 +0300

    one more commit

commit c6f834f878b20c861a7cfa1db7240c670197b55a (origin/main)
Author: unknown <itosha35@gmail.com>
Date:   Wed Jul 5 21:05:22 2023 +0300

Author: unknown <itosha35@gmail.com>
Date:   Wed Jul 5 23:58:07 2023 +0300

    ONE MORE afetr REVERT

commit c01aeb9b8043adee425c993d7bf26e2c7879aa1f
Author: unknown <itosha35@gmail.com>
Date:   Wed Jul 5 23:50:21 2023 +0300

    one more commit

commit c6f834f878b20c861a7cfa1db7240c670197b55a (origin/main)
Author: unknown <itosha35@gmail.com>
Date:   Wed Jul 5 21:05:22 2023 +0300
    HW_1 for GIT added
commit 8d43d84b99db22799354d3c35b690db2e2bf6afd
error: unknown option `caches'
usage: git rm [<options>] [--] <file>...

    -n, --dry-run         dry run
    -q, --quiet           do not list removed files
    --cached              only remove from the index
    -f, --force           override the up-to-date check
    -r                    allow recursive removal
    --ignore-unmatch      exit with a zero status even if nothing matched
    --sparse              allow updating entries outside of the sparse-checkout cone
    --pathspec-from-file <file>
                          read pathspec from file
    --pathspec-file-nul   with --pathspec-from-file, pathspec elements are separated with NUL character

PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git rm --cached README.md
rm 'README.md'
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git status
On branch main
You are currently reverting commit 6f292b7.
  (all conflicts fixed: run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

Changes to be committed:
        deleted:    README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git add .
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git status
On branch main
You are currently reverting commit 6f292b7.
  (all conflicts fixed: run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

Changes to be committed:

PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git status
On branch main
You are currently reverting commit 6f292b7.
  (all conflicts fixed: run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git status
On branch main
  (all conflicts fixed: run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md
git: 'commi' is not a git command. See 'git --help'.

The most similar commands are
        commit
        column
[main 8bba3ee] HAve tried
 1 file changed, 6 insertions(+), 2 deletions(-)
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git log --oneline
8bba3ee (HEAD -> main) HAve tried
6f292b7 ONE MORE afetr REVERT
c6f834f (origin/main) HW_1 for GIT added
8d43d84 seconde change
1649fda Changed
ce6e705 Create README.md
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git reset --soft 6f292b7
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md

PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git reset --soft c01aeb9
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md

PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git log --graph
* commit c01aeb9b8043adee425c993d7bf26e2c7879aa1f (HEAD -> main)
| Author: unknown <itosha35@gmail.com>
| Date:   Wed Jul 5 23:50:21 2023 +0300
|
|     one more commit
|
* commit c6f834f878b20c861a7cfa1db7240c670197b55a (origin/main)
| Author: unknown <itosha35@gmail.com>
| Date:   Wed Jul 5 21:05:22 2023 +0300
|
| Author: unknown <itosha35@gmail.com>
| Date:   Wed Jul 5 23:50:21 2023 +0300
|
|
* commit c6f834f878b20c861a7cfa1db7240c670197b55a (origin/main)
| Author: unknown <itosha35@gmail.com>
| Date:   Wed Jul 5 21:05:22 2023 +0300
|
|     HW_1 for GIT added
|
* commit 8d43d84b99db22799354d3c35b690db2e2bf6afd
| Author: unknown <itosha35@gmail.com>
| Date:   Wed Jul 5 20:59:11 2023 +0300
|
|     seconde change
|
* commit 1649fda6deac585a0b4571666fb9bdf9ac24e471
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git commit --amend -m "HAHAHA"
[main 820bf69] HAHAHA
 Date: Wed Jul 5 23:50:21 2023 +0300
 1 file changed, 7 insertions(+), 1 deletion(-)
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git log --graph
* commit 820bf6979a951104e3686822c00a225f74b60636 (HEAD -> main)
| Author: unknown <itosha35@gmail.com>
| Date:   Wed Jul 5 23:50:21 2023 +0300
|
|     HAHAHA
|
* commit c6f834f878b20c861a7cfa1db7240c670197b55a (origin/main)
| Author: unknown <itosha35@gmail.com>
| Date:   Wed Jul 5 21:05:22 2023 +0300
|
| Author: unknown <itosha35@gmail.com>
| Date:   Wed Jul 5 23:50:21 2023 +0300
|
|     HAHAHA
|
* commit c6f834f878b20c861a7cfa1db7240c670197b55a (origin/main)
| Author: unknown <itosha35@gmail.com>
| Date:   Wed Jul 5 21:05:22 2023 +0300
|
|     HW_1 for GIT added
|
* commit 8d43d84b99db22799354d3c35b690db2e2bf6afd
| Author: unknown <itosha35@gmail.com>
| Date:   Wed Jul 5 20:59:11 2023 +0300
|
|     seconde change
|
* commit 1649fda6deac585a0b4571666fb9bdf9ac24e471
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git log
Date:   Wed Jul 5 23:50:21 2023 +0300

    HAHAHA

commit c6f834f878b20c861a7cfa1db7240c670197b55a (origin/main)

    HW_1 for GIT added

commit 8d43d84b99db22799354d3c35b690db2e2bf6afd
Author: unknown <itosha35@gmail.com>
Date:   Wed Jul 5 20:59:11 2023 +0300

    seconde change

commit 1649fda6deac585a0b4571666fb9bdf9ac24e471
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git restore README.md
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git add .
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git restore README.md
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git restore --staged README.md
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md
no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git reset --hard
HEAD is now at 820bf69 HAHAHA
PS C:\Users\Наталья\Desktop\Anton_GEEK\GIT\Git_ext_lessons> git status
On branch main
nothing to commit, working tree clean

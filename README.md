# Git-exercise-advanced

part1:
Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main) 
$ touch test{1..4}.md

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git add test1.md && git commit -m "chore: Create initial file"
[main 01c4ef4] chore: Create initial file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test1.md

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main) 
$ git add test2.md && git commit -m "chore: Create another file"       
[main db4ecae] chore: Create another file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test2.md

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main) 
$ git add test3.md && git commit -m "chore: Create third and fourth files"
[main 8d88d14] chore: Create third and fourth files
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main) 
$ git status
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test4.md

nothing added to commit but untracked files present (use "git add" to track)

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main) 
$ git log
commit 8d88d14a1bd7d68ee9d6161f6d97d6ac6b25ff4d (HEAD -> main
commit 8d88d14a1bd7d68ee9d6161f6d97d6ac6b25ff4d (HEAD -> main)
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Mon May 20 19:47:20 2024 +0200

    chore: Create third and fourth files

commit db4ecae99d574bbdea0422a0fb299e0ccee93339
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Mon May 20 19:47:17 2024 +0200

    chore: Create another file

commit 01c4ef44e763ac4531504975cca90ee14a8cbbdd
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Mon May 20 19:47:16 2024 +0200

    chore: Create initial file

commit 79c43eceda996037610341d97bad27d52aa7a040 (origin/main, origin/HEAD)
Author: Emeline Uwimbabazi <105202770+emelyne1234@users.noreply.github.com>
Date:   Mon May 20 19:32:43 2024 +0200
commit 8d88d14a1bd7d68ee9d6161f6d97d6ac6b25ff4d (HEAD -> main)
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Mon May 20 19:47:20 2024 +0200

    chore: Create third and fourth files

commit db4ecae99d574bbdea0422a0fb299e0ccee93339
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Mon May 20 19:47:17 2024 +0200

    chore: Create another file

commit 01c4ef44e763ac4531504975cca90ee14a8cbbdd
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Mon May 20 19:47:16 2024 +0200

    chore: Create initial file

commit 79c43eceda996037610341d97bad27d52aa7a040 (origin/main, origin/HEAD)
Author: Emeline Uwimbabazi <105202770+emelyne1234@users.noreply.github.com>
Date:   Mon May 20 19:32:43 2024 +0200

challenge2: editting commit history


Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)     
$ git add test4.md
Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)     
$ git commit --amend
[main 065df2c] test4 added
 Date: Mon May 20 19:47:20 2024 +0200
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md
 create mode 100644 test4.md

challenge 3:squashing
 This is a combination of 2 commits.
# This is the 1st commit message:

chore: Create initial file

# This is the commit message #2:


Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git reset HEAD~

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git add test3.md

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git commit -m 'create third file'
[main 006110d] create third file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git add test4.md

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git commit -m 'create forth file'
[main 6cc87cc] create forth file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test4.md

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$
pick 006110d create third file
# This is a combination of 2 commits.
ed (main)
$ git add test3.md

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git commit -m 'create third file'
[main 6cc87cc] create forth file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test4.md

pick 6025fab create third and fourth file
Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ touch unwanted.txt

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ vi unwanted.txt

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git add unwanted.txt
warning: LF will be replaced by CRLF in unwanted.txt.
The file will have its original line endings in your working directory

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git commit -m 'unwanted'
[main 4b60899] unwanted
 1 file changed, 1 insertion(+)
 create mode 100644 unwanted.txt

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git rebase -i HEAD~2
Successfully rebased and updated refs/heads/main.

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git rebase -i
Successfully rebased and updated refs/heads/main.

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (ft/branch)
$ touch test5.md

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (ft/branch)
$ git add .

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (ft/branch)
$ git commit -m 'Implemented test 5'
[ft/branch 02d2df5] Implemented test 5
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test5.md

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (ft/branch)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git log
commit 34363fc533c95902834b79e5a868ecb69a8f95f9 (HEAD -> main)
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Mon May 20 19:47:16 2024 +0200

    chore: Create initial file

    chore: Create second file

commit 644bf6a1f5604299759c87f94c1cd6ab7d5a5706
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Tue May 21 15:12:28 2024 +0200

    create third and fourth file

commit 79c43eceda996037610341d97bad27d52aa7a040 (origin/main, origin/HEAD)
Author: Emeline Uwimbabazi <105202770+emelyne1234@users.noreply.github.com>
Date:   Mon May 20 19:32:43 2024 +0200

    Initial commit

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git checkout ft/branch
Switched to branch 'ft/branch'

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (ft/branch)
$ git log
commit 02d2df535a8b10534bf089e66078e2a8e2693de0 (HEAD -> ft/branch)
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Tue May 21 17:32:41 2024 +0200

    Implemented test 5

commit 34363fc533c95902834b79e5a868ecb69a8f95f9 (main)
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Mon May 20 19:47:16 2024 +0200

    chore: Create initial file

    chore: Create second file

commit 644bf6a1f5604299759c87f94c1cd6ab7d5a5706
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Tue May 21 15:12:28 2024 +0200

    create third and fourth file

commit 79c43eceda996037610341d97bad27d52aa7a040 (origin/main, origin/HEAD)
Author: Emeline Uwimbabazi <105202770+emelyne1234@users.noreply.github.com>
Date:   Mon May 20 19:32:43 2024 +0200

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (ft/branch)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git cherry-pick 02d2df535a8b10534bf089e66078e2a8e2693de0
[main a0f3389] Implemented test 5
 Date: Tue May 21 17:32:41 2024 +0200
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test5.md

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git log
commit a0f3389fa147cbf611109950ac6f50956012fc51 (HEAD -> main)
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Tue May 21 17:32:41 2024 +0200

    Implemented test 5

commit 34363fc533c95902834b79e5a868ecb69a8f95f9
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Mon May 20 19:47:16 2024 +0200

    chore: Create initial file

    chore: Create second file

commit 644bf6a1f5604299759c87f94c1cd6ab7d5a5706
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Tue May 21 15:12:28 2024 +0200

    create third and fourth file

commit 79c43eceda996037610341d97bad27d52aa7a040 (origin/main, origin/HEAD)
Author: Emeline Uwimbabazi <105202770+emelyne1234@users.noreply.github.com>
Date:   Mon May 20 19:32:43 2024 +0200

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$
Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git checkout ft/branch
Switched to branch 'ft/branch'

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (ft/branch)
$ git log
commit 02d2df535a8b10534bf089e66078e2a8e2693de0 (HEAD -> ft/branch)
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Tue May 21 17:32:41 2024 +0200

    Implemented test 5

commit 34363fc533c95902834b79e5a868ecb69a8f95f9 (main)
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Mon May 20 19:47:16 2024 +0200

    chore: Create initial file

    chore: Create second file

commit 644bf6a1f5604299759c87f94c1cd6ab7d5a5706
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Tue May 21 15:12:28 2024 +0200

    create third and fourth file

commit 79c43eceda996037610341d97bad27d52aa7a040 (origin/main, origin/HEAD)
Author: Emeline Uwimbabazi <105202770+emelyne1234@users.noreply.github.com>
Date:   Mon May 20 19:32:43 2024 +0200

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (ft/branch)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git cherry-pick 02d2df535a8b10534bf089e66078e2a8e2693de0
[main a0f3389] Implemented test 5
 Date: Tue May 21 17:32:41 2024 +0200
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test5.md

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git log
commit a0f3389fa147cbf611109950ac6f50956012fc51 (HEAD -> main)
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Tue May 21 17:32:41 2024 +0200

    Implemented test 5

commit 34363fc533c95902834b79e5a868ecb69a8f95f9
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Mon May 20 19:47:16 2024 +0200

    chore: Create initial file

    chore: Create second file

commit 644bf6a1f5604299759c87f94c1cd6ab7d5a5706
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Tue May 21 15:12:28 2024 +0200

    create third and fourth file

commit 79c43eceda996037610341d97bad27d52aa7a040 (origin/main, origin/HEAD)
Author: Emeline Uwimbabazi <105202770+emelyne1234@users.noreply.github.com>
Date:   Mon May 20 19:32:43 2024 +0200

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git log --graph
* commit a0f3389fa147cbf611109950ac6f50956012fc51 (HEAD -> main)
| Author: mbabaziemelyne <uwimbeme@gmail.com>
| Date:   Tue May 21 17:32:41 2024 +0200
|
|     Implemented test 5
|
* commit 34363fc533c95902834b79e5a868ecb69a8f95f9
| Author: mbabaziemelyne <uwimbeme@gmail.com>
| Date:   Mon May 20 19:47:16 2024 +0200
|
|     chore: Create initial file
|
|     chore: Create second file
|
* commit 644bf6a1f5604299759c87f94c1cd6ab7d5a5706

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git reflog
a0f3389 (HEAD -> main) HEAD@{0}: cherry-pick: Implemented test 5
34363fc HEAD@{1}: checkout: moving from ft/branch to main
02d2df5 (ft/branch) HEAD@{2}: checkout: moving from main to ft/branch
34363fc HEAD@{3}: checkout: moving from ft/branch to main
02d2df5 (ft/branch) HEAD@{4}: commit: Implemented test 5
34363fc HEAD@{5}: checkout: moving from main to ft/branch
34363fc HEAD@{6}: rebase (finish): returning to refs/heads/main
34363fc HEAD@{7}: rebase (pick): chore: Create initial file
644bf6a HEAD@{8}: rebase (pick): create third and fourth file
79c43ec (origin/main, origin/HEAD) HEAD@{9}: rebase (start): checkout refs/remotes/origin/main
6025fab HEAD@{10}: rebase (finish): returning to refs/heads/main
6025fab HEAD@{11}: rebase (start): checkout HEAD~2
4b60899 HEAD@{12}: commit: unwanted
6025fab HEAD@{13}: rebase (finish): returning to refs/heads/main
6025fab HEAD@{14}: rebase (start): checkout HEAD~2
6025fab HEAD@{15}: rebase (finish): returning to refs/heads/main
6025fab HEAD@{16}: rebase (squash): create third and fourth file
006110d HEAD@{17}: rebase (start): checkout HEAD~2
6cc87cc HEAD@{18}: commit: create forth file
006110d HEAD@{19}: commit: create third file
9ad85de HEAD@{20}: reset: moving to HEAD~
4f8838d HEAD@{21}: reset: moving to HEAD
:

Part2:
Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git branch ft/new-feature

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git checkout ft/new-feature
Switched to branch 'ft/new-feature'

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (ft/new-feature)
$ touch feature.txt

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (ft/new-feature)
Introductory content ...
$ vi feature.txt

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (ft/new-feature)
$ git add feature.txt
warning: LF will be replaced by CRLF in feature.txt.
The file will have its original line endings in your working directory

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (ft/new-feature)
$ git commit -m 'Implemented core functionality for new feature'
[ft/new-feature 1dd29a5] Implemented core functionality for new feature
 1 file changed, 1 insertion(+)
 create mode 100644 feature.txt

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (ft/new-feature)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ touch readme.txt

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ vi readme.

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ ls
readme.  README.md  readme.txt  test1.md  test2.md  test3.md  test4.md  test5.md

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ rm readme.

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ ls
README.md  readme.txt  test1.md  test2.md  test3.md  test4.md  test5.md

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ vi readme.txt

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git add readme.txt 
warning: LF will be replaced by CRLF in readme.txt.
The file will have its original line endings in your working directory


Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git branch -d ft/new-feature
error: The branch 'ft/new-feature' is not fully merged.
If you are sure you want to delete it, run 'git branch -D ft/new-feature'.

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git branch -D ft/new-feature
Deleted branch ft/new-feature (was 1dd29a5).

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git log
commit a0f3389fa147cbf611109950ac6f50956012fc51 (HEAD -> main)
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Tue May 21 17:32:41 2024 +0200

    Implemented test 5

commit 34363fc533c95902834b79e5a868ecb69a8f95f9
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Mon May 20 19:47:16 2024 +0200

    chore: Create initial file

    chore: Create second file

commit 644bf6a1f5604299759c87f94c1cd6ab7d5a5706
Author: mbabaziemelyne <uwimbeme@gmail.com>
Date:   Tue May 21 15:12:28 2024 +0200

    create third and fourth file

commit 79c43eceda996037610341d97bad27d52aa7a040 (origin/main, origin/HEAD)
Author: Emeline Uwimbabazi <105202770+emelyne1234@users.noreply.github.com>
Date:   Mon May 20 19:32:43 2024 +0200

    Initial commit

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git checkout -b ft/new-branch-from-commit a0f3389fa147cbf611109950ac6f50956012fc51
Switched to a new branch 'ft/new-branch-from-commit'
A       readme.txt

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (ft/new-branch-from-commit)  
$ ls
README.md  readme.txt  test1.md  test2.md  test3.md  test4.md  test5.md

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (ft/new-branch-from-commit)  
$ git checkout main
Switched to branch 'main'
A       readme.txt
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git merge ft/new-branch-from-commit
Already up to date.


Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (ft/new-branch-from-commit)
$ git commit -m 'Committing new commit'
[ft/new-branch-from-commit 0d9d6c5] Committing new commit
 1 file changed, 1 insertion(+)
 create mode 100644 readme.txt


Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (ft/new-branch-from-commit)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git rebase ft/new-branch-from-commit
Successfully rebased and updated refs/heads/main.

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)
$ git checkout a0f3389fa147cbf611109950ac6f50956012fc51
Note: switching to 'a0f3389fa147cbf611109950ac6f50956012fc51'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at a0f3389 Implemented test 5

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced ((a0f3389...))
$ git switch -
Previous HEAD position was a0f3389 Implemented test 5
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)
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
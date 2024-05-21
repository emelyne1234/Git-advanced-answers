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

Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)     
$ git add test4.md
Lenovo@Emelyne MINGW64 ~/OneDrive/Desktop/Git-exercise-advanced (main)     
$ git commit --amend
[main 065df2c] test4 added
 Date: Mon May 20 19:47:20 2024 +0200
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md
 create mode 100644 test4.md
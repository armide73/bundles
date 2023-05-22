 Bundle 1-1
============

(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint: 
hint: 	git config --global init.defaultBranch <name>
hint: 
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint: 
hint: 	git branch -m <name>
Initialized empty Git repository in /home/armide/Desktop/myproject/.git/
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch -m main
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ touch file1
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ ls
file1
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ touch file2.txt
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ ls
file1  file2.txt
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	file1
	file2.txt

nothing added to commit but untracked files present (use "git add" to track)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add .
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   file1
	new file:   file2.txt

(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git log
fatal: your current branch 'main' does not have any commits yet
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'first commit'
[main (root-commit) a15dd0e] first commit
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 file1
 create mode 100644 file2.txt
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git log
commit a15dd0e3160988fa3efa0be2ded66f123555653b (HEAD -> main)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Thu May 18 23:44:22 2023 +0200

    first commit
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git remote add origin https://github.com/armide73/green.git
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin main
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/armide73/green.git/'
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin main
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/armide73/green.git/'
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin main
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 223 bytes | 223.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/armide73/green.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ 
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch -a
* main
  remotes/origin/main
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout -bdev
Switched to a new branch 'dev'
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout -btest
Switched to a new branch 'test'
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch
  dev
  main
* test
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout dev
Switched to branch 'dev'
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch -d test
Deleted branch test (was a15dd0e).
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch
* dev
  main
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ 
  
            bundle 1-2
            ===========
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ touch home.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ ls
file1  file2.txt  home.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	home.html

nothing added to commit but untracked files present (use "git add" to track)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add home.html 
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'home'
[dev e01506f] home
 1 file changed, 12 insertions(+)
 create mode 100644 home.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch dev
nothing to commit, working tree clean
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git log
commit e01506fe2c70d70fdf698b142a3dbd25d317b22f (HEAD -> dev)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 00:21:04 2023 +0200

    home

commit a15dd0e3160988fa3efa0be2ded66f123555653b (origin/main, main)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Thu May 18 23:44:22 2023 +0200

    first commit
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git reset --hard a15dd0e3160988fa3efa0be2ded66f123555653b
HEAD is now at a15dd0e first commit
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git log
commit a15dd0e3160988fa3efa0be2ded66f123555653b (HEAD -> dev, origin/main, main)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Thu May 18 23:44:22 2023 +0200

    first commit
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	home.html

nothing added to commit but untracked files present (use "git add" to track)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add home.html 
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'home'
[main aa045d2] home
 1 file changed, 12 insertions(+)
 create mode 100644 home.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git log
commit aa045d2b4734802d9973c66d034d5df1a7ad3c84 (HEAD -> main)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 00:40:27 2023 +0200

    home

commit a15dd0e3160988fa3efa0be2ded66f123555653b (origin/main, dev)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Thu May 18 23:44:22 2023 +0200

    first commit
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git stash save 'stash home.html'
Saved working directory and index state On main: stash home.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git stash list
stash@{0}: On main: stash home.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add about.html 
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'about.html'
[main c553963] about.html
 1 file changed, 13 insertions(+)
 create mode 100644 about.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git stash save 'stash about.html'
Saved working directory and index state On main: stash about.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git stash list
stash@{0}: On main: stash about.html
stash@{1}: On main: stash home.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add team.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'team.html'
[main 892c630] team.html
 1 file changed, 12 insertions(+)
 create mode 100644 team.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git stash save 'stash team.html'
Saved working directory and index state On main: stash team.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git stash list
stash@{0}: On main: stash team.html
stash@{1}: On main: stash about.html
stash@{2}: On main: stash home.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git log
commit 892c6306395b283e48e8853fed7fae9c18c2c1ed (HEAD -> main)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 01:02:12 2023 +0200

    team.html

commit c5539635c5e7c64bef87b5f82e73c5f9be696f40
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 00:51:55 2023 +0200

    about.html

commit aa045d2b4734802d9973c66d034d5df1a7ad3c84
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 00:40:27 2023 +0200

    home

commit a15dd0e3160988fa3efa0be2ded66f123555653b (origin/main, dev)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Thu May 18 23:44:22 2023 +0200

    first commit
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git stash pop stash@{1} 
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   about.html

no changes added to commit (use "git add" and/or "git commit -a")
Dropped stash@{1} (ddde1ab3128a2c61471f98807c11f4e5a4c7de0e)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git stash list 
stash@{0}: On main: stash team.html
stash@{1}: On main: stash home.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git stash pop stash@{1} 
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   about.html
	modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")
Dropped stash@{1} (1882d087294c9df0e62537eaf24b54aa13793f7e)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin main
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 4 threads
Compressing objects: 100% (8/8), done.
Writing objects: 100% (8/8), 899 bytes | 899.00 KiB/s, done.
Total 8 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), done.
To https://github.com/armide73/green.git
   a15dd0e..892c630  main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git stash list 
stash@{0}: On main: stash team.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git stash pop stash@{0} 
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   about.html
	modified:   home.html
	modified:   team.html

no changes added to commit (use "git add" and/or "git commit -a")
Dropped stash@{0} (3399a1a92ec501e3403a8581a2804b053125af01)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git log
commit 892c6306395b283e48e8853fed7fae9c18c2c1ed (HEAD -> main, origin/main)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 01:02:12 2023 +0200

    team.html

commit c5539635c5e7c64bef87b5f82e73c5f9be696f40
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 00:51:55 2023 +0200

    about.html

commit aa045d2b4734802d9973c66d034d5df1a7ad3c84
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 00:40:27 2023 +0200

    home

commit a15dd0e3160988fa3efa0be2ded66f123555653b (dev)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Thu May 18 23:44:22 2023 +0200

    first commit
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git reset HEAD^
Unstaged changes after reset:
M	about.html
M	home.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git log
commit c5539635c5e7c64bef87b5f82e73c5f9be696f40 (HEAD -> main)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 00:51:55 2023 +0200

    about.html

commit aa045d2b4734802d9973c66d034d5df1a7ad3c84
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 00:40:27 2023 +0200

    home

commit a15dd0e3160988fa3efa0be2ded66f123555653b (dev)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Thu May 18 23:44:22 2023 +0200

    first commit
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ 
  
      bundle2-1
      =========
  
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ touch services.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ ls
about.html  file1  file2.txt  home.html  services.html  team.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch
  dev
* ft/bundle-2
  main
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add .
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git log
commit c5539635c5e7c64bef87b5f82e73c5f9be696f40 (HEAD -> ft/bundle-2, main)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 00:51:55 2023 +0200

    about.html

commit aa045d2b4734802d9973c66d034d5df1a7ad3c84
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 00:40:27 2023 +0200

    home

commit a15dd0e3160988fa3efa0be2ded66f123555653b (dev)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Thu May 18 23:44:22 2023 +0200

    first commit
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'service.html'
[ft/bundle-2 a8a3b51] service.html
 4 files changed, 26 insertions(+), 1 deletion(-)
 create mode 100644 services.html
 create mode 100644 team.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch ft/bundle-2
nothing to commit, working tree clean
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git log
commit a8a3b51d2417c381bf14adaf72eb751c9a37c2d4 (HEAD -> ft/bundle-2)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 01:47:05 2023 +0200

    service.html

commit c5539635c5e7c64bef87b5f82e73c5f9be696f40 (main)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 00:51:55 2023 +0200

    about.html

commit aa045d2b4734802d9973c66d034d5df1a7ad3c84
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 00:40:27 2023 +0200

    home

commit a15dd0e3160988fa3efa0be2ded66f123555653b (dev)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Thu May 18 23:44:22 2023 +0200

    first commit
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin ft/bundle-2 
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 539 bytes | 539.00 KiB/s, done.
Total 5 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/armide73/green/pull/new/ft/bundle-2
remote: 
To https://github.com/armide73/green.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
Branch 'ft/bundle-2' set up to track remote branch 'ft/bundle-2' from 'origin'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ 
  
      bundle 2-2
      ===========
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch ft/service-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add services.html 
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'service.html changes'
[ft/service-redesign ff40407] service.html changes
 1 file changed, 1 insertion(+), 1 deletion(-)
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git log
commit ff4040754adc35986a92ed2f8fc89eb816b0f982 (HEAD -> ft/service-redesign)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 02:19:09 2023 +0200

    service.html changes

commit a8a3b51d2417c381bf14adaf72eb751c9a37c2d4 (origin/ft/bundle-2, ft/bundle-2)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 01:47:05 2023 +0200

    service.html

commit c5539635c5e7c64bef87b5f82e73c5f9be696f40 (main)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 00:51:55 2023 +0200

    about.html

commit aa045d2b4734802d9973c66d034d5df1a7ad3c84
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 00:40:27 2023 +0200

armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ 
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ 
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ 
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin ft/service-redesign 
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 17, done.
Counting objects: 100% (17/17), done.
Delta compression using up to 4 threads
Compressing objects: 100% (16/16), done.
Writing objects: 100% (17/17), 1.55 KiB | 1.55 MiB/s, done.
Total 17 (delta 8), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (8/8), done.
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/armide73/green/pull/new/ft/service-redesign
remote: 
To https://github.com/armide73/green.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
Branch 'ft/service-redesign' set up to track remote branch 'ft/service-redesign' from 'origin'.
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout main
error: Your local changes to the following files would be overwritten by checkout:
	services.html
Please commit your changes or stash them before you switch branches.
Aborting
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch
  dev
  ft/bundle-2
* ft/service-redesign
  main
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git stash save 'service redisign'
Saved working directory and index state On service-redesign: service redisign
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 1 commit, and can be fast-forwarded.
  (use "git pull" to update your local branch)
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ 
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch
  dev
  ft/bundle-2
  ft/service-redesign
* main
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch
  dev
  ft/bundle-2
  ft/service-redesign
* main
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git stash list
stash@{0}: On service-redesign: service redisign
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git stash pop stash@{0} 
CONFLICT (modify/delete): services.html deleted in Updated upstream and modified in Stashed changes. Version Stashed changes of services.html left in tree at services.html~Stashed changes.
The stash entry is kept in case you need it again.
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git stash save 'service redisign'
services.html: needs merge
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git stash list
stash@{0}: On service-redesign: service redisign
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch
  dev
  ft/bundle-2
  ft/service-redesign
* main
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add services.html
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'service.html update main'
[main fb8141d] service.html update main
 1 file changed, 13 insertions(+)
 create mode 100644 services.html
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin main
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
To https://github.com/armide73/green.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/armide73/green.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch main
Your branch and 'origin/main' have diverged,
and have 1 and 1 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	services.html~Stashed changes

nothing added to commit but untracked files present (use "git add" to track)
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add .
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch main
Your branch and 'origin/main' have diverged,
and have 1 and 1 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	new file:   services.html~Stashed changes

armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add services.html
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'service.html update main'
[main 5833919] service.html update main
 1 file changed, 13 insertions(+)
 create mode 100644 services.html~Stashed changes
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin main
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
To https://github.com/armide73/green.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/armide73/green.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git pull origin 
remote: Enumerating objects: 8, done.
remote: Counting objects: 100% (8/8), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 4 (delta 2), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (4/4), 1.33 KiB | 1.33 MiB/s, done.
From https://github.com/armide73/green
   892c630..acc622f  main        -> origin/main
   a8a3b51..7430b6f  ft/bundle-2 -> origin/ft/bundle-2
hint: You have divergent branches and need to specify how to reconcile them.
hint: You can do so by running one of the following commands sometime before
hint: your next pull:
hint: 
hint:   git config pull.rebase false  # merge (the default strategy)
hint:   git config pull.rebase true   # rebase
hint:   git config pull.ff only       # fast-forward only
hint: 
hint: You can replace "git config" with "git config --global" to set a default
hint: preference for all repositories. You can also pass --rebase, --no-rebase,
hint: or --ff-only on the command line to override the configured default per
hint: invocation.
fatal: Need to specify how to reconcile divergent branches.
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git merge
Auto-merging services.html
CONFLICT (add/add): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git merge
fatal: You have not concluded your merge (MERGE_HEAD exists).
Please, commit your changes before you merge.
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch main
Your branch and 'origin/main' have diverged,
and have 2 and 4 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)

Changes to be committed:
	modified:   about.html
	modified:   home.html
	modified:   services.html
	new file:   team.html

armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin main
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
remote: Invalid username or password.
fatal: Authentication failed for 'https://github.com/armide73/green.git/'
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin main
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
To https://github.com/armide73/green.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/armide73/green.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'service conflict fix'
[main 8cdcff9] service conflict fix
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin main
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 12, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 4 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (9/9), 1.14 KiB | 1.14 MiB/s, done.
Total 9 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
To https://github.com/armide73/green.git
   acc622f..8cdcff9  main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ 
  
      Bundle 3-1
      ==========

(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch
  dev
  ft/bundle-2
  ft/service-redesign
* ft/team-page
  main
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ touch team.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ ls
 about.html   file2.txt   services.html                    team.html
 file1        home.html  'services.html~Stashed changes'
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch ft/team-page
nothing to commit, working tree clean
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch ft/team-page
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   team.html

no changes added to commit (use "git add" and/or "git commit -a")
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add team.html 
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'team changes'
[ft/team-page 3808d1e] team changes
 1 file changed, 1 insertion(+), 1 deletion(-)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin ft/team-page
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 19, done.
Counting objects: 100% (18/18), done.
Delta compression using up to 4 threads
Compressing objects: 100% (13/13), done.
Writing objects: 100% (13/13), 1.96 KiB | 1.96 MiB/s, done.
Total 13 (delta 7), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (7/7), completed with 4 local objects.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/armide73/green/pull/new/ft/team-page
remote: 
To https://github.com/armide73/green.git
 * [new branch]      ft/team-page -> ft/team-page
Branch 'ft/team-page' set up to track remote branch 'ft/team-page' from 'origin'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch
  dev
  ft/bundle-2
  ft/service-redesign
  ft/team-page
* main
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch ft/contact-page
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/service-redesign
  ft/team-page
* main
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout ft/team-page 
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git log
commit 3808d1ece4749563d3b379e334be8625d5d2e886 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 14:38:08 2023 +0200

    team changes

commit 8cdcff984175dae37193c030b311e7b7eb6ce53f (origin/main, main, ft/contact-page)
Merge: 5833919 acc622f
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 03:03:04 2023 +0200

    service conflict fix

commit 583391978ef17f2c5c307e07d82b88086a6e5bfb
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 02:44:39 2023 +0200

    service.html update main

commit fb8141d63a200deaafcec6564d0b0860396e8201
Author: Armide Tuyishime <armide.tuyi@gmail.com>
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout ft/contact-page 
Switched to branch 'ft/contact-page'
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git cherry-pick 3808d1ece4749563d3b379e334be8625d5d2e886
[ft/contact-page 257a792] team changes
 Date: Fri May 19 14:38:08 2023 +0200
 1 file changed, 1 insertion(+), 1 deletion(-)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add contact.html 
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'contact changes'
[ft/contact-page 7ee9e97] contact changes
 1 file changed, 12 insertions(+)
 create mode 100644 contact.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin ft/contact-page 
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 720 bytes | 720.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/armide73/green/pull/new/ft/contact-page
remote: 
To https://github.com/armide73/green.git
 * [new branch]      ft/contact-page -> ft/contact-page
Branch 'ft/contact-page' set up to track remote branch 'ft/contact-page' from 'origin'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch
  dev
  ft/bundle-2
  ft/contact-page
* ft/faq-page
  ft/service-redesign
  ft/team-page
  main
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add faq.html 
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'faq changes'
[ft/faq-page 490c528] faq changes
 1 file changed, 12 insertions(+)
 create mode 100644 faq.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin ft/faq-page 
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 233 bytes | 233.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/armide73/green/pull/new/ft/faq-page
remote: 
To https://github.com/armide73/green.git
 * [new branch]      ft/faq-page -> ft/faq-page
Branch 'ft/faq-page' set up to track remote branch 'ft/faq-page' from 'origin'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git log
commit 490c528f0545c371bf124d236db353279ec82cb3 (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 15:09:38 2023 +0200

    faq changes

commit 7ee9e97c6db0c15876a173eae7492aff47ae6437 (origin/ft/contact-page, ft/contact-page)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 15:04:21 2023 +0200

    contact changes

commit 257a7922b56d8024b68b87c08b65608c804a5ff0
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 14:38:08 2023 +0200

    team changes

commit 8cdcff984175dae37193c030b311e7b7eb6ce53f (origin/main, main)
Merge: 5833919 acc622f
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 03:03:04 2023 +0200

    service conflict fix

commit 583391978ef17f2c5c307e07d82b88086a6e5bfb
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 02:44:39 2023 +0200

    service.html update main

commit fb8141d63a200deaafcec6564d0b0860396e8201
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 02:35:48 2023 +0200

    service.html update main

commit acc622f30821b662f138af1c2ad0be1b72cadf3e
Merge: 892c630 7430b6f
Author: Armide Tuyishime <92937079+armide73@users.noreply.github.com>
Date:   Fri May 19 01:59:06 2023 +0200

    Merge pull request #1 from armide73/ft/bundle-2
    
    service.html

commit 7430b6f592067cf7ee2a5f25c12e816f2f7170d1 (origin/ft/bundle-2)
Merge: a8a3b51 892c630
Author: Armide Tuyishime <92937079+armide73@users.noreply.github.com>
Date:   Fri May 19 01:58:41 2023 +0200

    Merge branch 'main' into ft/bundle-2

commit a8a3b51d2417c381bf14adaf72eb751c9a37c2d4 (ft/bundle-2)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 01:47:05 2023 +0200

    service.html

commit 490c528f0545c371bf124d236db353279ec82cb3 (HEAD -> ft/faq-page, origin/ft/
faq-page)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 15:09:38 2023 +0200

    faq changes

commit 7ee9e97c6db0c15876a173eae7492aff47ae6437 (origin/ft/contact-page, ft/cont
act-page)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 15:04:21 2023 +0200

    contact changes

commit 257a7922b56d8024b68b87c08b65608c804a5ff0
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 14:38:08 2023 +0200

    team changes

commit 8cdcff984175dae37193c030b311e7b7eb6ce53f (origin/main, main)
Merge: 5833919 acc622f
Author: Armide Tuyishime <armide.tuyi@gmail.com>
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout ft/team-page 
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git log
commit 3808d1ece4749563d3b379e334be8625d5d2e886 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 14:38:08 2023 +0200

    team changes

commit 8cdcff984175dae37193c030b311e7b7eb6ce53f (origin/main, main)
Merge: 5833919 acc622f
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 03:03:04 2023 +0200

    service conflict fix

commit 583391978ef17f2c5c307e07d82b88086a6e5bfb
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 02:44:39 2023 +0200

    service.html update main

commit fb8141d63a200deaafcec6564d0b0860396e8201
Author: Armide Tuyishime <armide.tuyi@gmail.com>
Date:   Fri May 19 02:35:48 2023 +0200
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git revert 3808d1ece4749563d3b379e334be8625d5d2e886
[ft/team-page 9b6fd5c] Revert "team changes"
 1 file changed, 1 insertion(+), 1 deletion(-)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch ft/team-page
Your branch is ahead of 'origin/ft/team-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin ft/team-page 
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 337 bytes | 337.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/armide73/green.git
   3808d1e..9b6fd5c  ft/team-page -> ft/team-page
Branch 'ft/team-page' set up to track remote branch 'ft/team-page' from 'origin'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin ft/team-page 
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Branch 'ft/team-page' set up to track remote branch 'ft/team-page' from 'origin'.
Everything up-to-date
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ 
  
        Bundle 3-2
        ============
  
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
* ft/home-page-redesign
  ft/service-redesign
  ft/team-page
  main
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ ls
 about.html   file2.txt   services.html                    team.html
 file1        home.html  'services.html~Stashed changes'
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add home.html 
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	modified:   home.html

(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'main changes'
[main 4bc89e9] main changes
 1 file changed, 1 insertion(+)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin main
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
To https://github.com/armide73/green.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/armide73/green.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git pull origin
remote: Enumerating objects: 22, done.
remote: Counting objects: 100% (19/19), done.
remote: Compressing objects: 100% (12/12), done.
remote: Total 12 (delta 6), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (12/12), 3.89 KiB | 39.00 KiB/s, done.
From https://github.com/armide73/green
   8cdcff9..479fed3  main                -> origin/main
   ff40407..ab7459b  ft/service-redesign -> origin/ft/service-redesign
hint: You have divergent branches and need to specify how to reconcile them.
hint: You can do so by running one of the following commands sometime before
hint: your next pull:
hint: 
hint:   git config pull.rebase false  # merge (the default strategy)
hint:   git config pull.rebase true   # rebase
hint:   git config pull.ff only       # fast-forward only
hint: 
hint: You can replace "git config" with "git config --global" to set a default
hint: preference for all repositories. You can also pass --rebase, --no-rebase,
hint: or --ff-only on the command line to override the configured default per
hint: invocation.
fatal: Need to specify how to reconcile divergent branches.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git merge
Merge made by the 'ort' strategy.
 contact.html  | 12 ++++++++++++
 faq.html      | 12 ++++++++++++
 services.html |  1 +
 3 files changed, 25 insertions(+)
 create mode 100644 contact.html
 create mode 100644 faq.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin main
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 9, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 592 bytes | 592.00 KiB/s, done.
Total 5 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
To https://github.com/armide73/green.git
   479fed3..c8cf30a  main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout ft/home-page-redesign 
Switched to branch 'ft/home-page-redesign'
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git rebase main ft/home-page-redesign
Successfully rebased and updated refs/heads/ft/home-page-redesign.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch ft/home-page-redesign
nothing to commit, working tree clean
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch ft/home-page-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add home.html 
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'home.html changes'
[ft/home-page-redesign d0295d1] home.html changes
 1 file changed, 1 insertion(+)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch ft/home-page-redesign
nothing to commit, working tree clean
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin ft/home-page-redesign 
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 322 bytes | 322.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/armide73/green/pull/new/ft/home-page-redesign
remote: 
To https://github.com/armide73/green.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
Branch 'ft/home-page-redesign' set up to track remote branch 'ft/home-page-redesign' from 'origin'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ 

      Bundle 4-1
      ==========
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git remote add git-copy https://github.com/armide73/second_bundle_repo
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add home.html 
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'git copy changes'
[main bce8fab] git copy changes
 1 file changed, 1 insertion(+)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin main
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
To https://github.com/armide73/green.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/armide73/green.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git pull origin
remote: Enumerating objects: 9, done.
remote: Counting objects: 100% (9/9), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 7 (delta 2), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (7/7), 7.61 KiB | 216.00 KiB/s, done.
From https://github.com/armide73/green
   c8cf30a..6ff04ae  main       -> origin/main
hint: You have divergent branches and need to specify how to reconcile them.
hint: You can do so by running one of the following commands sometime before
hint: your next pull:
hint: 
hint:   git config pull.rebase false  # merge (the default strategy)
hint:   git config pull.rebase true   # rebase
hint:   git config pull.ff only       # fast-forward only
hint: 
hint: You can replace "git config" with "git config --global" to set a default
hint: preference for all repositories. You can also pass --rebase, --no-rebase,
hint: or --ff-only on the command line to override the configured default per
hint: invocation.
fatal: Need to specify how to reconcile divergent branches.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git merge 
Auto-merging home.html
CONFLICT (content): Merge conflict in home.html
Automatic merge failed; fix conflicts and then commit the result.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch main
Your branch and 'origin/main' have diverged,
and have 1 and 4 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Changes to be committed:
	new file:   README.md

Unmerged paths:
  (use "git add <file>..." to mark resolution)
	both modified:   home.html

(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add home.html 
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'git copy changes'
[main aaa0aea] git copy changes
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin main
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 634 bytes | 634.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 3 local objects.
remote: This repository moved. Please use the new location:
remote:   https://github.com/armide73/bundles.git
To https://github.com/armide73/green.git
   6ff04ae..aaa0aea  main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u git-copy 
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 74, done.
Counting objects: 100% (74/74), done.
Delta compression using up to 4 threads
Compressing objects: 100% (72/72), done.
Writing objects: 100% (74/74), 17.41 KiB | 2.49 MiB/s, done.
Total 74 (delta 42), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (42/42), done.
To https://github.com/armide73/second_bundle_repo
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'git-copy'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ 
  
      Bundle 4-2
      ==========
 (base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch ft/footer
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   faq.html

no changes added to commit (use "git add" and/or "git commit -a")
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add faq.html 
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'faq.html changes'
[ft/footer 8468a21] faq.html changes
 1 file changed, 1 insertion(+), 1 deletion(-)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch ft/footer
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   faq.html

no changes added to commit (use "git add" and/or "git commit -a")
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git add faq.html 
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'faq.html second changes'
[ft/footer 164cb8c] faq.html second changes
 1 file changed, 1 insertion(+)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin ft/footer 
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 583 bytes | 583.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
remote: This repository moved. Please use the new location:
remote:   https://github.com/armide73/bundles.git
remote: 
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/armide73/bundles/pull/new/ft/footer
remote: 
To https://github.com/armide73/green.git
 * [new branch]      ft/footer -> ft/footer
Branch 'ft/footer' set up to track remote branch 'ft/footer' from 'origin'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'git-copy/main'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git checkout -b ft/squshing
Switched to a new branch 'ft/squshing'
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git merge --squash ft/footer 
Updating aaa0aea..164cb8c
Fast-forward
Squash commit -- not updating HEAD
 faq.html | 3 ++-
 1 file changed, 2 insertions(+), 1 deletion(-)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git status
On branch ft/squshing
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	modified:   faq.html

(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git commit -m 'footer changes squashing'
[ft/squshing b9601f4] footer changes squashing
 1 file changed, 2 insertions(+), 1 deletion(-)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ git push -u origin ft/squshing 
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 335 bytes | 335.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: This repository moved. Please use the new location:
remote:   https://github.com/armide73/bundles.git
remote: 
remote: Create a pull request for 'ft/squshing' on GitHub by visiting:
remote:      https://github.com/armide73/bundles/pull/new/ft/squshing
remote: 
To https://github.com/armide73/green.git
 * [new branch]      ft/squshing -> ft/squshing
Branch 'ft/squshing' set up to track remote branch 'ft/squshing' from 'origin'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/myproject$ 
  
        Bundle 5-2
        ===========
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone$ git clone https://github.com/armide73/git-cafe-exercise.git
Cloning into 'git-cafe-exercise'...
remote: Enumerating objects: 107, done.
remote: Counting objects: 100% (12/12), done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 107 (delta 5), reused 4 (delta 4), pack-reused 95
Receiving objects: 100% (107/107), 1.95 MiB | 2.29 MiB/s, done.
Resolving deltas: 100% (5/5), done.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone$ cd git-cafe-exercise/
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git add index.html 
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	modified:   index.html

(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git commit -m 'index.html changes'
[main 8ce0cfc] index.html changes
 1 file changed, 1 insertion(+), 1 deletion(-)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git branch
* main
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git push -u origin main
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 323 bytes | 323.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/armide73/git-cafe-exercise.git
   d1d3f9c..8ce0cfc  main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ 
  
  Bundle 6-1
  ==========
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git branch
* main
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git checkout -b exercise1
Switched to a new branch 'exercise1'
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ touch Menu.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ ls
bat  images        index-2.html  index-4.html  js         README.md
css  index-1.html  index-3.html  index.html    Menu.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git status
On branch exercise1
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	Menu.html

nothing added to commit but untracked files present (use "git add" to track)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git add Menu.html 
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git commit -m 'Menu.html changes'
[exercise1 45e71ed] Menu.html changes
 1 file changed, 12 insertions(+)
 create mode 100644 Menu.html
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git push -u origin exercise1 
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 458 bytes | 458.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'exercise1' on GitHub by visiting:
remote:      https://github.com/armide73/git-cafe-exercise/pull/new/exercise1
remote: 
To https://github.com/armide73/git-cafe-exercise.git
 * [new branch]      exercise1 -> exercise1
Branch 'exercise1' set up to track remote branch 'exercise1' from 'origin'.
  
      Bundle 6-2
      ==========
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git checkout -b exercise2
Switched to a new branch 'exercise2'
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git status
On branch exercise2
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   index-4.html

no changes added to commit (use "git add" and/or "git commit -a")
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git add index-4.html 
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git commit -m 'index-4.html changes'
[exercise2 6f2d485] index-4.html changes
 1 file changed, 1 insertion(+), 1 deletion(-)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git push -u origin exercise2
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 309 bytes | 309.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'exercise2' on GitHub by visiting:
remote:      https://github.com/armide73/git-cafe-exercise/pull/new/exercise2
remote: 
To https://github.com/armide73/git-cafe-exercise.git
 * [new branch]      exercise2 -> exercise2
Branch 'exercise2' set up to track remote branch 'exercise2' from 'origin'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ 
  
        Bundle 6-3
        ==========
 (base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git checkout -b exercise3
Switched to a new branch 'exercise3'

(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git add index-4.html 
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git commit -m "phone number change"
[exercise3 47a1a85] phone number change
 1 file changed, 1 insertion(+), 1 deletion(-)
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$ git push -u origin exercise3
Username for 'https://github.com': armide73
Password for 'https://armide73@github.com': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 302 bytes | 302.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'exercise3' on GitHub by visiting:
remote:      https://github.com/armide73/git-cafe-exercise/pull/new/exercise3
remote: 
To https://github.com/armide73/git-cafe-exercise.git
 * [new branch]      exercise3 -> exercise3
Branch 'exercise3' set up to track remote branch 'exercise3' from 'origin'.
(base) armide@armide-ZHAOYANG-E40-80:~/Desktop/cafe_exercice_clone/git-cafe-exercise$  
  
  
  
  
  
  
  

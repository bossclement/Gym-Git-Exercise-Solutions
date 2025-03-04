# Bundle 1
## Exercise 1 answers
```bash
gymbigogwe@Bigogwes-iMac b1e1 % git init
Initialized empty Git repository in /Users/gymbigogwe/Desktop/deleteme/b1e1/.git/
gymbigogwe@Bigogwes-iMac b1e1 % echo hello world > file1.txt
gymbigogwe@Bigogwes-iMac b1e1 % echo hello world again > file2.txt
gymbigogwe@Bigogwes-iMac b1e1 % git branch -M main
gymbigogwe@Bigogwes-iMac b1e1 % git add -A
gymbigogwe@Bigogwes-iMac b1e1 % git remote add origin https://github.com/bossclement/Gym-Git-Exercise-Solutions.git
gymbigogwe@Bigogwes-iMac b1e1 % git commit -m "corrected mistakes in exercise one"
[master 0a5cc07] corrected mistakes in exercise one
 2 files changed, 2 insertions(+)
 create mode 100644 file1.txt
 create mode 100644 file2.txt
gymbigogwe@Bigogwes-iMac b1e1 % git remote set-url origin https://bossclement:<secret token>@github.com/bossclement/Gym-Git-Exercise-Solutions.git
gymbigogwe@Bigogwes-iMac b1e1 % git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 365 bytes | 365.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'main' on GitHub by visiting:
remote:      https://github.com/bossclement/Gym-Git-Exercise-Solutions/pull/new/master
remote: 
To https://github.com/bossclement/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main
gymbigogwe@Bigogwes-iMac b1e1 % 
```
## Exercise 2 answers
```bash
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % echo "<p>home page</p>" > home.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git add home.html         gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git stash
Saved working directory and index state WIP on main: a9ec18c starting flesh with exercise 2 bundle1
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git stash list
stash@{0}: WIP on main: a9ec18c starting flesh with exercise 2 bundle1
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % echo "<p>about page</p>" > about.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git add about.html 
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git stash
Saved working directory and index state WIP on main: a9ec18c starting flesh with exercise 2 bundle1
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % echo "<p>team page</p>" > team.html  
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git add team.html 
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git stash
Saved working directory and index state WIP on main: a9ec18c starting flesh with exercise 2 bundle1
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % ls
README.md	file1.txt	file2.txt
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git stash list
stash@{0}: WIP on main: a9ec18c starting flesh with exercise 2 bundle1
stash@{1}: WIP on main: a9ec18c starting flesh with exercise 2 bundle1
stash@{2}: WIP on main: a9ec18c starting flesh with exercise 2 bundle1
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git stash pop 2
On branch main
Your branch and 'origin/main' have diverged,
and have 1 and 1 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	new file:   home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   README.md

Dropped refs/stash@{2} (d792a603db02198b1c65f4fc049afc55e78d83c4)
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git add home.html 
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git stash  
Saved working directory and index state WIP on main: a9ec18c starting flesh with exercise 2 bundle1
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git stash pop 2
On branch main
Your branch and 'origin/main' have diverged,
and have 1 and 1 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	new file:   about.html

Dropped refs/stash@{2} (5301dc40eca8ababd3b1723451d58ecd6d4a86e7)
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git stash pop 0
On branch main
Your branch and 'origin/main' have diverged,
and have 1 and 1 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	new file:   about.html
	new file:   home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   README.md

Dropped refs/stash@{0} (853ff0ff1bf8cd30397aa4d6a4f3438f8940516e)
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git add .
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git commit -m "added home and about html files"
[main 6e0c138] added home and about html files
 3 files changed, 6 insertions(+), 10 deletions(-)
 create mode 100644 about.html
 create mode 100644 home.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git stash pop
On branch main
Your branch and 'origin/main' have diverged,
and have 2 and 1 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	new file:   team.html

Dropped refs/stash@{0} (9c6a45bbb9042d627907954ff038f2a4683ba8c2)
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git resset --hard
git: 'resset' is not a git command. See 'git --help'.

The most similar command is
	reset
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % ls
README.md	file1.txt	home.html
about.html	file2.txt	team.html
```
# Bundle 2
## Exercise 1
```bash
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % echo "<p>services page</p>" services.html
<p>services page</p> services.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % echo "<p>services page</p>" > services.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git add services.html 
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git commit -m "added service page" 
[ft/bundle-2 04da568] added service page
 1 file changed, 1 insertion(+)
 create mode 100644 services.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git push origin ft-bundle-2
error: src refspec ft-bundle-2 does not match any
error: failed to push some refs to 'https://github.com/bossclement/Gym-Git-Exercise-Solutions.git'
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git status
On branch ft/bundle-2
nothing to commit, working tree clean
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git push origin ft/bundle-2
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 629 bytes | 629.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/bossclement/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote: 
To https://github.com/bossclement/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
```
# Bundle 3
## Exercise 1 answers
```bash
git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % echo "<p>changes in team file</p>" > team.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git add .
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git status
On branch ft/team-page
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	new file:   team.html

gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git commit -m "created a teamfile"
[ft/team-page 7da3a96] created a teamfile
 1 file changed, 1 insertion(+)
 create mode 100644 team.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git push origin ft/team-page
Enumerating objects: 30, done.
Counting objects: 100% (30/30), done.
Delta compression using up to 8 threads
Compressing objects: 100% (20/20), done.
Writing objects: 100% (30/30), 3.92 KiB | 3.92 MiB/s, done.
Total 30 (delta 9), reused 8 (delta 3), pack-reused 0
remote: Resolving deltas: 100% (9/9), done.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/bossclement/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote: 
To https://github.com/bossclement/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout main
Switched to branch 'main'
Your branch and 'origin/main' have diverged,
and have 2 and 1 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout ft/team-page
Switched to branch 'ft/team-page'
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git log
commit 7da3a96cc6ab910e4bed797c3645db5da2c2b764 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Gym Bigogwe <gymbigogwe@Bigogwes-iMac.local>
Date:   Tue Mar 4 11:50:12 2025 +0200

    created a teamfile

commit 6e0c138b4698b25506bb997370e2d61246d74e44 (main, ft/contact-page)
Author: Gym Bigogwe <gymbigogwe@Bigogwes-iMac.local>
Date:   Tue Mar 4 11:32:33 2025 +0200

    added home and about html files

commit a9ec18cf5d6a294ff21282e444d11001d0339c5a
Author: Gym Bigogwe <gymbigogwe@Bigogwes-iMac.local>
Date:   Tue Mar 4 11:04:26 2025 +0200

    starting flesh with exercise 2 bundle1

commit 5062abd1c993c6706f85eddabd496bd5154b0e23
Author: bossclement <122975092+bossclement@users.noreply.github.com>
Date:   Tue Mar 4 10:54:40 2025 +0200

gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout ft/contact-page
Switched to branch 'ft/contact-page'
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git cherry-pick 7da3a96cc6ab910e4bed797c3645db5da2c2b764
[ft/contact-page b973cbe] created a teamfile
 Date: Tue Mar 4 11:50:12 2025 +0200
 1 file changed, 1 insertion(+)
 create mode 100644 team.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % ls
README.md	file1.txt	home.html
about.html	file2.txt	team.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % echo "<p>Contact page</p>" > contact.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git add .
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git commint -m "added contact page" 
git: 'commint' is not a git command. See 'git --help'.

The most similar command is
	commit
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git commit -m "added contact page" 
[ft/contact-page af5b58c] added contact page
 1 file changed, 1 insertion(+)
 create mode 100644 contact.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git status
On branch ft/contact-page
nothing to commit, working tree clean
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git push origin ft/contact-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (6/6), 564 bytes | 564.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/bossclement/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote: 
To https://github.com/bossclement/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % echo "<p>Faq page</p>" > faq.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git add .
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git commit -m 'added faq page'    
[ft/faq-page 0d13bf2] added faq page
 1 file changed, 1 insertion(+)
 create mode 100644 faq.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git push origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 290 bytes | 290.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/bossclement/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote: 
To https://github.com/bossclement/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git log
commit 0d13bf2b60ae061b52a243877fca14874596ab2c (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: Gym Bigogwe <gymbigogwe@Bigogwes-iMac.local>
Date:   Tue Mar 4 12:09:13 2025 +0200

    added faq page

commit af5b58c1b3fb769c059fa4d829c22bd6e58d9d5e (origin/ft/contact-page, ft/contact-page)
Author: Gym Bigogwe <gymbigogwe@Bigogwes-iMac.local>
Date:   Tue Mar 4 12:04:47 2025 +0200

    added contact page

commit b973cbe3c8b884d24dcbc2b0bb1fe855beb03cbb
Author: Gym Bigogwe <gymbigogwe@Bigogwes-iMac.local>
Date:   Tue Mar 4 11:50:12 2025 +0200

    created a teamfile

commit 6e0c138b4698b25506bb997370e2d61246d74e44 (main)
Author: Gym Bigogwe <gymbigogwe@Bigogwes-iMac.local>
Date:   Tue Mar 4 11:32:33 2025 +0200
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git revert b973cbe3c8b884d24dcbc2b0bb1fe855beb03cbb
[ft/faq-page 9a1ff17] Revert "created a teamfile"
 1 file changed, 1 deletion(-)
 delete mode 100644 team.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git push origin ft/faq-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 302 bytes | 302.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/bossclement/Gym-Git-Exercise-Solutions.git
   0d13bf2..9a1ff17  ft/faq-page -> ft/faq-page
```

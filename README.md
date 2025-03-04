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
## Exercise 2
```bash
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout main
Already on 'main'
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git pull
Already up to date.
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % echo "<p>service page</p>" > service.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git add .
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git commit -m "added service page"
[ft/service-redesign 0cf80d3] added service page
 1 file changed, 1 insertion(+)
 create mode 100644 service.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git push origin t/service-redesign
error: src refspec t/service-redesign does not match any
error: failed to push some refs to 'https://github.com/bossclement/Gym-Git-Exercise-Solutions.git'
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git push origin ft/service-redesign
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 619 bytes | 619.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/bossclement/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote: 
To https://github.com/bossclement/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % cat >> service.html
<p>added a new feature</p>    
^C
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git add .
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git commit -m "edited services in main"
[main 2cba8ef] edited services in main
 1 file changed, 1 insertion(+)
 create mode 100644 service.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 320 bytes | 320.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/bossclement/Gym-Git-Exercise-Solutions.git
   4c87399..2cba8ef  main -> main
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git merge main
Auto-merging service.html
CONFLICT (add/add): Merge conflict in service.html
Automatic merge failed; fix conflicts and then commit the result.
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % vim service.html 
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git add .
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git commit -m "merged service page from main to ft/service redesign branchs"
[ft/service-redesign 25ef2de] merged service page from main to ft/service redesign branchs
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git push origin ft/service-redesign
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 360 bytes | 360.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/bossclement/Gym-Git-Exercise-Solutions.git
   0cf80d3..25ef2de  ft/service-redesign -> ft/service-redesign
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
## Exercise 2
```bash
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout ft/faq-page
Switched to branch 'ft/faq-page'
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout main 
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % vim home.html 
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git add .
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git commit -m "added contents in home.html"
[main 2fa850f] added contents in home.html
 1 file changed, 1 insertion(+)
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git git checkout ft/home-page-redesign
git: 'git' is not a git command. See 'git --help'.

The most similar command is
	init
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout ft/home-page-redesign   
Switched to branch 'ft/home-page-redesign'
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git rebase main
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not apply bcd611e... finished budnle 3 exercise 1
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".
Could not apply bcd611e... finished budnle 3 exercise 1
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % vim README.md  
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git add .
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git commit -m "updated the readme file of redesign branch to the latest one"
[detached HEAD 74ee407] updated the readme file of redesign branch to the latest one
 1 file changed, 31 insertions(+)
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git push
fatal: You are not currently on a branch.
To push the history leading to the current (detached HEAD)
state now, use

    git push origin HEAD:<name-of-remote-branch>
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % vim home.html 
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git add home.html 
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git commit -m "changes in home.html"
[detached HEAD 3f1a744] changes in home.html
 1 file changed, 1 insertion(+)
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git push origin ft/home-page-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 2.15 KiB | 2.15 MiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting
remote:      https://github.com/bossclement/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote: 
To https://github.com/bossclement/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
```
## Bundle 4
# Exercise 1
```bash
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % vim home.html 
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git add home.html 
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git commit -m "added new changes in home"
[main 28c6f29] added new changes in home
 1 file changed, 1 insertion(+)
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git push origin
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 336 bytes | 336.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/bossclement/Gym-Git-Exercise-Solutions.git
   2fa850f..28c6f29  main -> main
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git remote add git-copy https://bossclement:<secret token>@github.com/bossclement/Git-exercise-clone.git
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git push git-copy
Enumerating objects: 54, done.
Counting objects: 100% (54/54), done.
Delta compression using up to 8 threads
Compressing objects: 100% (43/43), done.
Writing objects: 100% (54/54), 11.36 KiB | 11.36 MiB/s, done.
Total 54 (delta 22), reused 8 (delta 3), pack-reused 0
remote: Resolving deltas: 100% (22/22), done.
To https://github.com/bossclement/Git-exercise-clone.git
 * [new branch]      main -> main
```
# Exercise 2
```bash
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout -b ft/footer
Switched to a new branch 'ft/footer'
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % echo "<p>Footer page</p>" > footer.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git add footer.html 
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git commit -m "added fotter "
[ft/footer e74fed8] added fotter
 1 file changed, 1 insertion(+)
 create mode 100644 footer.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git push origin ft/footer
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 296 bytes | 296.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/bossclement/Gym-Git-Exercise-Solutions/pull/new/ft/footer
remote: 
To https://github.com/bossclement/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/footer -> ft/footer
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout ft/footer
Switched to branch 'ft/footer'
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % cat >> footer.html 
<p>New changes</p>
^C
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git add footer.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git commit -m "added second changes in footer"
[ft/footer 1596e01] added second changes in footer
 1 file changed, 1 insertion(+)
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git push origin ft/footer
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 315 bytes | 315.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/bossclement/Gym-Git-Exercise-Solutions.git
   e74fed8..1596e01  ft/footer -> ft/footer
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout ft/squashing
error: pathspec 'ft/squashing' did not match any file(s) known to git
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git merge --squash ft/footer
Updating 28c6f29..1596e01
Fast-forward
Squash commit -- not updating HEAD
 footer.html | 2 ++
 1 file changed, 2 insertions(+)
 create mode 100644 footer.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git commit -m "footer changes squashing"
[ft/squashing 63efe79] footer changes squashing
 1 file changed, 2 insertions(+)
 create mode 100644 footer.html
gymbigogwe@Bigogwes-iMac Gym-Git-Exercise-Solutions % git push origin ft/squashing
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 323 bytes | 323.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/bossclement/Gym-Git-Exercise-Solutions/pull/new/ft/squashing
remote: 
To https://github.com/bossclement/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/squashing -> ft/squashing
```

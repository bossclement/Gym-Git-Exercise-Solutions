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

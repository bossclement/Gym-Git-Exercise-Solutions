# Bundle 1
## Exercise 1 answers
```bash
gymbigogwe@Bigogwes-iMac b1e1 % git init
Initialized empty Git repository in /Users/gymbigogwe/Desktop/deleteme/b1e1/.git/
gymbigogwe@Bigogwes-iMac b1e1 % echo hello world > file1.txt
gymbigogwe@Bigogwes-iMac b1e1 % echo hello world again > file2.txt
gymbigogwe@Bigogwes-iMac b1e1 % git branch -M master
gymbigogwe@Bigogwes-iMac b1e1 % git add -A
gymbigogwe@Bigogwes-iMac b1e1 % git remote add origin https://github.com/bossclement/Gym-Git-Exercise-Solutions.git
gymbigogwe@Bigogwes-iMac b1e1 % git pull origin main
From https://github.com/bossclement/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
gymbigogwe@Bigogwes-iMac b1e1 % ls
File_1.txt	README.md	file1.txt	home.html
File_2.txt	about.html	file2.txt
gymbigogwe@Bigogwes-iMac b1e1 % git commit -m "corrected mistakes in exercise one"
[master 0a5cc07] corrected mistakes in exercise one
 2 files changed, 2 insertions(+)
 create mode 100644 file1.txt
 create mode 100644 file2.txt
gymbigogwe@Bigogwes-iMac b1e1 % git remote set-url origin https://bossclement:<secret token>@github.com/bossclement/Gym-Git-Exercise-Solutions.git
gymbigogwe@Bigogwes-iMac b1e1 % git push origin master
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 365 bytes | 365.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/bossclement/Gym-Git-Exercise-Solutions/pull/new/master
remote: 
To https://github.com/bossclement/Gym-Git-Exercise-Solutions.git
 * [new branch]      master -> master
gymbigogwe@Bigogwes-iMac b1e1 % 
```

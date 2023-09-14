park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git init
Initialized empty Git repository in C:/Users/park250s/Desktop/new/.git/

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (master)
$ git init -b main
warning: re-init: ignored --initial-branch=main
Reinitialized existing Git repository in C:/Users/park250s/Desktop/new/.git/

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (master)
$ eval "$(ssh-agent -s)"
Agent pid 2330

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (master)
$ ssh-keygen -t ed25519 -C "park250s@uregina.ca"
Generating public/private ed25519 key pair.
Enter file in which to save the key (/c/Users/park250s/.ssh/id_ed25519):
/c/Users/park250s/.ssh/id_ed25519 already exists.
Overwrite (y/n)? y
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/park250s/.ssh/id_ed25519
Your public key has been saved in /c/Users/park250s/.ssh/id_ed25519.pub
The key fingerprint is:
SHA256:ay2T4T5CvUloy3tpj4dF7gTEpYnNE0pnzF2E/eOi/sw park250s@uregina.ca
The key's randomart image is:
+--[ED25519 256]--+
|      .++o.=o    |
|     . B=+o .    |
|      o.*    .   |
|        ...   o  |
|       oS+   . . |
|      +.o=+ . .  |
|     + oBO.. .   |
|      +oO++o     |
|      .=o=o.E    |
+----[SHA256]-----+

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (master)
$ clip < ~/.ssh/id_ed25519.pub

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.md

nothing added to commit but untracked files present (use "git add" to track)

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (master)
$ git add *

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (master)
$ git commit -m "new"
[master (root-commit) 63e06f1] new
 1 file changed, 1 insertion(+)
 create mode 100644 readme.md

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (master)
$ git branch -M main

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git push -u origin main
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git remote add origin git@github.com:park250ss/374lab.git

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git branch -M main




park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git push -u origin main
Enter passphrase for key '/c/Users/park250s/.ssh/id_ed25519':
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 204 bytes | 204.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:park250ss/374lab.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git add *

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git commit -m "html"
[main 3fda5c3] html
 1 file changed, 12 insertions(+)
 create mode 100644 hello.html

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git push -u origin main
Enter passphrase for key '/c/Users/park250s/.ssh/id_ed25519':
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 459 bytes | 459.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:park250ss/374lab.git
   63e06f1..3fda5c3  main -> main
branch 'main' set up to track 'origin/main'.

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git add *

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git commit -m "2nd readme"
[main 4641cf7] 2nd readme
 1 file changed, 6 insertions(+)
 create mode 100644 2ndreadme.md

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git push -u origin main
Enter passphrase for key '/c/Users/park250s/.ssh/id_ed25519':
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 402 bytes | 201.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:park250ss/374lab.git
   3fda5c3..4641cf7  main -> main
branch 'main' set up to track 'origin/main'.

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git add *

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git commit -m "music"
[main 241866a] music
 1 file changed, 1 insertion(+)
 create mode 100644 music.txt

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git push -u origin main
Enter passphrase for key '/c/Users/park250s/.ssh/id_ed25519':
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 274 bytes | 274.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:park250ss/374lab.git
   4641cf7..241866a  main -> main
branch 'main' set up to track 'origin/main'.

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git branch alternate

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git add *

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git commit -m "timeline"
[main 0d4d34b] timeline
 1 file changed, 1 insertion(+)
 create mode 100644 timeline.txt

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git push -u origin main
Enter passphrase for key '/c/Users/park250s/.ssh/id_ed25519':
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 277 bytes | 277.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:park250ss/374lab.git
   241866a..0d4d34b  main -> main
branch 'main' set up to track 'origin/main'.

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git add *

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git commit -m "onlyone"
[main 7ba577e] onlyone
 1 file changed, 1 insertion(+)
 create mode 100644 onlyone.txt

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git push -u origin main
Enter passphrase for key '/c/Users/park250s/.ssh/id_ed25519':
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 268 bytes | 268.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:park250ss/374lab.git
   0d4d34b..7ba577e  main -> main
branch 'main' set up to track 'origin/main'.



park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git checkout alternate
Switched to branch 'alternate'

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (alternate)
$ git add *

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (alternate)
$ git commit -m "darkest"
[alternate 1abc0a6] darkest
 1 file changed, 1 insertion(+)
 create mode 100644 timeline.txt

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (alternate)
$ git push -u origin alternate
Enter passphrase for key '/c/Users/park250s/.ssh/id_ed25519':
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 280 bytes | 280.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'alternate' on GitHub by visiting:
remote:      https://github.com/park250ss/374lab/pull/new/alternate
remote:
To github.com:park250ss/374lab.git
 * [new branch]      alternate -> alternate
branch 'alternate' set up to track 'origin/alternate'.

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (alternate)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git merge alternate
Auto-merging timeline.txt
CONFLICT (add/add): Merge conflict in timeline.txt
Automatic merge failed; fix conflicts and then commit the result.

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main|MERGING)
$ git add *

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main|MERGING)
$ git commit -m "last"
[main 3b1134f] last

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git push -u origin main
Enter passphrase for key '/c/Users/park250s/.ssh/id_ed25519':
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 200 bytes | 200.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:park250ss/374lab.git
   7ba577e..3b1134f  main -> main
branch 'main' set up to track 'origin/main'.

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git log --all --decorate --oneline --graph
*   3b1134f (HEAD -> main, origin/main) last
|\
| * 1abc0a6 (origin/alternate, alternate) darkest
* | 7ba577e onlyone
* | 0d4d34b timeline
|/
* 241866a music
* 4641cf7 2nd readme
* 3fda5c3 html
* 63e06f1 new

park250s@ED4851-ST28 MINGW64 ~/Desktop/new (main)
$ git log --all --decorate --oneline --graph

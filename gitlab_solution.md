gitlab-hiba rezek



ex1 

1\. mkdir GitLab, cd gitlab

2\. git init

3\. a. it stores all vc info, commit history, branches, configs etc..

4\. echo "this is a readme file :) " > README.md

this is a readme file :)

README.md

5\. PS C:\\Users\\hibam\\Desktop\\gitlab> git status

On branch master



No commits yet



Untracked files:

&nbsp; (use "git add <file>..." to include in what will be committed)

&nbsp;       README.md



6\. PS C:\\Users\\hibam\\Desktop\\gitlab> git add README.md

PS C:\\Users\\hibam\\Desktop\\gitlab> git status

On branch master



No commits yet



Changes to be committed:

&nbsp; (use "git rm --cached <file>..." to unstage)

&nbsp;       new file:   README.md



readme now is in staging area.



7\. git commit -m "readme file created"

\[master (root-commit) c68a95a] readme file created

&nbsp;1 file changed, 0 insertions(+), 0 deletions(-)

&nbsp;create mode 100644 README.md



8.PS C:\\Users\\hibam\\Desktop\\gitlab> mkdir src

to create new directory

to add 2 files: echo > file1.py and same for file2.py



9.PS C:\\Users\\hibam\\Desktop\\gitlab> git add src

PS C:\\Users\\hibam\\Desktop\\gitlab> git status

On branch master

Changes to be committed:

&nbsp; (use "git restore --staged <file>..." to unstage)

&nbsp;       new file:   src/file1.py

&nbsp;       new file:   src/file2.py





committing the src :



PS C:\\Users\\hibam\\Desktop\\gitlab> git commit -m "added src folder"

\[master fee3af1] added src folder

&nbsp;2 files changed, 0 insertions(+), 0 deletions(-)

&nbsp;create mode 100644 src/file1.py

&nbsp;create mode 100644 src/file2.py



10.PS C:\\Users\\hibam\\Desktop\\gitlab> git diff

diff --git a/src/file1.py b/src/file1.py

index e69de29..61ad2b3 100644

--- a/src/file1.py

+++ b/src/file1.py

@@ -0,0 +1 @@

+#modifying the contents of file1.py for ex 1 q 10

\\ No newline at end of file



11.PS C:\\Users\\hibam\\Desktop\\gitlab> git add src/file1.py

PS C:\\Users\\hibam\\Desktop\\gitlab> git status

On branch master

Changes to be committed:

&nbsp; (use "git restore --staged <file>..." to unstage)

&nbsp;       modified:   src/file1.py



12\. c. PS C:\\Users\\hibam\\Desktop\\gitlab> git add src/file1.py

PS C:\\Users\\hibam\\Desktop\\gitlab> git status

On branch master

Changes to be committed:

&nbsp; (use "git restore --staged <file>..." to unstage)

&nbsp;       modified:   src/file1.py



13\. PS C:\\Users\\hibam\\Desktop\\gitlab> git commit -m "changes for file 1"

\[master 11fa249] changes for file 1

&nbsp;1 file changed, 1 insertion(+)

PS C:\\Users\\hibam\\Desktop\\gitlab> git log

commit 11fa2496a20259ff5f0ea124a9bbb92f9ec5ad87 (HEAD -> master)

Author: Hiba Rezek 

Date:   Mon Sep 22 14:02:13 2025 +0300



&nbsp;   changes for file 1



commit fee3af171002d3b9889180b3391d6228523920cb

Author: Hiba Rezek 

Date:   Mon Sep 22 13:56:07 2025 +0300



&nbsp;   added src folder



commit c68a95a21c30dbe96fdae33bcc98c00f86ee1dad

Author: Hiba Rezek 

Date:   Sun Sep 21 23:34:20 2025 +0300



&nbsp;   readme file created

&nbsp;

14.PS C:\\Users\\hibam\\Desktop\\gitlab> git show c68a95a21c

commit c68a95a21c30dbe96fdae33bcc98c00f86ee1dad

Author: Hiba Rezek 

Date:   Sun Sep 21 23:34:20 2025 +0300



&nbsp;   readme file created



diff --git a/README.md b/README.md

new file mode 100644

index 0000000..f42919e

Binary files /dev/null and b/README.md differ



**the minimum is 4 letters.**



15\. PS C:\\Users\\hibam\\Desktop\\gitlab> git log

commit 597adff345c715b0c6fd53e25351ad43fdd535ee (HEAD -> master)

Author: Hiba Rezek 

Date:   Mon Sep 22 14:10:17 2025 +0300



&nbsp;   added data.txt in src



commit 73bc144a82f48e0a978d055acd8593efcf634637

Author: Hiba Rezek 

Date:   Mon Sep 22 14:09:16 2025 +0300



&nbsp;   changes for file 2



commit 11fa2496a20259ff5f0ea124a9bbb92f9ec5ad87

Author: Hiba Rezek 

Date:   Mon Sep 22 14:02:13 2025 +0300



&nbsp;   changes for file 1



commit fee3af171002d3b9889180b3391d6228523920cb

Author: Hiba Rezek 

Date:   Mon Sep 22 13:56:07 2025 +0300



&nbsp;   added src folder



commit c68a95a21c30dbe96fdae33bcc98c00f86ee1dad

Author: Hiba Rezek 

Date:   Sun Sep 21 23:34:20 2025 +0300



&nbsp;   readme file created



modified file 2, and created a new txt file 





STRETCH TASK



1. PS C:\\Users\\hibam\\Desktop\\gitlab> git rm src/data.txt

rm 'src/data.txt'

data.txt is removed now.



2\. PS C:\\Users\\hibam\\Desktop\\gitlab> del newfile.txt



3.PS C:\\Users\\hibam\\Desktop\\gitlab> git status

On branch master

Changes to be committed:

&nbsp; (use "git restore --staged <file>..." to unstage)

&nbsp;       new file:   newfile.txt



Changes not staged for commit:

&nbsp; (use "git add/rm <file>..." to update what will be committed)

&nbsp; (use "git restore <file>..." to discard changes in working directory)

&nbsp;       deleted:    newfile.txt



&nbsp;git commit -m "deletion of newfile"

On branch master

nothing to commit, working tree clean



4.PS C:\\Users\\hibam\\Desktop\\gitlab> git mv file3.py src

PS C:\\Users\\hibam\\Desktop\\gitlab> git status

On branch master

Changes to be committed:

&nbsp; (use "git restore --staged <file>..." to unstage)

&nbsp;       renamed:    file3.py -> src/file3.py

&nbsp;

PS C:\\Users\\hibam\\Desktop\\gitlab> git add src/file3.py

PS C:\\Users\\hibam\\Desktop\\gitlab> git commit -m "moved file3 into src"

\[master 557eaa8] moved file3 into src

&nbsp;1 file changed, 0 insertions(+), 0 deletions(-)

&nbsp;rename file3.py => src/file3.py (100%)

created and commited file3.py, then moved it to src



5\.  PS C:\\Users\\hibam\\Desktop\\gitlab> git status

On branch master

Changes not staged for commit:

&nbsp; (use "git add/rm <file>..." to update what will be committed)

&nbsp; (use "git restore <file>..." to discard changes in working directory)

&nbsp;       deleted:    src/file2.py



Untracked files:

&nbsp; (use "git add <file>..." to include in what will be committed)

&nbsp;       src/newnamef2.py



no changes added to commit (use "git add" and/or "git commit -a")



the file is untracked now





&nbsp;	a. no because it is untracked

&nbsp;	b. git add newnamef2.py so that it becomes staged

&nbsp;	c. git considers that a rename is a deleted file and a new untracked file

6\. **to see last n commits we use git log -n**

PS C:\\Users\\hibam\\Desktop\\gitlab> git log -3

commit 060e26c11e14e83ae2ee1bbabeeddab9d2e75a38 (HEAD -> master)

Author: Hiba Rezek 

Date:   Tue Sep 23 08:04:46 2025 +0300



&nbsp;   renamed file2.py using system



commit 557eaa821135c581aef9a5aabc583ccfbefd27cd

Author: Hiba Rezek 

Date:   Tue Sep 23 07:59:02 2025 +0300



&nbsp;   moved file3 into src



commit 1ed5b0dc23b22b9163aba987b6e64e39e5fa5d15

Author: Hiba Rezek 

Date:   Mon Sep 22 14:25:13 2025 +0300



&nbsp;   add file3.py



7.--stat shows the summary of changes in a file

with git show it includes a summary of which files changed, how many lines were added/removed, and a total count.

with git diff it gives a per-file summary of changes between working directory and the index (or between two commits). 



8.PS C:\\Users\\hibam\\Desktop\\gitlab> git diff fee3..c68a

diff --git a/src/file1.py b/src/file1.py

deleted file mode 100644

index e69de29..0000000

diff --git a/src/file2.py b/src/file2.py

deleted file mode 100644

index e69de29..0000000

PS C:\\Users\\hibam\\Desktop\\gitlab> git diff c68a..fee3

diff --git a/src/file1.py b/src/file1.py

new file mode 100644

index 0000000..e69de29

diff --git a/src/file2.py b/src/file2.py

new file mode 100644

index 0000000..e69de29



true, the files were created.



---------------------------------------



ex2

1.PS C:\\Users\\hibam\\Desktop\\gitlab> git status

On branch master

nothing to commit, working tree clean



2.PS C:\\Users\\hibam\\Desktop\\gitlab> git branch my\_first\_branch



3.PS C:\\Users\\hibam\\Desktop\\gitlab> git checkout my\_first\_branch

Switched to branch 'my\_first\_branch'



4\. created data file and added content to it

PS C:\\Users\\hibam\\Desktop\\gitlab> git add data.txt

PS C:\\Users\\hibam\\Desktop\\gitlab> git commit -m "created data.txt"

\[my\_first\_branch c995dfa] created data.txt

&nbsp;1 file changed, 0 insertions(+), 0 deletions(-)

&nbsp;create mode 100644 data.txt

PS C:\\Users\\hibam\\Desktop\\gitlab> git add data.txt

PS C:\\Users\\hibam\\Desktop\\gitlab> git commit -m "adding data to data.txt"

\[my\_first\_branch 18258ef] adding data to data.txt

&nbsp;1 file changed, 1 insertion(+)



5.PS C:\\Users\\hibam\\Desktop\\gitlab> git log

commit 18258ef73c04f44a6e0570f925340f705710f290 (HEAD -> my\_first\_branch)

Author: Hiba Rezek 

Date:   Tue Sep 23 08:36:39 2025 +0300



&nbsp;   adding data to data.txt



commit c995dfa0e56ff7a6dc075a037e634fdb202d9461

Author: Hiba Rezek 

Date:   Tue Sep 23 08:35:56 2025 +0300



&nbsp;   created data.txt



commit 13a29b3ba0a9662388824c38455c6e4b88412ccc (master)

Author: Hiba Rezek 

Date:   Tue Sep 23 08:31:31 2025 +0300



&nbsp;   renamed file 2



true, the last 2 commits are on top.



6.PS C:\\Users\\hibam\\Desktop\\gitlab> git checkout master

Switched to branch 'master'

PS C:\\Users\\hibam\\Desktop\\gitlab> git log

commit 13a29b3ba0a9662388824c38455c6e4b88412ccc (HEAD -> master)

Author: Hiba Rezek 

Date:   Tue Sep 23 08:31:31 2025 +0300



&nbsp;   renamed file 2



commit 060e26c11e14e83ae2ee1bbabeeddab9d2e75a38

Author: Hiba Rezek 

Date:   Tue Sep 23 08:04:46 2025 +0300



&nbsp;   renamed file2.py using system



true, the files are no longer there



7\. PS C:\\Users\\hibam\\Desktop\\gitlab> git checkout my\_first\_branch

Switched to branch 'my\_first\_branch'

PS C:\\Users\\hibam\\Desktop\\gitlab> git log --graph

\* commit 18258ef73c04f44a6e0570f925340f705710f290 (HEAD -> my\_first\_branch)

| Author: Hiba Rezek 

| Date:   Tue Sep 23 08:36:39 2025 +0300

|

|     adding data to data.txt

|

\* commit c995dfa0e56ff7a6dc075a037e634fdb202d9461

| Author: Hiba Rezek 

| Date:   Tue Sep 23 08:35:56 2025 +0300

|

|     created data.txt

|

\* commit 13a29b3ba0a9662388824c38455c6e4b88412ccc (master)

| Author: Hiba Rezek 

| Date:   Tue Sep 23 08:31:31 2025 +0300

|

|     renamed file 2

|

\* commit 060e26c11e14e83ae2ee1bbabeeddab9d2e75a38

| Author: Hiba Rezek 

| Date:   Tue Sep 23 08:04:46 2025 +0300

|

|     renamed file2.py using system

|



it is linear.



8.a. PS C:\\Users\\hibam\\Desktop\\gitlab> git checkout master

Switched to branch 'master'

PS C:\\Users\\hibam\\Desktop\\gitlab> git merge my\_first\_branch

Updating 13a29b3..18258ef

Fast-forward

&nbsp;data.txt | 1 +

&nbsp;1 file changed, 1 insertion(+)

&nbsp;create mode 100644 data.txt

&nbsp;

**fast-forward merge**

b.PS C:\\Users\\hibam\\Desktop\\gitlab> git log

commit 18258ef73c04f44a6e0570f925340f705710f290 (HEAD -> master, my\_first\_branch)

Author: Hiba Rezek 

Date:   Tue Sep 23 08:36:39 2025 +0300



&nbsp;   adding data to data.txt



commit c995dfa0e56ff7a6dc075a037e634fdb202d9461

Author: Hiba Rezek 

Date:   Tue Sep 23 08:35:56 2025 +0300



&nbsp;   created data.txt

**no merge commit**

**c.**

PS C:\\Users\\hibam\\Desktop\\gitlab> git log --graph

\* commit 18258ef73c04f44a6e0570f925340f705710f290 (HEAD -> master, my\_first\_branch)

| Author: Hiba Rezek 

| Date:   Tue Sep 23 08:36:39 2025 +0300

|

|     adding data to data.txt

|

\* commit c995dfa0e56ff7a6dc075a037e634fdb202d9461

| Author: Hiba Rezek 

| Date:   Tue Sep 23 08:35:56 2025 +0300

|

|     created data.txt

|

\* commit 13a29b3ba0a9662388824c38455c6e4b88412ccc

| Author: Hiba Rezek 

| Date:   Tue Sep 23 08:31:31 2025 +0300

|

|     renamed file 2



**all is linear**



9\. modified files content for file1, file 3 and data



10\. modified newnamef2



11.PS C:\\Users\\hibam\\Desktop\\gitlab> git merge my\_first\_branch

Merge made by the 'ort' strategy.

&nbsp;data.txt     | 3 ++-

&nbsp;src/file1.py | 4 +++-

&nbsp;src/file3.py | 1 +

&nbsp;3 files changed, 6 insertions(+), 2 deletions(-)



12.PS C:\\Users\\hibam\\Desktop\\gitlab> git log

commit 4aee6aa7ec57bd043bd16f6f97f5e4b5e4eab01b (HEAD -> master)

Merge: 1732265 eb73bfb

Author: Hiba Rezek 

Date:   Tue Sep 23 08:53:00 2025 +0300



&nbsp;   Merge branch 'my\_first\_branch' -m "merge q11"



using git log --graph:

PS C:\\Users\\hibam\\Desktop\\gitlab> git log --graph

\*   commit 4aee6aa7ec57bd043bd16f6f97f5e4b5e4eab01b (HEAD -> master)

|\\  Merge: 1732265 eb73bfb

| | Author: Hiba Rezek 

| | Date:   Tue Sep 23 08:53:00 2025 +0300

| |

| |     Merge branch 'my\_first\_branch' -m "merge q11"

| |

| \* commit eb73bfbed182cab4b5e78feb18a5715798bf6daa (my\_first\_branch)

| | Author: Hiba Rezek 

| | Date:   Tue Sep 23 08:48:36 2025 +0300

| |

| |     added content to file3

| |

| \* commit 0c9358d933c14853ac8375d787595c9f2c48e373

| | Author: Hiba Rezek 

| | Date:   Tue Sep 23 08:47:36 2025 +0300

| |

| |     added data to data.txt

| |

| \* commit 840598657c433a89d8e5331a5ce535df720d4edd

| | Author: Hiba Rezek 

| | Date:   Tue Sep 23 08:46:56 2025 +0300

| |

| |     modified file 1 for q10 ex2

| |

\* | commit 1732265e70b32ed9a77a868b8ed05d9d62dd74c9

|/  Author: Hiba Rezek 



STRETCH TASK

1.PS C:\\Users\\hibam\\Desktop\\gitlab> git log -3

commit 8771fb30b90a86b9283c18179f8f4b55b50d7213 (HEAD -> my\_first\_branch)

Author: Hiba Rezek 

Date:   Tue Sep 23 08:58:47 2025 +0300



&nbsp;   added print statement for newnamef2.py



commit 9be0de0f3201370974acff1b8f48186b06c6bce4

Author: Hiba Rezek 

Date:   Tue Sep 23 08:58:17 2025 +0300



&nbsp;   added more content



2.did some modifications

3\. PS C:\\Users\\hibam\\Desktop\\gitlab> git merge my\_first\_branch -m "merge stretch task ex 2 q1"

Auto-merging data.txt

CONFLICT (content): Merge conflict in data.txt

Auto-merging src/newnamef2.py

CONFLICT (content): Merge conflict in src/newnamef2.py

Automatic merge failed; fix conflicts and then commit the result.



4\. PS C:\\Users\\hibam\\Desktop\\gitlab> git status

On branch master

You have unmerged paths.

&nbsp; (fix conflicts and run "git commit")

&nbsp; (use "git merge --abort" to abort the merge)



Unmerged paths:

&nbsp; (use "git add <file>..." to mark resolution)

&nbsp;       both modified:   data.txt

&nbsp;       both modified:   src/newnamef2.py



5,6,7,8. done via vscode





------------------------------------------------------

ex3



1.PS C:\\Users\\hibam\\Desktop\\gitlab> git branch undoing\_changes



2.PS C:\\Users\\hibam\\Desktop\\gitlab> git checkout undoing\_changes

Switched to branch 'undoing\_changes'



3\. since i already have a file 3, ill create f3.py



4.PS C:\\Users\\hibam\\Desktop\\gitlab> git commit -m "created f3.py (i already have a file3.py)"

\[undoing\_changes ff59b40] created f3.py (i already have a file3.py)

&nbsp;1 file changed, 1 insertion(+)

&nbsp;create mode 100644 src/f3.py



5.PS C:\\Users\\hibam\\Desktop\\gitlab> git diff

diff --git a/src/f3.py b/src/f3.py

index f21a68a..ef929fc 100644

--- a/src/f3.py

+++ b/src/f3.py

@@ -1 +1,2 @@

-#this is file3.py of q3 ex3

\\ No newline at end of file

+#this is file3.py of q3 ex3

+#new line in f3.py :)

\\ No newline at end of file



6.PS C:\\Users\\hibam\\Desktop\\gitlab> git checkout master

error: Your local changes to the following files would be overwritten by checkout:

&nbsp;       src/f3.py

Please commit your changes or stash them before you switch branches.

Aborting



PS C:\\Users\\hibam\\Desktop\\gitlab> git checkout -f master

Switched to branch 'master'

b.PS C:\\Users\\hibam\\Desktop\\gitlab> git status

On branch master

nothing to commit, working tree clean



changes are lost.

c. from git status message earlier:

(use "git restore <file>..." to discard changes in working directory)

&nbsp;       modified:   src/f3.py



if we yse git restore src/f3.py we will lose f3



7.done using vscode gui



8\.    resolving conflicts

PS C:\\Users\\hibam\\Desktop\\gitlab> git revert 6695a

fatal: cannot lock ref 'HEAD': is at 0bfbf6a691ecccb669b71b03570c1255027704f1 but expected 6695a2aed0658e02856037379e7a27e20769c6c4

PS C:\\Users\\hibam\\Desktop\\gitlab> git status

On branch master

nothing to commit, working tree clean

PS C:\\Users\\hibam\\Desktop\\gitlab> git log -2

commit 0bfbf6a691ecccb669b71b03570c1255027704f1 (HEAD -> master)

Author: Hiba Rezek 

Date:   Tue Sep 23 09:39:58 2025 +0300



&nbsp;   Revert "created file4.py"



&nbsp;   This reverts commit 6695a2aed0658e02856037379e7a27e20769c6c4.

a.revert makes a new commit that undoes the changes of a commit, while maintaining history

checkout switches to another branch or commit and it discards changes in a file like what happened earlier.



b.PS C:\\Users\\hibam\\Desktop\\gitlab> git log -2

commit 0bfbf6a691ecccb669b71b03570c1255027704f1 (HEAD -> master)

Author: Hiba Rezek 

Date:   Tue Sep 23 09:39:58 2025 +0300



&nbsp;   Revert "created file4.py"



&nbsp;   This reverts commit 6695a2aed0658e02856037379e7a27e20769c6c4.



commit 6695a2aed0658e02856037379e7a27e20769c6c4

Author: Hiba Rezek 

Date:   Tue Sep 23 09:38:12 2025 +0300



&nbsp;   created file4.py



c.the new commit literally undoes the one before it. it deleted the created file in previous commit.



9.done using vscode gui



10.PS C:\\Users\\hibam\\Desktop\\gitlab> git reset --soft HEAD^

PS C:\\Users\\hibam\\Desktop\\gitlab> git status

On branch master

Changes to be committed:

&nbsp; (use "git restore --staged <file>..." to unstage)

&nbsp;       new file:   src/file4.py



**b.the last commit is undone and the changes from this last commit are now in staging area.**



c. PS C:\\Users\\hibam\\Desktop\\gitlab> git log -3

commit 3febe33ef94fc70d52660357a7e7ab112a1eae61 (HEAD -> master)

Author: Hiba Rezek 

Date:   Tue Sep 23 09:47:24 2025 +0300



&nbsp;   add f3.py with initial content



commit 0bfbf6a691ecccb669b71b03570c1255027704f1

Author: Hiba Rezek 

Date:   Tue Sep 23 09:39:58 2025 +0300



&nbsp;   Revert "created file4.py"



&nbsp;   This reverts commit 6695a2aed0658e02856037379e7a27e20769c6c4.



commit 6695a2aed0658e02856037379e7a27e20769c6c4

Author: Hiba Rezek 

Date:   Tue Sep 23 09:38:12 2025 +0300



&nbsp;   created file4.py



**no, the previous commit is no longer there**



d. **using soft, the changes aren't lost and they are in staging area.**

**we can use git stash to take uncommitted changes (both staged and unstaged) and save them on a stack.this way we wont lose our work**



 **if we still want to make sure we can create a tag so that we can go back to it after resetting.**



11\. a.PS C:\\Users\\hibam\\Desktop\\gitlab> git reset HEAD

PS C:\\Users\\hibam\\Desktop\\gitlab> git status

On branch master

nothing to commit, working tree clean



**nothing changes because we dont have anything in staging area.if we have staged files it will unstage them but theyll still be in working directory.** 

**b. head is where the current pointer is, head^ is the parent commit. since we want to unstage changes in current commit we use head.**

**c. by default it is --mixed. Mixed moves the branch pointer to the specified commit.it resets the staging area (index) to match that commit. it does NOT touch working directory; changes remain as uncommitted edits.**





12.PS C:\\Users\\hibam\\Desktop\\gitlab>  git reset --hard

HEAD is now at 233bb17 update file4.py comment for clarity

a. working directory and history are both lost. 

b. it used the last commit where the head is.

c. it would have removed all changes from this commit and the staged and unstaged changes are lost



13.PS C:\\Users\\hibam\\Desktop\\gitlab> git log -5

commit 233bb1755950ce3cc5c4d0721fa3fd0cd61eafac (HEAD -> master)

Author: Hiba Rezek 

Date:   Tue Sep 23 10:05:33 2025 +0300



&nbsp;   update file4.py comment for clarity



commit 9417d80d1a8bbc071d889b5897ba182c1148b388

Author: Hiba Rezek 

Date:   Tue Sep 23 09:56:42 2025 +0300



&nbsp;   create file4.py with initial content



commit 3febe33ef94fc70d52660357a7e7ab112a1eae61

Author: Hiba Rezek 

Date:   Tue Sep 23 09:47:24 2025 +0300



&nbsp;   add f3.py with initial content



commit 0bfbf6a691ecccb669b71b03570c1255027704f1

Author: Hiba Rezek 

Date:   Tue Sep 23 09:39:58 2025 +0300



&nbsp;   Revert "created file4.py"



&nbsp;   This reverts commit 6695a2aed0658e02856037379e7a27e20769c6c4.



commit 6695a2aed0658e02856037379e7a27e20769c6c4

Author: Hiba Rezek 

Date:   Tue Sep 23 09:38:12 2025 +0300





14.PS C:\\Users\\hibam\\Desktop\\gitlab> git log -5

commit aaaf8267560b9a19576f292b812abb8e70c86829 (HEAD -> master)

Author: Hiba Rezek 

Date:   Tue Sep 23 10:15:37 2025 +0300



&nbsp;   added comment to f3



commit c068fe2950690c525e9fbf89916d98c2a79c6d5b

Author: Hiba Rezek 

Date:   Tue Sep 23 10:14:54 2025 +0300



&nbsp;   add additional content to file4.py



commit 064f06d5c57ddba1b7c9c605b56530c87e414888

Author: Hiba Rezek 

Date:   Tue Sep 23 10:14:32 2025 +0300



&nbsp;   content for file5



commit 92e72274e6bdb15487f937b6bcb132fd5ef16e54

Author: Hiba Rezek 

Date:   Tue Sep 23 10:14:01 2025 +0300



&nbsp;   created  file5.py



commit 233bb1755950ce3cc5c4d0721fa3fd0cd61eafac

Author: Hiba Rezek 

Date:   Tue Sep 23 10:05:33 2025 +0300



&nbsp;   update file4.py comment for clarity



--------------------------------------------------------



EX4



1.PS C:\\Users\\hibam\\Desktop\\gitlab> git checkout -b feature-branch

Switched to a new branch 'feature-branch'



2.done via gui



3.PS C:\\Users\\hibam\\Desktop\\gitlab> git checkout master

Switched to branch 'master'



4.done via gui



5.history:

PS C:\\Users\\hibam\\Desktop\\gitlab> git log --oneline --graph --branches

\* 9d108ab (HEAD -> master) created main file + contents

| \* 3dcf9c5 (feature-branch) feature 1 and some contents

|/

\* aaaf826 added comment to f3

\* c068fe2 add additional content to file4.py

\* 064f06d content for file5

\* 92e7227 created  file5.py

\* 233bb17 update file4.py comment for clarity

\* 9417d80 create file4.py with initial content

\* 3febe33 add f3.py with initial content

\* 0bfbf6a Revert "created file4.py"

\* 6695a2a created file4.py

| \* ff59b40 (undoing\_changes) created f3.py (i already have a file3.py)

|/

\*   11cab3f resolving conflicts

|\\

| \* 8771fb3 (my\_first\_branch) added print statement for newnamef2.py

| \* 9be0de0 added more content

\* | ab7223e added additional information to data.txt and updated print statements in file1.py and newnamef2.py to reflect branch context

\* | 4aee6aa Merge branch 'my\_first\_branch' -m "merge q11"

|\\|

| \* eb73bfb added content to file3

| \* 0c9358d added data to data.txt

| \* 8405986 modified file 1 for q10 ex2

\* | 1732265 modifiied newnamef2.py

|/

\* 18258ef adding data to data.txt

\* c995dfa created data.txt

\* 13a29b3 renamed file 2

\* 060e26c renamed file2.py using system

\* 557eaa8 moved file3 into src

\* 1ed5b0d add file3.py

\* 61d01e0 deleted data.txt

\* 597adff added data.txt in src

\* 73bc144 changes for file 2

\* 11fa249 changes for file 1

\* fee3af1 added src folder

\* c68a95a readme file created





6\.

&nbsp;	a.PS C:\\Users\\hibam\\Desktop\\gitlab> git rebase master

&nbsp;	Successfully rebased and updated refs/heads/feature-branch.

what actually happened:
we're on feature-branch, we take all commits on feature branch that are not in master and we add them to latest version of master. the base branch is master, since commits will be appended to it starting from latest commit of master.





&nbsp;	

&nbsp;	b.PS C:\\Users\\hibam\\Desktop\\gitlab> git status

On branch feature-branch

nothing to commit, working tree clean



PS C:\\Users\\hibam\\Desktop\\gitlab> git log --oneline --graph --branches

\* 79cb4e0 (HEAD -> feature-branch) feature 1 and some contents

\* 9d108ab (master) created main file + contents

\* aaaf826 added comment to f3

\* c068fe2 add additional content to file4.py

\* 064f06d content for file5

\* 92e7227 created  file5.py

\* 233bb17 update file4.py comment for clarity

\* 9417d80 create file4.py with initial content

\* 3febe33 add f3.py with initial content

\* 0bfbf6a Revert "created file4.py"

\* 6695a2a created file4.py



c.the main branch's commits are no longer visible, also we dont have any history of the rebase. the tree is linear



d.rebase rewrites feature branch’s history to make it appear as if it was built directly on main, while merge keeps both histories intact and explicitly marks the merge point. files that didn't exist on the base branch will not be added after rebase.



7.PS C:\\Users\\hibam\\Desktop\\gitlab> git rebase master

warning: skipped previously applied commit 79cb4e0

hint: use --reapply-cherry-picks to include skipped commits

hint: Disable this message with "git config set advice.skippedCherryPicks false"

Auto-merging feature1.py

CONFLICT (content): Merge conflict in feature1.py

error: could not apply d0ca0dd... modification for ex4 q7c

hint: Resolve all conflicts manually, mark them as resolved with

hint: "git add/rm <conflicted\_files>", then run "git rebase --continue".

hint: You can instead skip this commit: run "git rebase --skip".

hint: To abort and get back to the state before "git rebase", run "git rebase --abort".

hint: Disable this message with "git config set advice.mergeConflict false"

Could not apply d0ca0dd... # modification for ex4 q7c



d.PS C:\\Users\\hibam\\Desktop\\gitlab> git status

interactive rebase in progress; onto f296de8

Last command done (1 command done):

&nbsp;  pick d0ca0dd # modification for ex4 q7c

No commands remaining.

You are currently rebasing branch 'feature-branch' on 'f296de8'.

&nbsp; (fix conflicts and then run "git rebase --continue")

&nbsp; (use "git rebase --skip" to skip this patch)

&nbsp; (use "git rebase --abort" to check out the original branch)



Unmerged paths:

&nbsp; (use "git restore --staged <file>..." to unstage)

&nbsp; (use "git add <file>..." to mark resolution)

&nbsp;       both modified:   feature1.py



no changes added to commit (use "git add" and/or "git commit -a")



9.PS C:\\Users\\hibam\\Desktop\\gitlab> git log --oneline --graph --branches

\* 3a22c85 (HEAD -> feature-branch) modification for ex4 q7c

\* f296de8 (master) modification for q7b

\* 72ae9f5 feature 1 and some contents

\* 9d108ab created main file + contents

\* aaaf826 added comment to f3

\* c068fe2 add additional content to file4.py

\* 064f06d content for file5

\* 92e7227 created  file5.py

\* 233bb17 update file4.py comment for clarity

\* 9417d80 create file4.py with initial content

\* 3febe33 add f3.py with initial content

\* 0bfbf6a Revert "created file4.py"

\* 6695a2a created file4.py

| \* ff59b40 (undoing\_changes) created f3.py (i already have a file3.py)

|/

\*   11cab3f resolving conflicts

|\\

| \* 8771fb3 (my\_first\_branch) added print statement for newnamef2.py

| \* 9be0de0 added more content

\* | ab7223e added additional information to data.txt and updated print statements in file1.py and newnamef2.py to reflect branch context

\* | 4aee6aa Merge branch 'my\_first\_branch' -m "merge q11"

|\\|

| \* eb73bfb added content to file3

| \* 0c9358d added data to data.txt

| \* 8405986 modified file 1 for q10 ex2



b.the branches look combines because the feature branch now starts after master’s latest commit, not because of a merge.

c. after rebasing feature-branch onto master, the graph became linear . feature-branch now appears as if it started from the tip of master.



If we had merged instead, we would see a branch + merge commit connecting master and feature-branch in the graph.

10. done using gui
11.a.
b. Squashing takes multiple commits and combines them into a single commit, rewriting history so it looks like you made one clean change instead of many smaller steps.
c.done using gui
d. To amend an old commit during a rebase, start an interactive rebase going back to the commit you want to edit (git rebase -i HEAD~N). When the editor opens, mark the target commit with edit instead of pick and save. Git will pause at that commit, allowing you to make changes (edit your files as needed, then stage them with git add <file>). Once staged, amend the commit (git commit --amend) to update its content or message. After that, continue the rebase (git rebase --continue). If conflicts arise, resolve them in the files, stage the fixes (git add <file>), and run git rebase --continue again. Finally, if the branch has already been pushed to a remote, you’ll need to force push your changes (git push origin branch-name --force).

12.PS C:\\Users\\hibam\\Desktop\\gitlab> git log --oneline --graph --branches

\* 4784702 (master) mod file 5

\* ef4a362 mod main

| \* 497bce8 (HEAD -> feature-branch) modifications for main

| \* a84993a modifications for file4 again

| \* 3a22c85 modification for ex4 q7c

|/

\* f296de8 modification for q7b

\* 72ae9f5 feature 1 and some contents

\* 9d108ab created main file + contents

\* aaaf826 added comment to f3

\* c068fe2 add additional content to file4.py

\* 064f06d content for file5

\* 92e7227 created  file5.py

\* 233bb17 update file4.py comment for clarity


1.Use git status to see which branch you are on.
$ git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean

2.What does git log look like?
$ git log
commit 219d535e4faf19afcec23c2f9b3247883b4b031f (HEAD -> master, origin/master, origin/HEAD)
Author: Nha Vuong <46470817+nhavuong@users.noreply.github.com>
Date:   Fri Jan 24 18:35:23 2020 -0800

    Rename greeting.txt to 3-way-merge/greeting.txt

commit 232a3f6c86b9c36643917bc0d5453cc737be53b7
Author: Nha Vuong <46470817+nhavuong@users.noreply.github.com>
Date:   Fri Jan 24 18:34:47 2020 -0800

    Rename README.md to 3-way-merge/README.md

commit 8a57494f2a5b30ba6a4fe0ec7009636790c26908
Merge: fa565ea 9c77862
Author: Nha Vuong <vtnha.cseiu@gmail.com>
Date:   Fri Jan 24 18:01:03 2020 -0800

    Merge branch 'greeting'

commit fa565ea91fdd288fa20543a46eec8659a3f448e5
Author: Nha Vuong <vtnha.cseiu@gmail.com>
Date:   Fri Jan 24 17:59:05 2020 -0800

    create README.md

commit 9c778629abb21a24f7b6723452a68fa6f1347255
Author: Nha Vuong <vtnha.cseiu@gmail.com>
Date:   Fri Jan 24 17:57:18 2020 -0800

    change greeting.txt

commit ca1a398e867c1657bd9b89acf43262d65df93634
Author: Nha Vuong <vtnha.cseiu@gmail.com>
Date:   Fri Jan 24 17:55:27 2020 -0800

    Add content to greeting.txt

commit 77822cbae56c3e3eb7ffe083b23ed7303ae4d4e9
Author: Nha Vuong <vtnha.cseiu@gmail.com>
Date:   Fri Jan 24 17:54:27 2020 -0800

    Add file greeting.txt

3.Create a file
$ touch example.txt

4.What does the output from git status look like now?
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        ./

nothing added to commit but untracked files present (use "git add" to track)

5.add the file to the staging area
6.How does git status look now?
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   README.md
        new file:   example.txt


7.commit the file to the repository
8.How does git status look now?
$ git status
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

9.Change the content of the file you created earlier
10.What does git status look like now?
$ git status
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   example.txt

no changes added to commit (use "git add" and/or "git commit -a")


11.add the file change
12.What does git status look like now?
$ git status
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   example.txt

13.Change the file again
14.Make a commit
15.What does the status look like now?
$ git status
On branch master
Your branch is ahead of 'origin/master' by 2 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   example.txt

no changes added to commit (use "git add" and/or "git commit -a")


 The log?
$ git log
commit 86a19081bb4b27894d4dc3330320c43ac8b3db87 (HEAD -> master)
Author: Nha Vuong <vtnha.cseiu@gmail.com>
Date:   Fri Jan 24 18:59:23 2020 -0800

    change without add .

commit eebbc52a6c5da8788ba28d46997687ffb70b2c6c
Author: Nha Vuong <vtnha.cseiu@gmail.com>
Date:   Fri Jan 24 18:56:34 2020 -0800

    change

commit 219d535e4faf19afcec23c2f9b3247883b4b031f (origin/master, origin/HEAD)
Author: Nha Vuong <46470817+nhavuong@users.noreply.github.com>
Date:   Fri Jan 24 18:35:23 2020 -0800

    Rename greeting.txt to 3-way-merge/greeting.txt

commit 232a3f6c86b9c36643917bc0d5453cc737be53b7
Author: Nha Vuong <46470817+nhavuong@users.noreply.github.com>
Date:   Fri Jan 24 18:34:47 2020 -0800

    Rename README.md to 3-way-merge/README.md

commit 8a57494f2a5b30ba6a4fe0ec7009636790c26908
Merge: fa565ea 9c77862
Author: Nha Vuong <vtnha.cseiu@gmail.com>
Date:   Fri Jan 24 18:01:03 2020 -0800

    Merge branch 'greeting'

commit fa565ea91fdd288fa20543a46eec8659a3f448e5
Author: Nha Vuong <vtnha.cseiu@gmail.com>
Date:   Fri Jan 24 17:59:05 2020 -0800

    create README.md

commit 9c778629abb21a24f7b6723452a68fa6f1347255
Author: Nha Vuong <vtnha.cseiu@gmail.com>
Date:   Fri Jan 24 17:57:18 2020 -0800

    change greeting.txt

commit ca1a398e867c1657bd9b89acf43262d65df93634
Author: Nha Vuong <vtnha.cseiu@gmail.com>
Date:   Fri Jan 24 17:55:27 2020 -0800

    Add content to greeting.txt


16.Commit the newest change
$ git status
On branch master
Your branch is ahead of 'origin/master' by 3 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

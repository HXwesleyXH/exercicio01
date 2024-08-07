# Continuous Integration and Continuous Delivery
## 2024 - MBA CLC & DevOps_12
### EXERCICIO 01 - ENTREGA
#
```
echo 01 > arquivo.txt
```

```
git add -A
```

```
git status
```
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   arquivo.txt

```
git commit -m "git add example -arquivo.txt"
```
[main d4c68a4] git add example -arquivo.txt
 1 file changed, 1 insertion(+)
 create mode 100644 arquivo.txt

```
git status
```
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

```
git log
```
commit d4c68a49ba4395491455810f49d414ddb02b4dca (HEAD -> main)
Author: HXwesleyXH <HXwesleyXH@hotmail.com>
Date:   Tue Aug 6 22:01:22 2024 -0300

    git add example -arquivo.txt

commit ae1228f4ebd2fc40d3fdd3d39f6df4d5b8886f7a (origin/main, origin/HEAD)
Author: Wesley Martins Rodrigues <53615747+HXwesleyXH@users.noreply.github.com>
Date:   Tue Aug 6 20:23:40 2024 -0300
    Initial commit

```
echo 02 > arquivo.txt
```

```
git diff
```

diff --git a/arquivo.txt b/arquivo.txt
index 8a0f05e..9e22bcb 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-01
+02

```
git add -A
```

```
git status
```
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt

```
echo 03 > arquivo.txt
```

```
git diff
```
diff --git a/arquivo.txt b/arquivo.txt
index 9e22bcb..75016ea 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-02
+03

```
git restore .
```

```
git status
```
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt

```
git commit -m "novo commit"
```
[main 4c2ca72] novo commit
 1 file changed, 1 insertion(+), 1 deletion(-)

```
git log
```
commit 4c2ca72cfc795674854778ddd312516928c3e1f8 (HEAD -> main)
Author: HXwesleyXH <HXwesleyXH@hotmail.com>
Date:   Tue Aug 6 22:08:55 2024 -0300

    novo commit

commit d4c68a49ba4395491455810f49d414ddb02b4dca
Author: HXwesleyXH <HXwesleyXH@hotmail.com>
Date:   Tue Aug 6 22:01:22 2024 -0300

    git add example -arquivo.txt

commit ae1228f4ebd2fc40d3fdd3d39f6df4d5b8886f7a (origin/main, origin/HEAD)
Author: Wesley Martins Rodrigues <53615747+HXwesleyXH@users.noreply.github.com>
:...skipping...
commit 4c2ca72cfc795674854778ddd312516928c3e1f8 (HEAD -> main)
Author: HXwesleyXH <HXwesleyXH@hotmail.com>
Date:   Tue Aug 6 22:08:55 2024 -0300

    novo commit

commit d4c68a49ba4395491455810f49d414ddb02b4dca
Author: HXwesleyXH <HXwesleyXH@hotmail.com>
Date:   Tue Aug 6 22:01:22 2024 -0300

    git add example -arquivo.txt

commit ae1228f4ebd2fc40d3fdd3d39f6df4d5b8886f7a (origin/main, origin/HEAD)
Author: Wesley Martins Rodrigues <53615747+HXwesleyXH@users.noreply.github.com>
Date:   Tue Aug 6 20:23:40 2024 -0300
:...skipping...
commit 4c2ca72cfc795674854778ddd312516928c3e1f8 (HEAD -> main)
Author: HXwesleyXH <HXwesleyXH@hotmail.com>
Date:   Tue Aug 6 22:08:55 2024 -0300

    novo commit

commit d4c68a49ba4395491455810f49d414ddb02b4dca
Author: HXwesleyXH <HXwesleyXH@hotmail.com>
Date:   Tue Aug 6 22:01:22 2024 -0300

    git add example -arquivo.txt

commit ae1228f4ebd2fc40d3fdd3d39f6df4d5b8886f7a (origin/main, origin/HEAD)
Author: Wesley Martins Rodrigues <53615747+HXwesleyXH@users.noreply.github.com>
Date:   Tue Aug 6 20:23:40 2024 -0300

    Initial commit

```
echo > .gitignore
```

```
nano .gitgnore
```

```
git status
```
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   .gitignore

no changes added to commit (use "git add" and/or "git commit -a")

```
echo > novo.txt
```

```
git status
```
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   .gitignore

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        novo.txt

no changes added to commit (use "git add" and/or "git commit -a")
# Avaliação
Avaliação. Faça um merge e um rebase no repositório git_test.


Avaliação.

Faça um merge e um rebase no
repositório git_test




C:\Avaliação\github>git init
Initialized empty Git repository in C:/Avaliação/github/.git/

C:\Avaliação\github>git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        olaMundo.txt

nothing added to commit but untracked files present (use "git add" to track)

C:\Avaliação\github>git add olamundo.txt

C:\Avaliação\github>git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        olaMundo.txt

nothing added to commit but untracked files present (use "git add" to track)

C:\Avaliação\github>git add olamundo.txt

C:\Avaliação\github>git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        olaMundo.txt

nothing added to commit but untracked files present (use "git add" to track)

C:\Avaliação\github>git add olaMundo.txt

C:\Avaliação\github>git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   olaMundo.txt


C:\Avaliação\github>git commit -m "Adicionei meu nome completo"
[master (root-commit) 066a6d3] Adicionei meu nome completo
 1 file changed, 1 insertion(+)
 create mode 100644 olaMundo.txt

C:\Avaliação\github>git branch merge

C:\Avaliação\github>git checkout merge
Switched to branch 'merge'

C:\Avaliação\github>git branch
  master
* merge

C:\Avaliação\github>git status
On branch merge
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   olaMundo.txt

no changes added to commit (use "git add" and/or "git commit -a")

C:\Avaliação\github>git add olaMundo.txt

C:\Avaliação\github>git status
On branch merge
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   olaMundo.txt


C:\Avaliação\github>git commit -am "Vou fazer o merge"
[merge 71a1abf] Vou fazer o merge
 1 file changed, 2 insertions(+), 1 deletion(-)

C:\Avaliação\github>git status
On branch merge
nothing to commit, working tree clean

C:\Avaliação\github>git log
commit 71a1abfce5586d511b20f5461b344bb36ac561fc (HEAD -> merge)
Author: Fernando Marques <fernandotakeshi47@gmail.com>
Date:   Wed Aug 17 16:03:19 2022 -0400

    Vou fazer o merge

commit 066a6d35d936b66d768f186d4aeb4f8eb219e94c (master)
Author: Fernando Marques <fernandotakeshi47@gmail.com>
Date:   Wed Aug 17 16:00:54 2022 -0400

    Adicionei meu nome completo

C:\Avaliação\github>git checkout master
Switched to branch 'master'

C:\Avaliação\github>git branch
* master
  merge

C:\Avaliação\github>git merge merge
Updating 066a6d3..71a1abf
Fast-forward
 olaMundo.txt | 3 ++-
 1 file changed, 2 insertions(+), 1 deletion(-)

C:\Avaliação\github>git branch
* master
  merge

C:\Avaliação\github>git branch rebase

C:\Avaliação\github>git status
On branch master
nothing to commit, working tree clean

C:\Avaliação\github>git checkout rebase
Switched to branch 'rebase'

C:\Avaliação\github>git branch
  master
  merge
* rebase

C:\Avaliação\github>git add olaMundo.txt

C:\Avaliação\github>git status
On branch rebase
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   olaMundo.txt


C:\Avaliação\github>git commit -am "Editei o uma frase"
[rebase d91e6d6] Editei o uma frase
 1 file changed, 2 insertions(+), 1 deletion(-)

C:\Avaliação\github>git branch
  master
  merge
* rebase

C:\Avaliação\github>git checkaut master
git: 'checkaut' is not a git command. See 'git --help'.

The most similar command is
        checkout

C:\Avaliação\github>git branch master
fatal: a branch named 'master' already exists

C:\Avaliação\github>git rebase rebase
Current branch rebase is up to date.

C:\Avaliação\github>git branch
  master
  merge
* rebase

C:\Avaliação\github>git checkout master
Switched to branch 'master'

C:\Avaliação\github>git branch
* master
  merge
  rebase

C:\Avaliação\github>git rebase rebase
Successfully rebased and updated refs/heads/master.

C:\Avaliação\github>
# ejercicio-git-libro

## Clonacion del repositorio ##

````
Usuario@DESKTOP-5OONOR5 MINGW64 ~/Documents/tarea_ciclo/ets (main|MERGING)
$ git clone https://github.com/habccode/ejercicio-git-libro.git
Cloning into 'ejercicio-git-libro'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.

Usuario@DESKTOP-5OONOR5 MINGW64 ~/Documents/tarea_ciclo/ets (main|MERGING)
$ ls
Github/  ejercicio-git-branch/  ejercicio-git-libro/

Usuario@DESKTOP-5OONOR5 MINGW64 ~/Documents/tarea_ciclo/ets (main|MERGING)
$ ls -la
total 8
drwxr-xr-x 1 Usuario 197121 0 Oct 23 00:56 ./
drwxr-xr-x 1 Usuario 197121 0 Oct 22 23:05 ../
drwxr-xr-x 1 Usuario 197121 0 Oct 22 23:07 Github/
drwxr-xr-x 1 Usuario 197121 0 Oct 23 00:08 ejercicio-git-branch/
drwxr-xr-x 1 Usuario 197121 0 Oct 23 00:56 ejercicio-git-libro/

Usuario@DESKTOP-5OONOR5 MINGW64 ~/Documents/tarea_ciclo/ets (main|MERGING)
$ code .

Usuario@DESKTOP-5OONOR5 MINGW64 ~/Documents/tarea_ciclo/ets (main|MERGING)
$



````

## Usando Comandos Log ##

````
$ git log
commit dd0ae7462af2bb6e0223e7db94fe28707c3807f2 (HEAD -> main, origin/ejercicio1-branch, ejercicio1-branch)
Author: habccode <armandocarrillo211194@gmail.com>
Date:   Sat Oct 5 16:19:09 2024 +0200

    first commit

commit f98508091f130efc153a17a25fe104d2b785570f
Author: habccode <armandocarrillo211194@gmail.com>
Date:   Sat Oct 5 15:32:35 2024 +0200

    primer commit

commit 33301ed9bca31af322ba7e1bb4438533897292dd
Author: habccode <armandocarrillo211194@gmail.com>
Date:   Sat Oct 5 15:29:45 2024 +0200

    Esperando el Primero

commit d1832fed33fb9ea58bfa923026d4800aa7ef7836
Author: armando <armandocarrillo211194@gmail.com>
Date:   Wed Oct 2 01:44:05 2024 +0200

    segundo commit: README

commit 1eb73e438c2fccf89c56f873db962aeae1e9b594
Author: armando <armandocarrillo211194@gmail.com>
Date:   Wed Oct 2 01:28:20 2024 +0200

    Primer commit: Añadir README

commit 6658a700623f1ad317c86ae4a87016b7362034ee
Author: armando <armandocarrillo211194@gmail.com>
Date:   Wed Oct 2 00:46:02 2024 +0200

    primer commit

Usuario@DESKTOP-5OONOR5 MINGW64 ~/Documents/tarea_ciclo/ets (main|MERGING)
````


## Usando git log --oneline --graph##

````
Usuario@DESKTOP-5OONOR5 MINGW64 ~/Documents/tarea_ciclo/ets (main|MERGING)
$ git log --oneline --graph
* dd0ae74 (HEAD -> main, origin/ejercicio1-branch, ejercicio1-branch) first commit
* f985080 primer commit
* 33301ed Esperando el Primero
* d1832fe segundo commit: README
* 1eb73e4 Primer commit: Añadir README
* 6658a70 primer commit

Usuario@DESKTOP-5OONOR5 MINGW64 ~/Documents/tarea_ciclo/ets (main|MERGING)
$


````

### Usando	git log --oneline --stat#
````
Usuario@DESKTOP-5OONOR5 MINGW64 ~/Documents/tarea_ciclo/ets (main|MERGING)
$ git log --oneline --stat
dd0ae74 (HEAD -> main, origin/ejercicio1-branch, ejercicio1-branch) first commit
 README.md | 1 +
 1 file changed, 1 insertion(+)
f985080 primer commit
 README.md | 1 +
 1 file changed, 1 insertion(+)
33301ed Esperando el Primero
 README.md | 2 ++
 1 file changed, 2 insertions(+)
d1832fe segundo commit: README
 trs-ejercicios | 1 +
 1 file changed, 1 insertion(+)
1eb73e4 Primer commit: Añadir README
 README.md | 2 ++
 1 file changed, 2 insertions(+)
6658a70 primer commit
 README.md | 1 +
 1 file changed, 1 insertion(+)


````

## Carpetas Capitulos##
````
Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro (main)
$ "Git es un sistema de control de versiones ideado por Linus Torvalds."
bash: Git es un sistema de control de versiones ideado por Linus Torvalds.: command not found

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro (main)
$ cat > capitulos/capitulo1.txt
Git es un sistema de control de versiones ideado por Linus Torvalds.

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro (main)
$ git add .
warning: in the working copy of 'capitulos/capitulo1.txt', LF will be replaced by CRLF the next time Git touches it

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro (main)
$ git add .

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro (main)
$ git commit -m"Añadido Capitulo 1."
[main f382d42] Añadido Capitulo 1.
 2 files changed, 125 insertions(+), 1 deletion(-)
 create mode 100644 capitulos/capitulo1.txt

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro (main)
$ git log
commit f382d42db8dd33d53f1e5a62e2c44bde05d78762 (HEAD -> main)
Author: habccode <armandocarrillo211194@gmail.com>
Date:   Wed Oct 23 01:32:37 2024 +0200

    Añadido Capitulo 1.

commit c31f1019211ab853bdb7065b60d3037a3f944539 (origin/main, origin/HEAD)
Author: harby <armandocarrillo211194@gmail.com>
Date:   Wed Oct 23 01:54:58 2024 +0200

    Initial commit

````

## Cambio en el head##

````
$ git add .
git commit -m "Añadido capítulo 2."
git diff HEAD~2..HEAD
fatal: Unable to create 'C:/Users/Usuario/.git/index.lock': File exists.

Another git process seems to be running in this repository, e.g.
an editor opened by 'git commit'. Please make sure all processes
are terminated then try again. If it still fails, a git process
may have crashed in this repository earlier:
remove the file manually to continue.
fatal: Unable to create 'C:/Users/Usuario/.git/index.lock': File exists.

Another git process seems to be running in this repository, e.g.
an editor opened by 'git commit'. Please make sure all processes
are terminated then try again. If it still fails, a git process
may have crashed in this repository earlier:
remove the file manually to continue.
diff --git a/README.md b/README.md
index 1924ac8..2d12f0f 100644
--- a/README.md
+++ b/README.md
@@ -3,3 +3,5 @@
 · git
 # proyectoets1
 # ejercicio4
+# ejercicio4
+# ejercicio4

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets (ejercicio-branch2)
$


````

## Capitulo 3##
````
Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (main)
$ cat > capitulo3.txt
Git permite la creación de ramas lo que permite tener distintas versiones del mismo proyecto y trabajar de manera simultanea en ellas.

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (main)
$ git add .
git commit -m "Añadido capítulo 3."
git log
 git diff <codigo hash de la primera version>..HEAD
warning: in the working copy of 'capitulos/capitulo3.txt', LF will be replaced by CRLF the next time Git touches it
[main 6917f4c] Añadido capítulo 3.
 1 file changed, 1 insertion(+)
 create mode 100644 capitulos/capitulo3.txt
commit 6917f4c68c9918f2f9638e342f06ac4f34736bb1 (HEAD -> main)
Author: habccode <armandocarrillo211194@gmail.com>
Date:   Wed Oct 23 01:49:13 2024 +0200

    Añadido capítulo 3.

commit a8c05fd5051d4816db6097e12972e8efdaa89cc2
Author: habccode <armandocarrillo211194@gmail.com>
Date:   Wed Oct 23 01:44:35 2024 +0200

    Añadido capítulo 2.

commit f382d42db8dd33d53f1e5a62e2c44bde05d78762
Author: habccode <armandocarrillo211194@gmail.com>
Date:   Wed Oct 23 01:32:37 2024 +0200

    Añadido Capitulo 1.

commit c31f1019211ab853bdb7065b60d3037a3f944539 (origin/main, origin/HEAD)
Author: harby <armandocarrillo211194@gmail.com>
Date:   Wed Oct 23 01:54:58 2024 +0200

    Initial commit
bash: codigo: No such file or directory


````
## capitulo 4##
````
Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets (ejercicio-branch2)
$ ls
Github/  ejercicio-git-branch/  ejercicio-git-libro/

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets (ejercicio-branch2)
$ cd ejercicio-git-libro/

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro (main)
$ ls
README.md  capitulos/

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro (main)
$ cd capitulos/

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (main)
$ ls
capitulo1.txt  capitulo2.txt  capitulo3.txt

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (main)
$ cat > índice.txt
Indice de los cápitulos, con conceptos avanzados de git

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (main)
$ git add .

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (main)
$ echo "Indice de los cápitulos, con conceptos avanzados de git" >> indice.txt

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (main)
$ git add .
warning: in the working copy of 'capitulos/indice.txt', LF will be replaced by CRLF the next time Git touches it

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (main)
$ git commit -m"Se crea el indice."
[main e22c3af] Se crea el indice.
 2 files changed, 2 insertions(+)
 create mode 100644 capitulos/indice.txt
 create mode 100644 "capitulos/\303\255ndice.txt"

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (main)
$ git annotate indice.txt
e22c3aff        (  habccode     2024-10-23 02:07:03 +0200       1)Indice de los cápitulos, con conceptos avanzados de git



````

## Capitulo 5##

````
Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (main)
$   git branch bibliografia
  git branch -av
  bibliografia        e22c3af Se crea el indice.
* main                e22c3af [ahead 4] Se crea el indice.
  remotes/origin/HEAD -> origin/main
  remotes/origin/main c31f101 Initial commit

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (main)
$

````

## Capitulo 6

````
Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (main)
$ ls
capitulo1.txt  capitulo2.txt  capitulo3.txt  indice.txt  índice.txt

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (main)
$ cat > capitulo4.txt
  En este capítulo veremos cómo usar GitHub para alojar repositorios en remoto.

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (main)
$ git add .
git commit -m "Añadido capítulo 4."
git log --graph --all --oneline
warning: in the working copy of 'capitulos/capitulo4.txt', LF will be replaced by CRLF the next time Git touches it
[main 05e13af] Añadido capítulo 4.
 1 file changed, 1 insertion(+)
 create mode 100644 capitulos/capitulo4.txt
* 05e13af (HEAD -> main) Añadido capítulo 4.
* e22c3af (bibliografia) Se crea el indice.
* 6917f4c Añadido capítulo 3.
* a8c05fd Añadido capítulo 2.
* f382d42 Añadido Capitulo 1.
* c31f101 (origin/main, origin/HEAD) Initial commit

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (main)
$
````

## Capitulo 7##

````
$ git checkout bibliografia
Switched to branch 'bibliografia'

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (bibliografia)
$ git barnch
git: 'barnch' is not a git command. See 'git --help'.

The most similar command is
        branch

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (bibliografia)
$ git branch
* bibliografia
  main

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (bibliografia)
$ cat > bibliografia.txt
- Chacon, S. and Straub, B. PRO Git. Apress.

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (bibliografia)
$ git add .
git commit -m "Añadida primera referencia bibliográfica."
git log --graph --all --oneline
warning: in the working copy of 'capitulos/bibliografia.txt', LF will be replaced by CRLF the next time Git touches it
[bibliografia 9f28246] Añadida primera referencia bibliográfica.
 1 file changed, 1 insertion(+)
 create mode 100644 capitulos/bibliografia.txt
* 9f28246 (HEAD -> bibliografia) Añadida primera referencia bibliográfica.
| * 05e13af (main) Añadido capítulo 4.
|/
* e22c3af Se crea el indice.
* 6917f4c Añadido capítulo 3.
* a8c05fd Añadido capítulo 2.
* f382d42 Añadido Capitulo 1.
* c31f101 (origin/main, origin/HEAD) Initial commit

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (bibliografia)
$


````

## Capitulo 8##

````Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (bibliografia)
$ git add .
git commit -m "Añadida primera referencia bibliográfica."
git log --graph --all --oneline
warning: in the working copy of 'capitulos/bibliografia.txt', LF will be replaced by CRLF the next time Git touches it
[bibliografia 9f28246] Añadida primera referencia bibliográfica.
 1 file changed, 1 insertion(+)
 create mode 100644 capitulos/bibliografia.txt
* 9f28246 (HEAD -> bibliografia) Añadida primera referencia bibliográfica.
| * 05e13af (main) Añadido capítulo 4.
|/
* e22c3af Se crea el indice.
* 6917f4c Añadido capítulo 3.
* a8c05fd Añadido capítulo 2.
* f382d42 Añadido Capitulo 1.
* c31f101 (origin/main, origin/HEAD) Initial commit

Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (bibliografia)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 5 commits.
Merge made by the 'ort' strategy.
 capitulos/bibliografia.txt | 1 +
 1 file changed, 1 insertion(+) ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (main)
 create mode 100644 capitulos/bibliografia.txt
hint: Waiting for your editor to close the file...
Usuario@DESKTOP-5OONOR5 MINGW64 ~/documents/tarea_ciclo/ets/ejercicio-git-libro/capitulos (main)
$


````

## Capitulo 9##

````


````


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


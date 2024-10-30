# nombre-ejercicio-git-libro

## Clonar repositorio nombre-ejercicio-git-libro

``` code

Bárbara@DESKTOP-6E58R1N MINGW64 ~/Documents/Projects (master)
$ git clone https://github.com/materancode/nombre-ejercicio-git-libro.git
Cloning into 'nombre-ejercicio-git-libro'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.

Bárbara@DESKTOP-6E52R1N MINGW64 ~/Documents/Projects (master)
$ cd Ejercicio-git-libro
bash: cd: Ejercicio-git-libro: No such file or directory

Bárbara@DESKTOP-6E88R1N MINGW64 ~/Documents/Projects (master)
$ ls
Prueba/  nombre-ejercicio-git-libro/  repositorio-ejercicio-1/

Bárbara@DESKTOP-6E85R1N MINGW64 ~/Documents/Projects (master)
$ ls -la
total 16
drwxr-xr-x 1 Bárbara 197121 0 Oct 17 01:46 ./
drwxr-xr-x 1 Bárbara 197121 0 Oct 17 01:37 ../
drwxr-xr-x 1 Bárbara 197121 0 Oct  5 17:53 .git/
drwxr-xr-x 1 Bárbara 197121 0 Oct  5 17:42 Prueba/
drwxr-xr-x 1 Bárbara 197121 0 Oct 17 01:46 nombre-ejercicio-git-libro/
drwxr-xr-x 1 Bárbara 197121 0 Oct  5 17:19 repositorio-ejercicio-1/

Bárbara@DESKTOP-6E85R1N MINGW64 ~/Documents/Projects (master)
$ cd nombre-ejercicio-git-libro/

Bárbara@DESKTOP-6E885R1N MINGW64 ~/Documents/Projects/nombre-ejercicio-git-libro (main)
$ ls -la
total 9
drwxr-xr-x 1 Bárbara 197121  0 Oct 17 01:46 ./
drwxr-xr-x 1 Bárbara 197121  0 Oct 17 01:46 ../
drwxr-xr-x 1 Bárbara 197121  0 Oct 17 01:46 .git/
-rw-r--r-- 1 Bárbara 197121 28 Oct 17 01:46 README.md

Bárbara@DESKTOP-6E88R1N MINGW64 ~/Documents/Projects/nombre-ejercicio-git-libro (main)
$ code .

Bárbara@DESKTOP-6E88R1N MINGW64 ~/Documents/Projects/nombre-ejercicio-git-libro (main)
$


```


## Historial de Cambios "git log"

``` code
Bárbara@DESKTOP-6E338R1N MINGW64 ~/Documents/Projects/nombre-ejercicio-git-libro (main)
$ git log
commit b42210352e211007d782f1b48c73d9a39248d10c (HEAD -> main, origin/main, origin/HEAD)
Author: materancode <materanrolo@gmail.com>
Date:   Mon Oct 14 15:58:35 2024 +0100

    Initial commit

Bárbara@DESKTOP-6E58R1N MINGW64 ~/Documents/Projects/nombre-ejercicio-git-libro (main)
$ ^C

Bárbara@DESKTOP-6E58R1N MINGW64 ~/Documents/Projects/nombre-ejercicio-git-libro (main)
$

Bárbara@DESKTOP-6E58R1N MINGW64 ~/Documents/Projects/nombre-ejercicio-git-libro (main)
$ git log --oneline --graph
* b422103 (HEAD -> main, origin/main, origin/HEAD) Initial commit

Bárbara@DESKTOP-6E58R1N MINGW64 ~/Documents/Projects/nombre-ejercicio-git-libro (main)
$

Bárbara@DESKTOP-6E88R1N MINGW64 ~/Documents/projects/nombre-ejercicio-git-libro (main)
$ cd capitulos

Bárbara@DESKTOP-6E88R1N MINGW64 ~/Documents/projects/nombre-ejercicio-git-libro/capitulos (main)
$ code .

Bárbara@DESKTOP-6E88R1N MINGW64 ~/Documents/projects/nombre-ejercicio-git-libro/capitulos (main)
$ git add .

Bárbara@DESKTOP-6E88R1N MINGW64 ~/Documents/projects/nombre-ejercicio-git-libro/capitulos (main)
$ git commit -m "Se añadio el primer capitulo"
[main aa4d3cd] Se añadio el primer capitulo
 1 file changed, 1 insertion(+)
 create mode 100644 capitulos/capitulo1.txt

Bárbara@DESKTOP-6E88R1N MINGW64 ~/Documents/projects/nombre-ejercicio-git-libro/capitulos (main)
$ git log
commit aa4d3cdc11b9585557a40935c002e69c9be3af52 (HEAD -> main)
Author: materancode <materanrolo@gmail.com>
Date:   Thu Oct 17 02:24:27 2024 +0100

    Se añadio el primer capitulo



```

## Se añaden los capitulos

``` code
commit b42210352e211007d782f1b48c73d9a38248d10c (origin/main, origin/HEAD)
Author: materancode <materanrolo@gmail.com>
Date:   Mon Oct 14 15:58:35 2024 +0100

    Initial commit




Bárbara@DESKTOP-6E88R1N MINGW64 ~/Documents/Projects/nombre-ejercicio-git-libro/capitulos (main)
$ ls
capitulo1.txt  capitulo2.txt  capitulo3.txt

Bárbara@DESKTOP-6E88R1N MINGW64 ~/Documents/Projects/nombre-ejercicio-git-libro/capitulos (main)
$ cat > índice.txt
Indice de los cápitulos, con conceptos avanzados de git

Bárbara@DESKTOP-6E88R1N MINGW64 ~/Documents/Projects/nombre-ejercicio-git-libro/capitulos (main)
$ ls
capitulo1.txt  capitulo2.txt  capitulo3.txt  índice.txt

Bárbara@DESKTOP-6E88R1N MINGW64 ~/Documents/Projects/nombre-ejercicio-git-libro/capitulos (main)
$  git add .
 git commit -m "Se crea el indice."
 echo "Indice de los cápitulos, con conceptos avanzados de git" >> indice.txt
 git add .
 git commit -m "Añadido el índice ."
 git annotate indice.txt
warning: in the working copy of 'capitulos/índice.txt', LF will be replaced by CRLF the next time Git touches it
[main 0286cb8] Se crea el indice.
 1 file changed, 1 insertion(+)
 create mode 100644 "capitulos/\303\255ndice.txt"
warning: in the working copy of 'capitulos/indice.txt', LF will be replaced by CRLF the next time Git touches it
[main 63982e2] Añadido el índice .
 1 file changed, 1 insertion(+)
 create mode 100644 capitulos/indice.txt
63982e2a        (materancode    2024-10-29 23:07:52 +0000       1)Indice de los cápitulos, con conceptos avanzados de git

Bárbara@DESKTOP-6E88R1N MINGW64 ~/Documents/Projects/nombre-ejercicio-git-libro/capitulos (main)

```

## Cambios en la bibliografía

´´´ code
Bárbara@DESKTOP-6E88R1N MINGW64 ~/Documents/Projects/nombre-ejercicio-git-libro/capitulos (main)
$ cat > capitulo4.txt
  En este capítulo veremos cómo usar GitHub para alojar repositorios en remoto.

Bárbara@DESKTOP-6E88R1N MINGW64 ~/Documents/Projects/nombre-ejercicio-git-libro/capitulos (main)
$ git add .
git commit -m "Añadido capítulo 4."
git log --graph --all --oneline
warning: in the working copy of 'capitulos/capitulo4.txt', LF will be replaced by CRLF the next time Git touches it
[main c67fb9c] Añadido capítulo 4.
 1 file changed, 1 insertion(+)
 create mode 100644 capitulos/capitulo4.txt
* c67fb9c (HEAD -> main) Añadido capítulo 4.
* 63982e2 (bibliografia) Añadido el índice .
* 0286cb8 Se crea el indice.
* 4a4db26 Añadido capítulo 3.


´´´





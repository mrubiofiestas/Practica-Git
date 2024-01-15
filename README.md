# Practica-git
## Identificación:
Nombre y apellidos del/a alumno/a: **Milagros del Rosario Rubio Fiestas**

Nombre del módulo: **LMSGI** 

Nombre del instituto: **IES Aguadulce**

Curso escolar: **DAW 23/24**

### Creación del repositorio en nuestro ordenador (init)
```
Mila@DESKTOP-014ABM1 MINGW64
~ $ git config --global user.email "mila@gmail.com" 

Mila@DESKTOP-014ABM1 MINGW64 ~
$ git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/etc/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
user.name=repaso
user.email=mila@gmail.com
```
### Creación del repositorio en nuestro ordenador (init)
```
Mila@DESKTOP-014ABM1 MINGW64 ~/Documents/Practica-git (master)
$ git init
Initialized empty Git repository in C:/Users/Mila/Documents/Practica-git/.git/

```

### Creación de un commit inicial (add, status, commit, log)
```
Mila@DESKTOP-014ABM1 MINGW64 ~/Documents/Practica-git (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    Documentacion.md
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        img/
        index.html

no changes added to commit (use "git add" and/or "git commit -a")

Mila@DESKTOP-014ABM1 MINGW64 ~/Documents/Practica-git (master)
$ git add .


Mila@DESKTOP-014ABM1 MINGW64 ~/Documents/Practica-git (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md
        new file:   img/Captura de pantalla 2024-01-15 090259.png
        new file:   img/Captura de pantalla 2024-01-15 090539.png
        renamed:    Documentacion.md -> index.html


Mila@DESKTOP-014ABM1 MINGW64 ~/Documents/Practica-git (master)
$ git commit -m "añado img"
[master c03606a] añado img
 4 files changed, 31 insertions(+), 4 deletions(-)
 create mode 100644 img/Captura de pantalla 2024-01-15 090259.png
 create mode 100644 img/Captura de pantalla 2024-01-15 090539.png
 rename Documentacion.md => index.html (100%)


 Mila@DESKTOP-014ABM1 MINGW64 ~/Documents/Practica-git (master)
$ git log --oneline
c03606a (HEAD -> master) añado img
7e46b0f añado README.md
```

##  Creación del repositorio en Github y añadimos de colaborador al profesor. 
![Error](img/Captura%20de%20pantalla%202024-01-15%20090259.png)
![Error](img/Captura%20de%20pantalla%202024-01-15%20090539.png)

## Añadir el remoto al repositorio local (branch, remote)
```
Mila@DESKTOP-014ABM1 MINGW64 ~/Documents/Practica-git (master)
$ git branch
* master

Mila@DESKTOP-014ABM1 MINGW64 ~/Documents/Practica-git (master)
$ git remote add origin https://github.com/mrubiofiestas/Practica-git.git

Mila@DESKTOP-014ABM1 MINGW64 ~/Documents/Practica-git (master)
$ git remote
origin

Mila@DESKTOP-014ABM1 MINGW64 ~/Documents/Practica-git (master)
$ git remote -v
origin  https://github.com/mrubiofiestas/Practica-git.git (fetch)
origin  https://github.com/mrubiofiestas/Practica-git.git (push)

Mila@DESKTOP-014ABM1 MINGW64 ~/Documents/Practica-git (master)
$ git push origin master
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 8 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (10/10), 53.20 KiB | 13.30 MiB/s, done.
Total 10 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/mrubiofiestas/Practica-git.git
 * [new branch]      master -> master
```

## Subir el repositorio a Github (push) y comprobar que está subido a Github.
```
Mila@DESKTOP-014ABM1 MINGW64 ~/Documents/Practica-git (master)
$ git push origin master
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 1.31 KiB | 1.31 MiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/mrubiofiestas/Practica-git.git
   c03606a..7a3caaa  master -> master
```
![Error](img/Captura%20de%20pantalla%202024-01-15%20212240.png)

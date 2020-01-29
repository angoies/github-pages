# github-pages
Nota: el uso b�sico de git se explica en otro m�dulo.

## 1. Tener una cuenta en github
https://github.com/

## 2. Crear en github repositorio para usar github pages
https://help.github.com/en/github/working-with-github-pages

* Crear repositorio
* Activar en settings la opci�n github pages sobre rama master
  * Proporciona URL para ver el sitio web que crearemos, En este tutorial https://angoies.github.io/github-pages/

* Anotar url para clonar repositorio (en bot�n clone o download)
  * en este tutorial => git clone https://github.com/angoies/github-pages.git

## 3. Clonar en vscode el repositorio

### 3.1 necesario tener git instalado y configurado:
```console
$ apt install git
// Set your username:
$ git config --global user.name "FIRST_NAME LAST_NAME"
// Set your email address:
$ git config --global user.email "MY_NAME@example.com"
```

### 3.2 Clonar 
```console
usuario@mdebian10:~/prj$ git config --global user.name "Jose Gómez"
usuario@mdebian10:~/prj$ git config --global user.email "ango.ies@gmail.com"
usuario@mdebian10:~/prj$ git clone https://github.com/angoies/github-pages.git
Clonando en 'github-pages'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Desempaquetando objetos: 100% (3/3), listo.
usuario@mdebian10:~/prj$ ls -al
total 12
drwxr-xr-x  3 usuario usuario 4096 ene 28 21:07 .
drwxr-xr-x 10 usuario usuario 4096 ene 28 21:00 ..
drwxr-xr-x  3 usuario usuario 4096 ene 28 21:07 github-pages
usuario@mdebian10:~/prj$ code github-pages/
```

## 4. Trabajando en vscode
Al iniciar code con el nombre del directorio clonado detecta los ficheros de configuraci�n de git, etc.
En barra de activades lateral est� la opci�n source control: git

Unresumen r�pido: https://code.visualstudio.com/docs/editor/versioncontrol

### Crear una p�gina index.html
Nuevo fichero, etc...
A�adir al stage, commit con mensaje. REcordaemos que se actualiza repositorio local, no remoto.

Neceitamos hacer  push, y nos pide usuario y clave

https://help.github.com/en/github/using-git/caching-your-github-password-in-git


### Comprobar la p�gina en 
https://angoies.github.io/github-pages/
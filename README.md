# github-pages
Nota: el uso básico de git se explica en otro módulo.

## 1. Tener una cuenta en github
https://github.com/

## 2. Crear en github repositorio para usar github pages
https://help.github.com/en/github/working-with-github-pages

* Crear repositorio
* Activar en settings la opción github pages sobre rama master
  * Proporciona URL para ver el sitio web que crearemos, En este tutorial https://angoies.github.io/github-pages/

* Anotar url para clonar repositorio (en botón clone o download)
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
usuario@mdebian10:~/prj$ git config --global user.name "Test User"
usuario@mdebian10:~/prj$ git config --global user.email "testuser@mimail.com"
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
Al iniciar code con el nombre del directorio clonado detecta los ficheros de configuración de git, etc.
En barra de activades lateral está la opción source control: git

Un resumen rápido: https://code.visualstudio.com/docs/editor/versioncontrol

### Crear una página index.html
Nuevo fichero, etc...
Añadir al stage, commit con mensaje. Recordaemos que se actualiza repositorio local, no remoto. Para ello neceitamos hacer  push, y nos pide usuario y clave si no hemos añadido clave pública, etc. 
https://help.github.com/en/github/using-git/caching-your-github-password-in-git


### Comprobar la página en 
https://angoies.github.io/github-pages/

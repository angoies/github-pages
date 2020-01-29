# github-pages

## Tener cuenta en github
https://github.com/

## Crear repositorio de una determinada forma para usar github pages
https://help.github.com/en/github/working-with-github-pages

Crear repositorio, activar en settings la opción  github pages sobre rama master
Proporciona URL para ver el sitio web que crearemos, 
 en este tutorial => https://angoies.github.io/github-pages/

Anotar url para clonar repositorio (en botón clone o download)
  en este tutorial => git clone https://github.com/angoies/github-pages.git

## Clonar en vscode el repositorio..

### necesario git instalado y configurado: user and email..
apt install git
// Set your username:
git config --global user.name "FIRST_NAME LAST_NAME"
// Set your email address:
git config --global user.email "MY_NAME@example.com"

### git clone

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

## En vscode
al iniciar code con el nombre del directorio cloando, detecta los ficheros de congfiguración git, etc..
enb barta lateral izquierda está la opción source control: git
### Crear una página index.html
ctrl+N, etc...
Añadir (en SC, +)
commit con mensaje
Se actuliza resposotiro lcoal, no remoto..

hacer push.. pide usuario y clalve..
?? que esté en confiuración?


https://code.visualstudio.com/docs/editor/versioncontrol

https://help.github.com/en/github/using-git/caching-your-github-password-in-git


## ver página online
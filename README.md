# github-pages
Nota: el uso básico de git se explica en otro módulo.

## 1. Tener una cuenta en github
https://github.com/

## 2. Crear en github repositorio para usar github pages
Tiene las instrucciones detalladas en https://help.github.com/en/github/working-with-github-pages

Básicamente:
* Crear un repositorio
* Activar en settings la opción **Pages** sobre rama master
  * Proporcionar URL para ver el sitio web que crearemos, la de este tutorial https://angoies.github.io/github-pages/

* copiar la url para clonar repositorio en local (en botón clone o download)
  * para el ejemplo de este tutorial => git clone https://github.com/angoies/github-pages.git

## 3. Clonar en vscode el repositorio
Puede usar la línea de comandos, o trabajar directamente en el editor. En este resumen usaremos la segunda.

### 3.1 Paso previo: tener git instalado y configurado
Para ello desde un terminal:

```console
$ apt install git
// Set your username:
$ git config --global user.name "FIRST_NAME LAST_NAME"
// Set your email address:
$ git config --global user.email "MY_NAME@example.com"
```

### 3.2 Clonamos el proyecto (inicialemente estará vacío)
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
En barra de activades lateral está la opción _source control_: git

Un resumen rápido sobre el uso de code y git: https://code.visualstudio.com/docs/editor/versioncontrol

### Crear una página index.html y una de estilos
Nuevo fichero, index.html. Crear una página sencilla, con una hoja de estilo asociada. Crear la hoja de estilo etc. 
Una vez realizados lso cambios, vamos a la barra de actividades de la izquierda, opción "source control", que nos muestra un número con los cambios pendientes. Al desplegar aparecen los ficheros modificados ("Changed") y los incorporados al stage ("Staged Changes"). Al pulsar sobre el nombre del fichero se muestran los cambios en el fichero (diff). Se añade al stage pulsando sobre el icono "+". Una vez todos los ficheros revisados y añadidos al Stage hacemos Commit desde el  mnú superior. 

En general es recomendable al inicirse en el uso de git ejecutar los comando en CLI para además de aprender saber realmente qúe estamos  haciendo. En este caso sería :

```shell
~/github-pages$ git status
En la rama master
Tu rama está actualizada con 'origin/master'.

Cambios no rastreados para el commit:
  (usa "git add <archivo>..." para actualizar lo que será confirmado)
  (usa "git restore <archivo>..." para descartar los cambios en el directorio de trabajo)
        modificado:     css/estilos.css
        modificado:     index.html

sin cambios agregados al commit (usa "git add" y/o "git commit -a")
~/github-pages$ git commit -m "Testing: modificados color cabecera y descripcion en HTML"
[master 0941fed] Testing: modificados color cabecera y descripcion en HTML
 2 files changed, 3 insertions(+), 1 deletion(-)
~/github-pages$  git push origin master
Username for 'https://github.com': angoies
Password for 'https://angoies@github.com': 
Enumerando objetos: 9, listo.
Contando objetos: 100% (9/9), listo.
Compresión delta usando hasta 8 hilos
Comprimiendo objetos: 100% (4/4), listo.
Escribiendo objetos: 100% (5/5), 584 bytes | 584.00 KiB/s, listo.
Total 5 (delta 2), reusado 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/angoies/github-pages.git
   27ce913..0941fed  master -> master
~/github-pages$ 
```

### Comprobar la página en 
https://angoies.github.io/github-pages/

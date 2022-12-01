# Apuntes-entorns
![git-github](https://user-images.githubusercontent.com/114684316/205066498-ebbbe329-a341-49b5-a1ab-36ff80db8735.png)
## Crear un repositorio:
Creamos un directorio de trabajo, una carpeta, con un documento de texto. Para que git comienze a hacer un seguimiento de nuestro trabjo, debemos utilizar el comando **git init**.
Una vez que lo introducimos, este crea dos áreas: 
* Área de ensaño (staging area), es temporal, podemos ver los estados de nuestros archivos.
* Repositorio local, se almacenan copias de nuestro proyecto. 
Hacer un seguimiento de uno o de todos: **git add . **(todos) o ** git add nombre del archivo**

Del directorio de trabajo utilizando **git add** nos pasamos a la área de ensayo, luego, con el comando **git commit** traslada los archivos al área de repositorio local. Luego con el comando **git status -s** (todo lo que no esta en el repositorio, se ve que has hecho cambios y no los has puesto al reporitorio) nos da un listado con los archivos y directorios que tenemos en la carpeta del proyecto. 
Para agregar una descripción o comentario al seguimiento utilizamos el comando **git commit -m "comentario"**, hacemos esto para guardar cambios. Antes de esto debemos decir el archivo en el que esta: **git add hola.txt** y seguidamente usamos **git commit -m "comentario"**.
Para ver un listado de todos los  commits, copias : **git log --oneline**.
Si queremos restaurarlo, al inicio: **git reset --hard numeroamarillo**
## Subir un repositorio a git o clonarlo
Utilizamos el comando **git remote add origin https...** o **git clone url**
## Crear tags/etiquetas
Subir los cambios del remoto a local utilizamos: **git pull** 
Añadir etiquetas : **git tag v1 -m "Versión 1**
Para que aparezca en nuestro repositorio en github debemos: **git push --tags**
Para volver al estado original de un archivo cuando todavía no se ha hecho add : **git checkout nombre-de-archivo**
Para confirmar los cambios del último commit y guardarlos en el repositorio main : **git push origin main**
## Revisar commits realizados
Revisar los commits: **git  log  --oneline --all**
Para ver el contenido del archivo README.md en el commit actual : **cat  README.md**
Si queremos mover la posición del head: **git checkout amarillo**
Luego **cat README.md**
Y seguidamente nos fijamos en **git log --oneline --all**, aquí se ha cambiado.
Para volver al último commit de la rama master: **git  checkout master**
Para traer los cambios realizados en main o master,  a tu copia local **git pull origin main**
((Para crear una rama en nuestra consola: **git branch nombreinventado**))
((Para movernos a esta rama: **git checkout nombreinventado**))
## Etiquetar commits y ver diferencias
Etiquetar commits: **git tag  -a v1(nom etiqueta)  -m "Versión 1"  8b67**
Para eliminarla: **git tag -d nombre_etiqueta**
Para ver los cambios introducidos respecto al commit anterior: **git show ...(podemos poner head,v2,..)**
Para ver las diferencias entre commmits : **git  diff  v1..v2**
También se puede hacer esto: **git show v1..v2**

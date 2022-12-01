# Apuntes-entorns

## Crear un repositorio:
Creamos un directorio de trabajo, una carpeta, con un documento de texto. Para que git comienze a hacer un seguimiento de nuestro trabjo, debemos utilizar el comando **git init**.
Una vez que lo introducimos, este crea dos áreas: 
* Área de ensaño (staging area), es temporal, podemos ver los estados de nuestros archivos.
* Repositorio local, se almacenan copias de nuestro proyecto. 
Hacer un seguimiento de uno o de todos: **git add . ** o ** git add nombre del archivo**

Del directorio de trabajo utilizando **git add** nos pasamos a la área de ensayo, luego, con el comando **git commit** traslada los archivos al área de repositorio local. Luego con el comando **git status -s** (todo lo que no esta en el repositorio, se ve que has hecho cambios y no los has puesto al reporitorio) nos da un listado con los archivos y directorios que tenemos en la carpeta del proyecto. 
Para agregar una descripción o comentario al seguimiento utilizamos el comando **git commit -m "comentario"**, hacemos esto para guardar cambios. Antes de esto debemos decir el archivo en el que esta: **git add hola.txt** y seguidamente usamos **git commit -m "comentario"**.
Para ver un listado de todos los  commits, copias : **git log --oneline**.
Si queremos restaurarlo, al inicio: **git reset --hard numeroamarillo**
## Subir archivo a github


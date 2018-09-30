## Los comandos de configuración sirven para que en ese reportorio todos los archivos tengan las mismas características generales.

* git config --global user.name "i62gacar"
Este comando hace que el usuario propietario del repertorio, sea el indicado entre comillas.

* git config --global user.email i62gacar@uco.es 
Este comando hace que el correo de este repertorio sea el que esta despues de user.email.

* git config --global core.editor "gedit" 
Este comando hace que el editor de texto predeterminado sea el que esta entre comillas.

* git config --global color.ui true 
Este comando cambia el color de la interfaz de todo el repertorio.

* git config –list 
Este comando sirve para listar toda la configuración general.

## Ahora vamos a ver algunos comandos basicos de git

* git init 
Este comando hace que git empieze a controlar el repositorio en el que estamos

* git add 
Este comando hace que añadamos el fichero que hay detras al staging area.

* git commit -m "Mensaje" 
Este comando pasa todo lo que haya en el staging area y lo pasa al repositorio de git, añadiendole el mensaje para saber que ha realizado ese cambio.

* git commit -am " Mensaje " 
Este comando pasa el fichero del area de trabajo logal al repositorio de git de un solo paso.

* git log 
Este comando que lista todos los commit que se han realizado, junto con us id, y su mensaje.

* git help log 
Este comando imprime un tutorial de todas las opciones de log.

* git log -n 5 
Este comando lista los ultimos 5 commit.

* git log -- since =2018 -09 -18 
Este comando lista los commit que se han realizado a partir de la fecha.

* git log -- author ="i62gacar" 
Este comando lista los commit que ha realizado un usuario

* git status 
Este comando te dice la diferencia entre la area de trabajo y el repositorio de git, y tambien la difernecia entre el staging area y el repositorio de git.


* git diff 
Este comando te dice la diferencia entre el area de trabajo y el repertorio de git.

* git diff – staged 
Este comando te dice la difernecia entre el staging area y el repertorio de git.

* git rm archivo git commit -m " Mensaje " 
Estos comandos sirven para eliminar un fichero del repertorio.

* git mv antiguo nuevo git commit -m " Mensaje " 
Estos comandos sirven para mover o renombrar un fichero en el repertorio.

* git checkout  nombre_fichero 
Este comando sirve para deshacer un cambio de un fichero.

* git reset HEAD nombre_fichero 
Este comando sirve para eliminar un cambio del staging area.

* git commit -- amend -m " Mensaje " 
Este comando sirve para complementar el ultimo commit.

* git checkout < id_commit >  nombre_archivo 
Este comando sirve para volver a un commit antiguo.

* git revert < id_commit > 
Este comando sirve para deshacer un commit en concreto.

* git reset -- soft < id_commit >, git reset -- mixed < id_commit >, git reset -- hard < id_commit > 
Estos comando sirven apra deshacer varios cambios del repositorio.

* git clean –n 
Este comando sirve para listar los ficheros los cuales git no controla.

* git clean –f 
Este comando sirve para eliminar los ficheros que git no controla.

* git ls - tree master, git ls - tree master ^^^, git ls - tree master ~3 
Estos comando sirven para listar contenido del repositorio de git.

* git log – oneline 
Este comando sirve para lista los ultimos commit en una sola linea.

* git log -- oneline -3 
Este comando sirve para listar los ultimos 3 commit en una sola linea.

* git show 
Este comando sirve para listar el contenido de un commit.

* git diff<id> nombre_archivo 
Este comando sirve para comparar un commit con el actual.

* git diff id .. id nombre_archivo 
Este comando sirve para dos commit.





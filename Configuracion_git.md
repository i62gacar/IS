##Los comandos de configuración sirven para que en ese reportorio todos los archivos tengan las mismas características generales.

* git config --global user.name "i62gacar", este comando hace que el usuario propietario del repertorio, sea el indicado entre comillas.

* git config --global user.email i62gacar@uco.es, este comando hace que el correo de este repertorio sea el que esta despues de user.email.

* git config --global core.editor "gedit", este comando hace que el editor de texto predeterminado sea el que esta entre comillas.

* git config --global color.ui true, este comando cambia el color de la interfaz de todo el repertorio.

* git config –list, este comando sirve para listar toda la configuración general.

##Ahora vamos a ver algunos comandos basicos de git

* git init, este comando hace que git empieze a controlar el repositorio en el que estamos

* git add, este comando hace que añadamos el fichero que hay detras al staging area.

* git commit -m "Mensaje", este comando pasa todo lo que haya en el staging area y lo pasa al repositorio de git, añadiendole el mensaje para saber que ha realizado ese cambio.

* git commit -am " Mensaje ", este comando pasa el fichero del area de trabajo logal al repositorio de git de un solo paso.

* git log, este comando que lista todos los commit que se han realizado, junto con us id, y su mensaje.

* git help log, este comando imprime un tutorial de todas las opciones de log.

* git log -n 5, este comando lista los ultimos 5 commit.

* git log -- since =2018 -09 -18, este comando lista los commit que se han realizado a partir de la fecha.

* git log -- author ="i62gacar", este comando lista los commit que ha realizado un usuario

* git status, este comando te dice la diferencia entre la area de trabajo y el repositorio de git, y tambien la difernecia entre el staging area y el repositorio de git.


* git diff, este comando te dice la diferencia entre el area de trabajo y el repertorio de git.

* git diff – staged, este comando te dice la difernecia entre el staging area y el repertorio de git.

* git rm archivo git commit -m " Mensaje ", estos comandos sirven para eliminar un fichero del repertorio.

* git mv antiguo nuevo git commit -m " Mensaje ", estos comandos sirven para mover o renombrar un fichero en el repertorio.

* git checkout  nombre_fichero, este comando sirve para deshacer un cambio de un fichero.

* git reset HEAD nombre_fichero, este comando sirve para eliminar un cambio del staging area.

* git commit -- amend -m " Mensaje ", este comando sirve para complementar el ultimo commit.

* git checkout < id_commit >  nombre_archivo, este comando sirve para volver a un commit antiguo.

* git revert < id_commit >, este comando sirve para deshacer un commit en concreto.

* git reset -- soft < id_commit >, git reset -- mixed < id_commit >, git reset -- hard < id_commit >, estos comando sirven apra deshacer varios cambios del repositorio.

* git clean –n, este comando sirve para listar los ficheros los cuales git no controla.

* git clean –f, este comando sirve para eliminar los ficheros que git no controla.

* git ls - tree master, git ls - tree master ^^^, git ls - tree master ~3, estos comando sirven para listar contenido del repositorio de git.

* git log – oneline, este comando sirve para lista los ultimos commit en una sola linea.

* git log -- oneline -3, este comando sirve para listar los ultimos 3 commit en una sola linea.





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


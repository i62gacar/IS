## Los comandos de configuración sirven para que en ese reportorio todos los archivos tengan las mismas características generales.

* git config --global user.name "i62gacar" :
Este comando hace que el usuario propietario del repertorio, sea el indicado entre comillas.

* git config --global user.email i62gacar@uco.es :
Este comando hace que el correo de este repertorio sea el que esta despues de user.email.

* git config --global core.editor "gedit" :
Este comando hace que el editor de texto predeterminado sea el que esta entre comillas.

* git config --global color.ui true :
Este comando cambia el color de la interfaz de todo el repertorio.

* git config –list :
Este comando sirve para listar toda la configuración general.

## Ahora vamos a ver algunos comandos basicos de git

* git init :
Este comando hace que git empieze a controlar el repositorio en el que estamos

* git add :
Este comando hace que añadamos el fichero que hay detras al staging area.

* git commit -m "Mensaje" :
Este comando pasa todo lo que haya en el staging area y lo pasa al repositorio de git, añadiendole el mensaje para saber que ha realizado ese cambio.

* git commit -am " Mensaje " :
Este comando pasa el fichero del area de trabajo logal al repositorio de git de un solo paso.

* git log :
Este comando que lista todos los commit que se han realizado, junto con us id, y su mensaje.

* git help log :
Este comando imprime un tutorial de todas las opciones de log.

* git log -n 5 :
Este comando lista los ultimos 5 commit.

* git log -- since =2018 -09 -18 :
Este comando lista los commit que se han realizado a partir de la fecha.

* git log -- author ="i62gacar" :
Este comando lista los commit que ha realizado un usuario

* git status :
Este comando te dice la diferencia entre la area de trabajo y el repositorio de git, y tambien la difernecia entre el staging area y el repositorio de git.


* git diff :
Este comando te dice la diferencia entre el area de trabajo y el repertorio de git.

* git diff – staged :
Este comando te dice la difernecia entre el staging area y el repertorio de git.

* git rm archivo git commit -m " Mensaje " :
Estos comandos sirven para eliminar un fichero del repertorio.

* git mv antiguo nuevo git commit -m " Mensaje " :
Estos comandos sirven para mover o renombrar un fichero en el repertorio.

* git checkout  nombre_fichero :
Este comando sirve para deshacer un cambio de un fichero.

* git reset HEAD nombre_fichero :
Este comando sirve para eliminar un cambio del staging area.

* git commit -- amend -m " Mensaje " :
Este comando sirve para complementar el ultimo commit.

* git checkout < id_commit >  nombre_archivo :
Este comando sirve para volver a un commit antiguo.

* git revert < id_commit > :
Este comando sirve para deshacer un commit en concreto.

* git reset -- soft < id_commit >, git reset -- mixed < id_commit >, git reset -- hard < id_commit > :
Estos comando sirven apra deshacer varios cambios del repositorio.

* git clean –n :
Este comando sirve para listar los ficheros los cuales git no controla.

* git clean –f :
Este comando sirve para eliminar los ficheros que git no controla.

* git ls - tree master, git ls - tree master ^^^, git ls - tree master ~3 :
Estos comando sirven para listar contenido del repositorio de git.

* git log – oneline :
Este comando sirve para lista los ultimos commit en una sola linea.

* git log -- oneline -3 :
Este comando sirve para listar los ultimos 3 commit en una sola linea.

* git show :
Este comando sirve para listar el contenido de un commit.

* git diff<id> nombre_archivo :
Este comando sirve para comparar un commit con el actual.

* git diff id .. id nombre_archivo :
Este comando sirve para dos commit.




# Comandos de ramas en git

Las ramas en git se usan para separar la línea principal del proyecto de forma que se puedan trabajar en otras versiones del software sin pisar la principal.

![Ejemplo de Ramas](https://www.paradigmadigital.com/wp-content/uploads/2016/08/Git4.jpg)

Los siguientes comandos se usarán para trabajar ramas en proyecto de git:

1. Ver las ramas listadas:

~~~

git branch

~~~

2. Crear una rama

~~~

git branch nombre_rama

~~~

3. Cambiarnos de rama

~~~

git checkout nombre_rama

~~~

4. Hacer pasos 2 y 3 al mismo tiempo

~~~

git checkout -b nombre_rama

~~~

5. Comparar ramas

~~~

git diff nombre_rama...nombre_rama

~~~

6. Ver ramas idénticas a la actual

~~~

git branch --merged

~~~

7. Renombrar ramas

~~~

git branch -m nombre_antiguo nombre_nuevo

~~~

8. Eliminar ramas

~~~

git branch -d nombre_rama
git branch -D nombre_rama

~~~

9. Integrar ramas a la actual

~~~

git merge nombre_rama

~~~

10. Resolver conflictos (de forma manual)

~~~

git merge --abort

~~~

11. Almacenar cambios temporales

~~~

git stash save "Mensaje"

~~~

12. Listar cambios

~~~

git stash list

~~~

13. Ver contenido de un cambio temporal

~~~

git stash show -p nombre_stash

~~~

14. Eliminar cambio temporal

~~~

git stash drop nombre_stash

~~~

15. Aplicar cambio del *stash*

~~~

git stash apply nombre_stash
git stash pop nombre_stash

~~~

# Comandos de Github en Git

Github es un sitio de internet donde puedes subir los proyectos que creas usando git. Aunque ambos no son iguales.

![Github no es Git](https://i.blogs.es/0bdd9c/github/450_1000.jpg)

Los comandos se usan para subir el código de tus proyectos a esta página web.

1. Añadir repositorio remoto

~~~
git remote add origin url
~~~

2. Ver rpositorios remotos

~~~
git remote -v
~~~

3. Eliminar repositorio remoto

~~~
git remote rm origin
~~~

4. Añadir cambios LOCAL -> REMOTO

~~~
git push -u origin master
~~~

5. Al revés (REMOTO -> LOCAL)

~~~
git pull -u origin master
~~~

6. Ver ramas remotas

~~~
git branch -r
~~~

7. Ver todas las ramas

~~~
git branch -a
~~~

8. Clonar un repositorio remoto

~~~
git clone url
~~~

## Dar seguimiento a las ramas remotas

* LOCAL -> REMOTO

~~~
git push ...
~~~

* REMOTO -> LOCAL

- Sincronización y unión

~~~
git fetch origin
git merge origin/master
~~~

- En un paso

~~~
git pull
~~~

## Operaciones con ramas remotas

* Creación

~~~
git push -u origin rama_remota
~~~

* Copia

~~~
git checkout -b local remoto
~~~

* Eliminación

~~~
git push origin --delete rama_remota
~~~

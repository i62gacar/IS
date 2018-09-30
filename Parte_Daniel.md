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

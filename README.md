# Aprendiendo _Git_ y _GitHub_

Esto se va poner chido 

## Comandos terminal

- git init
- git add .
- git commit -m "<message>"
- git commit (abre archivo de configuracion en el cual tienes q poner el mensaje y guardar el archivo y cerrarlo para que haga efectos los cambios)
- git remote add origin https://github.com/usuario/repositorio.git
- git push -u origin main (coloca como rama principal a la rama main)
- git push .
- git pull 
- git branch -M main
- git branch -m main {rama1} (para crear una rama que sea igual al nombre que coloque en rama1 sin {} y copia todo los componentes de la rama main)
- git symbolic-ref refs/remotes/origin/HEAD refs/remotes/origin/ma (Cambia el HEAD actual a la rama main)
- para modificar la rama por default ir a GitHub al repositorio y en settings(configuraciones), cambiar el default branch
- git config --global init.defaultBranch main (remplaza la rama en git)
- git push origin --delete master (elimina la rama master)


*Abre la ayuda en un navegador de internet*
- git help (función)
*Abre la ayuda en la terminal*
- git -h (función)

# En el archivo .gitignore incluimos todo lo que NO queramos incluir en nuestro repositorio. Lo podemos crear manualmente o con gitignore.io.

- *esto es un comentario*

archivo.ext
carpeta
/archivo_desde_raiz.ext

- *ignorar todos los archivos que terminen en .log*

*.log

- *excepto production.log*

!production.log

- *ignorar los archivos terminados en .txt dentro de la carpeta doc, pero no en sus subcarpetas*

doc/*.txt

- *ignorar todos los archivos terminados en .txt dentro de la carpeta doc y también en sus subcarpetas*

doc/**/*.txt

# Ramas,  cambios y uso de ramas

- crear rama /
git branch nombre-rama

- cambiar de rama /
git checkout nombre-rama

- crear una rama y cambiarte a ella /
git checkout -b rama

- eliminar rama /
git branch -d nombre-rama

- eliminar ramas remotas /
git push origin --delete nombre-rama

- eliminar rama (forzado) /
git branch -D nombre-rama

- listar todas las ramas del repositorio /
git branch

- lista ramas no fusionadas a la rama actual /
git branch --no-merged

- lista ramas fusionadas a la rama actual /
git branch --merged

- rebasar ramas /
git checkout rama-secundaria
git rebase rama-principa



## git push --set-upstream origin = git push -u origin

git log (para ver los commit)
git log --oneline (Ver todo los commit sin descripcion por mensaje
 y codigo)
Apretar enter las veces que sea necesario para llegar a ver toda la lista

git commit --amend --no-edit (Modificar el ultimo commit sin cambiar el comentario)

git reset --hard HEAD~1 (Volver al commit anterior)
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
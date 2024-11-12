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
## Configuración básica

Configurar nombre de usuario
```ssh
	git config --global user.name "nick"
```
Configurar e-mail
```ssh	
	git config --global user.email e@mail.com
```
Marco de colores para los comandos
```ssh
	git config --global color.ui true
```

## Iniciando repositorio

Iniciamos GIT en carpeta actual
```ssh
	git init
```
Clonar el repositorio
```ssh
	git clone <url>
```
Preparar carpeta actual para commit
```ssh
	git add .
```
Hacer el primer commit
```ssh
	git commit -m "Texto que identifique por que se hizo el commit"
```
Subir al repositorio
```ssh
	git push origin master
```


## GIT ADD


Preparar carpeta actual para commit
```ssh
	git add .
```
Añadir archivo para commit
```ssh
	git add <archivo>
```
Añadir todos los archivos para el commit omitiendo los nuevos
```ssh
	git add --all 
```
Añadir todos los archivos con la extensión específica
```ssh
	git add *.txt
```
Añadir todos los archivos dentro de un directorio y de una extensión específica
```ssh
	git add docs/*.txt
```
Añadir todos los archivos dentro de un directorios
```ssh
	git add docs/
```

## GIT PUSH

Subir al repositorio
```ssh
	git push <origien> <branch>
```
Subir una etiqueta
```ssh
	git push --tags
```
## GIT LOG

Mostrar los logs de los commits
```ssh
	git log
```
Mostrar los cambios en los commits
```ssh
	git log --oneline --stat
```
Mostrar gráficos de los commits
```ssh
	git log --oneline --graph
```

## GIT HEAD

Sacar un archivo del commit
```ssh
	git reset HEAD <archivo>
```
Devolver el último commit que se hizo y pone los cambios en staging
```ssh
	git reset --soft HEAD^
```
Devolver el último commit y todos los cambios
```ssh
	git reset --hard HEAD^
```
Devolver los 2 últimos commit y todos los cambios
```ssh
	git reset --hard HEAD^^
```
Rollback merge/commit
```ssh
	git log
	git reset --hard <commit_sha>
```
## GIT REMOTE

Agregar repositorio remoto
```ssh
	git remote add origin <url>
```
Cambiar de remote
```ssh
	git remote set-url origin <url>
```
Eliminar repositorio
```ssh
	git remote rm <name/origin>
```
Mostrar lista repositorios
```ssh
	git remote -v
```
Mostrar las branches remotos
```ssh	
	git remote show origin
```
Limpiar todos las branches eliminados
```ssh
	git remote prune origin 
```
## GIT BRANCH

Crear una branch
```ssh
	git branch <nameBranch>
```
Listar las branches
```ssh
	git branch
```
Eliminar la branch y unirlo al master
```ssh
	git branch -d <nameBranch>
```
Eliminar sin preguntar
```ssh
	git branch -D <nameBranch>
```
## GIT TAG

Mostrar una lista de todas las tags
```ssh
	git tag
```
Crear una nueva tag
```ssh
	git tag -a <verison> - m "esta es la versión x"
```

## OTROS COMANDOS

Listar estado actual del repositorio con lista de archivos modificados o agregados
```ssh
	git status
```
Quitar del HEAD un archivo y ponerle el estado de no trabajado
```ssh
	git checkout -- <file>
```
Crear una branch en base a una online
```ssh
	git checkout -b newlocalbranchname origin/branch-name
```
Buscar los cambios nuevos y actualizar el repositorio
```ssh
	git pull origin <nameBranch>
```
Cambiar de branch
```ssh
	git checkout <nameBranch/tagname>
```
Unir la branch actual con el especificado
```ssh
	git merge <nameBranch>
```
Verificar cambios en el repositorio online con el local
```ssh
	git fetch
```
Borrar un archivo del repositorio
```ssh
	git rm <archivo> 
```

## Fork

Descargar remote de un fork
```
	git remote add upstream <url>
```

Merge con master de un fork
```
	git fetch upstream
	git merge upstream/master
```

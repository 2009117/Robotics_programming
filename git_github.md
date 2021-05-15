# Git Commands
In the following document, I going to show the differents commads with **git** . This command are for the second week of the Structured Programming. The following aspects will be taken:

- Basic commands of Bash
- Their functions 

##  Commands

- **Git init**: crea un nuevo repositorio local Git.
`git init `

- **Git status**: muestra la lista de los archivos que se han cambiado junto con los archivos que están por ser preparados o confirmados.
`git status`

- **Git init "myfile"**: Crear un repositorio con un nombre.
`git init [nombre deseado]`

- **Git clone** : se usa para copiar un repositorio. Si esta en el servidor.
- `git clone nombredeusuario@host:/path/to/repository`
 
- **Git add**:  Para agregar archivos al area de preparación. 
`git add [nombre]`
`git add * `---> ***sirve para poder agregar todo***

- **Git commit**: Creará una lista instanteana de los cambios y los guardara en el directorio de git.
`git commit`
`git commit --amend`---> ***Agrega algun cambio que le hayas hecho al commit***
- **Git mv**: Sirve para poder cambiar de nombre de un archivo
`git mv [Nombre original del archivo] from_file_to`

- **Git mv**: cambiar de lugar un archivo 
`git commit -m "Moved [nombre del archivo] to [nuevo lugar]
` 

- **Git clone**: Para poder clonar proyectos
`git clone [URL del proyecto que queramos clonar]`

##
-  **Git log** 

|Code  | function |
|------|--------| 
| `git log`| sirve | 
| `git log -p -2` | Sirve para mostrar las versiones del proyecto
| `git log -since=2.weeks`| Sirve para poder ver los ultimos proyectos. (***tu delimitas el tiempo***) 
|`git log --stat`| Muestras las estadisticas de modificacion del archivo en cada commit.
|`git log -p`| Mostrar el parche introducido en cada commit
| `git log --shortstat`| Muestra solo la linea modificada/ insercciones/ eliminaciones del comando. 
|`git log --name-only`|Muestra la lista de archivos modificados después de la información de confirmación
| `git log -abbrev-commit` | Muestra solo los primeros caracteres de las suma de comprobación SHA-1 en lugar de los 40
##

- **Git relative**: Muestra la fecha de un formato relativo. 
`git --relative-date`

- **Git reset HEAD** : Sirve para quitar archivos
`git reset HEAD [nombre del archivo`
- **Git checkout**: Nos ayuda a que un archivo al que le hicimos un commnit no se modifique. Tambien para regresar a la version respaldad del archivo.
`git checkout [nombre del archivo] `

- **Git remote**: 
`git remote -V`---> Nos da la lisat de los directorios que estan remotos. 
`git remote add pb [IURL]` --->  Agrega directorios
- **Git fetch pb**:Muestra las últimas versiones del proyecto.
`git remote pb`

- **Git tag**: Mostrar versiones
`git tag`
`git tag -a v1.4 -m "my version 1.4"] `---> Sirve para poner una etiqueta de versión. 
##
- **Branch**

- **Git push**: 
`git push`---> Se usa para enviar confirmaciones locales 
`git push origin < master >`---> En esta es la misma solo que podemos cambiar la rama a la que queremos que vaya.

- **Git branch** para crear ramas
`git branch`
`git branch < nombre de la rama >`

- **Git branch** para borrar una rama: 
`git branch -d [nombre de la rama]`
`git branch -D [nombre de la rama]`---> Para forzar el borrado de la rama. 
- **Git checkout**: Crea ramas y te ayuda a navegar en ellas.
`git checkout -b < nombre de la rama >`
-  **Git merge**: Se usa para fusionar una rama con otra rama activa 
-`git merge < nombre de la rama > `
 
-  **Git diff**: 
`git diff --base <nombre del archivo>`---> Se usa para hacer una lista de conflictos

`git diff < source-branch > < target-branch >`---> Se usa para ver los conflictos que hay entre ramas antes de fusionarlas.

##

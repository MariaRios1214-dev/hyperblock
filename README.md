# hyperblock

Un block increible para el curso de Git y Github

# Commands Git

- git log --oneline - Te muestra el id commit y el título del commit.
- git log --decorate- Te muestra donde se encuentra el head point en el log.
- git log --stat - Explica el número de líneas que se cambiaron brevemente.
- git log -p- Explica el número de líneas que se cambiaron y te muestra que se cambió en el contenido.
- git shortlog - Indica que commits ha realizado un usuario, mostrando el usuario y el titulo de sus commits.
- git log --graph --oneline --decorate y
- git log --pretty=format:"%cn hizo un commit %h el dia %cd" - Muestra mensajes personalizados de los commits.
- git log -3 - Limitamos el número de commits.
- git log --after=“2018-1-2” ,
- git log --after=“today” y
- git log --after=“2018-1-2” --before=“today” - Commits para localizar por fechas.
- git log --author=“Name Author” - Commits realizados por autor que cumplan exactamente con el nombre.
- git log --grep=“INVIE” - Busca los commits que cumplan tal cual está escrito entre las comillas.
- git log --grep=“INVIE” –i- Busca los commits que cumplan sin importar mayúsculas o minúsculas.
- git log – index.html- Busca los commits en un archivo en específico.
- git log -S “Por contenido”- Buscar los commits con el contenido dentro del archivo.
- git log > log.txt - guardar los logs en un archivo txt

# Fork

![image](imagenes/fork.jpg)

Forks o Bifurcaciones
Es una característica única de GitHub en la que se crea una copia exacta del estado actual de un repositorio directamente en GitHub, éste repositorio podrá servir como otro origen y se podrá clonar (como cualquier otro repositorio), en pocas palabras, lo podremos utilizar como un git cualquiera
.
Un fork es como una bifurcación del repositorio completo, tiene una historia en común, pero de repente se bifurca y pueden variar los cambios, ya que ambos proyectos podrán ser modificados en paralelo y para estar al día un colaborador tendrá que estar actualizando su fork con la información del original.
.
Al hacer un fork de un poryecto en GitHub, te conviertes en dueñ@ del repositorio fork, puedes trabajar en éste con todos los permisos, pero es un repositorio completamente diferente que el original, teniendo alguna historia en común.
.
Los forks son importantes porque es la manera en la que funciona el open source, ya que, una persona puede no ser colaborador de un proyecto, pero puede contribuír al mismo, haciendo mejor software que pueda ser utilizado por cualquiera.
.
Al hacer un fork, GitHub sabe que se hizo el fork del proyecto, por lo que se le permite al colaborador hacer pull request desde su repositorio propio.

Trabajando con más de 1 repositorio remoto
Cuando trabajas en un proyecto que existe en diferentes repositorios remotos (normalmente a causa de un fork) es muy probable que desees poder trabajar con ambos repositorios, para ésto puedes crear un remoto adicional desde consola.

git remote add <nombre_del_remoto> <url_del_remoto>
git remote upstream https://github.com/MariaRios1214-dev/hyperblock.git
Al crear un remoto adicional podremos, hacer pull desde el nuevo origen (en caso de tener permisos podremos hacer fetch y push)

git pull <remoto> <rama>
git pull upstream master
Éste pull nos traerá los cambios del remoto, por lo que se estará al día en el proyecto, el flujo de trabajo cambia, en adelante se estará trabajando haciendo pull desde el upstream y push al origin para pasar a hacer pull request.

git pull upstream master
git push origin master

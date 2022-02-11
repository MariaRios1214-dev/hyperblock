# hyperblock
Un block increible para el curso de Git y Github 


# Commands Git 
* git log --oneline - Te muestra el id commit y el título del commit.
* git log --decorate- Te muestra donde se encuentra el head point en el log.
* git log --stat - Explica el número de líneas que se cambiaron brevemente.
* git log -p- Explica el número de líneas que se cambiaron y te muestra que se cambió en el contenido.
* git shortlog - Indica que commits ha realizado un usuario, mostrando el usuario y el titulo de sus commits.
* git log --graph --oneline --decorate y
* git log --pretty=format:"%cn hizo un commit %h el dia %cd" - Muestra mensajes personalizados de los commits.
* git log -3 - Limitamos el número de commits.
* git log --after=“2018-1-2” ,
* git log --after=“today” y
* git log --after=“2018-1-2” --before=“today” - Commits para localizar por fechas.
* git log --author=“Name Author” - Commits realizados por autor que cumplan exactamente con el nombre.
* git log --grep=“INVIE” - Busca los commits que cumplan tal cual está escrito entre las comillas.
* git log --grep=“INVIE” –i- Busca los commits que cumplan sin importar mayúsculas o minúsculas.
* git log – index.html- Busca los commits en un archivo en específico.
* git log -S “Por contenido”- Buscar los commits con el contenido dentro del archivo.
* git log > log.txt - guardar los logs en un archivo txt

# SSH --- Protocolo Security shell

Generar una nueva llave SSH: (Cualquier sistema operativo)

ssh-keygen -t rsa -b 4096 -C "youremail@example.com"

**Comprobar proceso y agregarlo (Windows)**

eval $(ssh-agent - s)
ssh-add ~/.ssh/id_rsa
**Cambiar la url / ir a url proyecto8**
git remote-v ---> Muestra estado actual del direccion de repositorio
git remote set-url origin ssh del proyecto 
**ejemplo** git remote set-url origin git@github.com:MariaRios1214-dev/hyperblock.git


**Comprobar proceso y agregarlo (Mac)**

eval "$(ssh-agent -s)"

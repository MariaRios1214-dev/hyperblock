# hyperblock
Un block increible para el curso de Git y Github 


# Commands Git 
* git log --oneline - Te muestra el id commit y el título del commit.
* git log --decorate- Te muestra donde se encuentra el head point en el log.
* git log --stat - Explica el número de líneas que se cambiaron brevemente.
* git log -p- Explica el número de líneas que se cambiaron y te muestra que se cambió en el contenido.
* git shortlog - Indica que commits ha realizado un usuario, mostrando el usuario y el titulo de sus commits.
* git log --graph -> Muestra ultimos paths historia del proyecto
* git log --graph --oneline --decorate Muestra todos los paths historia del proyecto
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
* git log --all --graph --decorate --oneline --> muestra a nivel de ramas el hitorias del proyecto

# SSH --- Protocolo Security shell

Generar una nueva llave SSH: (Cualquier sistema operativo) </br>
ssh-keygen -t rsa -b 4096 -C "youremail@example.com"

**Comprobar proceso y agregarlo (Windows)**

eval $(ssh-agent -s)
ssh-add ~/.ssh/id_rsa

**Cambiar la url / ir a url ssh del proyecto**

git remote-v ---> Muestra estado actual del direccion de repositorio </br>
git remote set-url origin ssh del proyecto </br>
**ejemplo** git remote set-url origin git@github.com:MariaRios1214-dev/hyperblock.git

**Comprobar proceso y agregarlo (Mac)**

eval "$(ssh-agent -s)"
¿Usas macOS Sierra 10.12.2 o superior?
Haz lo siguiente:

cd ~/.ssh
Crea un archivo config…
Con vim config
Con VSCode code config
Pega la siguiente configuración en el archivo…
Host *
  AddKeysToAgent yes
  UseKeychain yes
  IdentityFile ~/.ssh/id_rsa

**Agrega tu llave privada en tu entorno**

ssh-add -K ~/.ssh/id_rsa

# Alias para guardar comandos 
 alias pathRamas="git log --all --graph --decorate --oneline"
 y luego solo es llamar el alias ej **pathRamas**

# Tags

## create  tags con hash (commit corto)
$ git tag -a v0.1 -m "Resultado de las primeras clases del grupo" 963f613
## ver tags
$ git tag
v0.1
## ver  tags con relacion al commit hash (commit corto)
$ git show-ref --tags
2550019ebd4eede402e9b3e3dd15424158c2c205 refs/tags/v0.1

## empujar los tags al ambiente 
$ git push origin --tags

##borar tags
$ git tag -d v0.2

##eliminar totalmente la referencia del tags / borrado permanente
$ git push origin :refs/tags/v0.2

Warning: Permanently added the ECDSA host key for IP address '140.82.112.4' to the list of known hosts.
To github.com:MariaRios1214-dev/hyperblock.git
 - [deleted]         v0.2






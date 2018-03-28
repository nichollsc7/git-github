# Git y GitHub
Aprendizaje sobre Git y  Github

## Cualidades de Git

Con git  es posible el manejo veloz de la información ya que guarda dato  sobre el cambio realizado y no todo el el cambio por versión para mayor velocidad y el poder trabajar de manera offline sin que afecte tú propio progreso en el repositorio.



 + Permite trabajar con grandes proyectos.

 +  Facilidad en el manejo desde tu propio computador

 +  Codigo  bastamente completo con herramientas de utilidad

 +  Manejo a gusto en que versión continuar progresando.

 +  Poder replicar fácilmente  los repositorios

 


## Sistemas control de versiones
Es un sistema que nos permite almacenar información, como biblioteca y separe en capitulos los avances que hagas en el libro( archivo o conjunto de archivos) a lo largo del tiempo.

## Clasificado en  3 tipos de SCV:

#### Local

La información  es guardada en el computador que se use, no esta en otro lugar o internet, donde  tendrias toda la información puedes volver atras o continuar donde ibas.

+ Precaución: En caso de perdida del computador o de la información donde esta contenida los archivos, se perderia totalmente el archivo o los archivos.

##### Central

La información es guardada en el  computador y en el servidor donde esta almacenado el repositorio.

 + la información guardada en el servidor puede ser distribuida a demás computadores y los computadores pueden hacer cambios y mandarlos a el servidor.

 + Precaución: Si el server el lugar donde se esta recibiendo los cambios, en caso de perdida del servidor, se perderian los cambios y avances o hasta la totalidad de los archivos.

 #### Distribuido (En donde aplica GitHub)

 La información es guardada en internet, cada integrante que participe en el repositorio, cada uno tendra el repositorio completo en el computador, podra alterar o cambiar su propio repositorio sin alterar el repositorio de otros, como tambíen el poder mezclarlos.

 + En caso de perdida del computador,  se podra recuperar  la información "que se perdio con el computador" pidiendo una copia de la información guardada  en la computadora principal o cualquier copia  del repositorio.

 ## Comandos de Git y sus funciones

<details>
    <summary>Comandos basicos de Git</summary>

```
git: lista de los subcomandos de Git

git config --global user.email example@example.com :

git config --global user.name example :

git init: iniciar un repositorio dentro de la carpeta o (git init example para que tenga nombre el repositorio)

git status: muestra los archivos que esperan ser agregados en el staging area, los que son agregados y esperan confirmanción; guardados cuando se use el comando git commit.

git add example : agrega el archivo al Staging Area.

git log : muestra los commit creados, con la fecha, el autor y el codigo de 40 digitos como Hash del mismo.

git log --oneline : muestra la lista de los commist de manera resumida.

git mv example: mueve, renombra una carpeta

```
</details>
<details>
    <summary>Comandos basicos Git 2</summary>

```
git version: muestra la version instalada de Git

git clone link : clona un directorio de el link dado

git branch: git branch [nombre] se crea una nueva rama
-l: listamos las ramas
-d/-D [nombre]: borramos rama
-m [nombre] [nombre_nuevo]: para renombrar ramas

git checkout [nombre/sha1]: Nos permite mover entre ramas y entre commits, no vamos a borrar nada. Acá es donde podemos movernos en el tiempo.

git checkout -b [nombre_rama]: Nos permite crear una nueva rama sin necesidad de usar branch

git commit "example": agrega a los archivos que  estan en el Staging area y el nombre

git diff: sirve para comparar los cambios hechos entre commits con su respectiva versión(tag) o su numero hexadecimal o el sha1.

git log >bitacora_log.txt recomendable hacer un respaldo antes de cualquier reset.

git reset --soft: No toca los cambios en área de trabajo. Solo borra los títulos(restablece el encabezado del commit). Esto deja todos los cambios modificados, listos para hacer un commit nuevo y resumido.

git reset --mixed: es muy parecido a reset soft, la diferencia es que git reset mixed iguala el Stagin area al working directory. Significa que borra el commit, pero para que nosotros puedamos hacer un commit nos toca antes agregar los archivos al Stagin area.

git stash: es otro de los limbos, como el staging area. Para agregar los cambios estos deben estar en el staging area.

git stash list: nos muestra la lista de stash que tengamos.

git stash drop stash@{numero}: nos permite borrar un stash.

git stash apply: aplicamos el último cambio

```
</details>

</details>

<details>
    <summary>Comandos basicos de Git 3</summary>

```
git init add -A : Agrega todos los archivos del Working Directory al Staging Area.

git init add [file or directory] : Agrega un archivo o carpeta del Working Directory al Staging Area.

git init add -n [file or directory] : Simula el agregado de un archivo o directorio al Staging Area pero la verdad no lo hace.

git rm --cached [file or directory] : Elimina un archivo o carpeta del Staging Area y lo deja en el Working Directory.

git commit --amend : concatena cambios al ultimo commit.

git tag  number: etiquetar  que sirve para saber la versión de el ultimo commit.

git tag: nos permite agregar etiquetas a nuestros cambios.
-a para la anotación
-m para el mensaje

-l nos muestra la lista de etiquetas
-f para renombrar
-d para borrar

Git fetch origin master: Traer del remoto

Git merge origin/master: combinar lo que se trajo de remoto con la rama donde se escribe este comando

git push origin master : Asi subimos nuestros cambios a github


git push origin master --tags : Tambien podemos enviar los tags 


git push origin [otra_rama] : Podemos enviar otras ramas

git pushorigin --all: enviar todas las ramas directamente una sola vez

git merge [rama]: Nos permite mezclar los cambios realizados en dicha rama con la rama en la que estamos.

fast-forward: los mezcla automáticamente
recursive/auto-merging: ambas ramas salieron al mismo tiempo y hay algo nuevo en la rama que la otra no recuerda, por eso hace la mezcla recursiva.
manual merge: nos va a tocar decirle a git específicamente los cambios que queremos mezclar.

git rebase: hace prácticamente lo mismo que merge, cambiamos la historia de nuestro proyecto sin crear bifurcaciones del proyecto. Es mejor usar merge
Usar solo git rebase de manera local.

-i: de manera interactiva, nos abrira el editor que tengamos definido en la configuración de git.

git cherry-pick [SHA-1]: Cuando usamos el git cherry-pick no cambia de rama el commit, en este caso git hace una copia del commit y la pega en la rama que queremos con un SHA-1 diferente. 




```
</details>

<details>
    <summary>Comandos basicos terminal</summary>

```
mkdir example: crea la carpeta con el nombre example

ls: muestra los archivos dentro de la carpeta

clear :limpia la terminal

touch: crea un archivo dentro de la carpeta

rm example: para borrar el archivo llamado example

rm -rf example: para borrar la carpeta example

vim example.txt : para editar  el archivo example(al finalizar salir con qw para salir y guardar) 

q: para salir dentro de un archivo

w: para guardar los cambios dentro de un archivo

```
</details>

<details>
    <summary>Comandos entre Git y GitHub </summary>

```
git clone [https/ssh] : en github nos hace una copia del proyecto en nuestro perfil/repositorios para poder hacerle lo que queramos,dependendo de  si eliges https o ssh, el ssh pide verificar de forma remota por mayor seguridad.
(https://help.github.com/articles/which-remote-url-should-i-use/)

git remote add [origin] [SSH/HTTPS] : Conecta un repositorio con nuestro equipo local.

git remote -v : Lista las conexiones existentes.

git remote remove [origin] : Elimina una conexión con algún repositorio.


```
</details>

### Palabras claves

SHA : “secure hash algorithm” (algoritmo de hashes seguros)

Hash : es un algoritmo que convierte cualquier cosa en una cadena de caracteres de 40 caracteres




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

git init:

//muestra que archivos estan integrados, cuales esperan para ser integrados  y cuales  estan
git status

git add :

git log :

git log --oneline :

git mv example:

git rm example: elimina rm

git rm -f example: elimina forzado rm

git version: muestra la version instalada de Git




```
</details>
<details>
    <summary>Comandos basicos Git 2</summary>

```
git clone:

git branch:

git checkout:

git commit:

git diff:



git log >bitacora_log.txt recomendable hacer un respaldo antes de cualquier reset.

git reset --soft: No toca los cambios en área de trabajo. Solo borra los títulos(restablece el encabezado del commit). Esto deja todos los cambios modificados, listos para hacer un commit nuevo y resumido.

git reset --mixed: es muy parecido a reset soft, la diferencia es que git reset mixed iguala el Stagin area al working directory. Significa que borra el commit, pero para que nosotros puedamos hacer un commit nos toca antes agregar los archivos al Stagin area.
```
</details>

<details>
    <summary>Comandos basicos terminal</summary>

```
mkdir example: crea la carpeta con el nombre example

ls:

clear :limpia la terminal


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

<details>
    <summary>Comandos</summary>

```


```
</details>
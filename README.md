# practica_git

1- ¿Qué comando utilizaste en el paso 11? ¿Por qué?

Utilicé el comando *git reset --hard HEAD~1* porque deshace el commit  modificando el "working copy" a como estaba antes (commit anterior al deshecho), es decir, se mueve el puntero HEAD al commit anterior y  se pierden todas modificaciones posteriores a éste.

2- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

Con el comando *git reflog* copié el identificador del commit que deshice, y luego ejecuté el comando *git reset --hard <ident.commit>. Asi se recuperan archivos borrados o,como en este caso, archivos modificados.

3- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

No, porque en los commit que tienen en común el archivo era el mismo (donde se crea el archivo git-nuestro.md)  y en la rama main no se realizó modificación alguna. Con lo cual, el merge se realizó sin problemas.

4- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

Si, porque el archivo en ambas ramas tienen distintas modificaciones en las mismas líneas.

5- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

No, porque en la rama main el archivo no tenía modificaciones (ídem punto 3) 

6- ¿Qué comando o comandos utilizaste en el paso 25?

*git log --graph --decorate --pretty=oneline*

lo configuré con el alias “graph” para que se ejecuten todos los comandos juntos (*git graph*).

7- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

Si, porque el commit realizado desde la rama <title> quedaba como en “linea” a los commits
 de la rama <main>.
 
8- ¿Qué comando o comandos utilizaste en el paso 27?

Para deshacer el merge sin perder los cambios en el working copy usé *git reset HEAD~1* 

9- ¿Qué comando o comandos utilizaste en el paso 28?

Utilicé el comando que me sugirió git:* git restore git-nuestro.md*

10- ¿Qué comando o comandos utilizaste en el paso 29?

Para eliminar utilicé el comando *git branch -D title*

11- ¿Qué comando o comandos utilizaste en el paso 30?

Comandos para volver al merge: *git reflog* (copio el identificador del commit del merge)
 y *git reset --hard <num identif. del commit>*

12- ¿Qué comando o comandos usaste en el paso 32?

*git checkout <num de identif .del commit inicial>*

13- ¿Qué comando o comandos usaste en el punto 33?

*git checkout \<num de identif. de cuando le puse el titulo al poema\>*


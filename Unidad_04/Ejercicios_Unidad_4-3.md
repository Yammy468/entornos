# Entorno de desarrollo

## Control de versiones

**1).** Además de Git, ¿que otros sistemas de control de versiones existen?

Sistemas de control de versiones más conocidos (además de **Git**):

* CVS 
* Subversion
* Mercurial


**2).** En Git, ¿qué tres áreas existen?

En Git, las áreas que existen son los siguientes:

- Working directory (directorio de trabajo)
- Staging area (área de preparación)
- Repository (directorio de Git)


**3).** Busca en Internet un buen tutorial de GIT y realízalo. ¿De qué tutorial se trata?

Tutorial de git: https://programarfacil.com/blog/arduino-blog/git-y-github/ (Git y Github)

**4).** Visualiza el siguiente video y responde a las cuestiones que aparecen más abajo.

- https://www.youtube.com/watch?v=uR6G2v_WsRA

  

**5).** En Git, ¿para qué sirve el comando `git config`? 

El comando `git config` es una función útil que sirve para definir valores de configuración de Git a nivel de un proyecto global o local. Al ejecutar, se modificará un archivo de texto de configuración.


**6).** En Git, ¿para qué sirve el comando `git init`? 

El comando `git init` crea un nuevo repositorio de Git. Puede convertir un proyecto existente en un repositorio de Git, o para inicializar un nuevo repositorio vacío.


**7).** En Git, ¿para qué sirve el comando `git clone`? 

El comando `git clone` se utiliza principalmente para apuntar a un repositorio existente y clonar o copiar dicho repositorio en un nuevo directorio, en otra ubicación. 


**8).** En Git, ¿para qué sirve el comando `git status`? 

El comando `git status` muestra el estado del directorio de trabajo y del área del entorno de ensayo. Permite ver los cambios que se han preparado, los que no y los archivos en los que Git no va a realizar el seguimiento.


**9).** En Git, ¿para qué sirve el comando `git add`? 

![T4_E9.png](https://github.com/Yammy468/entornos/blob/main/images/T4_E9.png?raw=true)

El comando `git add` añade un cambio del directorio de trabajo en el entorno de ensayo. De este modo, indica a Git que quieres incluir actualizaciones en un archivo concreto en la próxima confirmación.


**10).** En Git, ¿para qué sirve el comando `git commit`? 

![T4_E10.png](https://github.com/Yammy468/entornos/blob/main/images/T4_E10.png?raw=true)

El comando `git commit` sirve para confirmar una instantánea del directorio del entorno de ensayo en el historial de confirmaciones de los repositorios.


**11).** En Git, ¿para qué sirve el comando `git log`? 

El comando `git log` es una herramienta básica de Git para explorar el historial del repositorio. Se usa para buscar una versión concreta de un proyecto o saber los cambios que se introducirán.


**12).** En Git, ¿para qué sirve el comando `git reset HEAD nombrearchivo`? 

![T4_E12.png](https://github.com/Yammy468/entornos/blob/main/images/T4_E12.png?raw=true)

El comando `git reset` HEAD~2 mueve la rama actual hacia atrás dos confirmaciones, eliminando efectivamente las dos instantáneas que acabamos de crear del historial del proyecto. 


**13).** En Git, ¿para qué sirve el comando `git checkout -- nombrearchivo`? 

![T4_E13.png](https://github.com/Yammy468/entornos/blob/main/images/T4_E13.png?raw=true)

El comando `git checkout` te permite navegar entre las ramas creadas por git branch.  Al extraer una rama, se actualizan los archivos en el directorio de trabajo para que coincidan con la versión almacenada en esa rama, y ​​le dice a Git que registre todas las confirmaciones nuevas en esa rama.


**14).** Visualiza el siguiente video y responde a las cuestiones que aparecen más abajo.

- https://www.youtube.com/watch?v=FyAAIHHClqI

  

**15).** En Git, ¿para qué sirve el comando `git branch`? 

El comando `git branch` te permite crear, enumerar y eliminar ramas, así como cambiar su nombre. No te permite cambiar entre ramas o volver a unir un historial bifurcado. Por este motivo, git branch está estrechamente integrado con los comandos git checkout y git merge .


**16).** En Git, ¿para qué sirve el comando `git checkout`? 

El comando `git checkout` te permite navegar entre las ramas creadas por git branch.  Al extraer una rama, se actualizan los archivos en el directorio de trabajo para que coincidan con la versión almacenada en esa rama, y ​​le dice a Git que registre todas las confirmaciones nuevas en esa rama.


**17).** En Git, ¿para qué sirve el comando `git merge`? 

El comando `git merge` se usa para integrar o fusionar las líneas independientes de desarrollo creadas por git branch de una rama con otra rama. 


**18).** En Git, explica cómo funciona la fusión (merge) de tipo fast-forward.

![T4_E18-1.png](https://github.com/Yammy468/entornos/blob/main/images/T4_E18-1.png?raw=true)

![T4_E18-2.png](https://github.com/Yammy468/entornos/blob/main/images/T4_E18-2.png?raw=true)

La herramienta de *Fast Forward* en Git Merge se utiliza para realizar fusiones de avance rápido en las situaciones donde exista un proceso lineal desde el extremo de la rama actual y que se extienda hasta la rama de destino.


**19).** En Git, explica cómo funciona la fusión (merge) de tipo 3-way.

![T4_E19-1.png](https://github.com/Yammy468/entornos/blob/main/images/T4_E19-1.png?raw=true)

![T4_E19-2.png](https://github.com/Yammy468/entornos/blob/main/images/T4_E19-2.png?raw=true)

La fusión de *3-way* se basa en 3 confirmaciones diferentes: 

- El ancestro común.
- La punta de la rama Master.
- La punta de la rama de funciones.

Git identifica estas tres confirmaciones mediante instantáneas. Git compara el ancestro común con cada una de las confirmaciones de punta. 


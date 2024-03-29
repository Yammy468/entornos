# Ejercicios Unidad 6

## Diagramas de casos de uso

**1).** Nombra y describe brevemente los elementos que se utilizan en un diagrama de casos de uso. Busca información si es necesario.

Los elementos de **Diagramas de casos de uso** : 

- **Actores** : es *cualquier entidad que desempeñe un papel* en un sistema determinado. Puede ser una persona, una organización o un sistema externo.

- **Límites del sistema (sujeto)** : refleja los límites o *alcances que abarca* un determinado sistema. Se utiliza para reflejar diferentes áreas dentro del mismo.

- **Casos de uso**  : se utiliza para representar una de las funcionalidades que realiza el  sistema. Es una secuencia de acciones que hace el sistema y que producen un resultado que puede percibir un usuario.

- **Relaciones** :  la interacción entre *dos casos de uso* o de *un actor con un caso de uso* se representa por medio de una relación.  Las principales *relaciones* son: Generalización (Generalization), Inclusión (Include) y Extensión (Extends).

  

  ![Notacion_Caso_de_Uso.png](https://github.com/Yammy468/entornos/blob/main/images/Notacion_Caso_de_Uso.png?raw=true)

**2).** Por cada ejemplo de diagrama de casos de uso que aparece en las diapositivas, realiza su interpretación. Escribe la descripción con tus palabras.

- **Ejemplo 1** :

  ![Ejemplo_1_casos_de_uso.png](https://github.com/Yammy468/entornos/blob/main/images/Ejemplo_1_casos_de_uso.png?raw=true)

   

  ![Ejemplo_1-2_casos_de_uso.png](https://github.com/Yammy468/entornos/blob/main/images/Ejemplo_1-2_casos_de_uso.png?raw=true)  



En un sistema de compra digital se quiere organizar los datos de los clientes que compra online. Todos los clientes, tanto los que están registrados como los que son nuevos, son clientes de la web. 

Todos los clientes pueden ver los artículos de compra siempre y cuando estén autentificados (con un proveedor de identidad, solo los registrados). Pero solo los registrados pueden comprar, los nuevos se tienen  que hacerse cliente para poder hacer las compras. 

Para hacer la compra primero se tiene que autentificarse con un proveedor de identidad y luego acceder a los métodos de pagos, puede ser a traves de pago de crédito o PayPal.

En el método de pago: 

- Para poder acceder a la autentificación de los clientes, se tiene que:

​		=> Autentificarse, se inicia sesión como usuario, guardar/recordar su usuario y luego iniciar su sesión (único).

​		=> Luego pasar por el proveedor de identidad, se identifica con su inicio de sesión único.

- Se puede ver los artículos comprado y/o subir su tarjeta de crédito para poder realizar su compra final/total.

- También incluye los impuestos y los gastos de envió de la compra. 

- Se puede pagar mediante pago de tarjeta de crédito o pago de PayPal.



------



- **Ejemplo 2** :

  ![](https://github.com/Yammy468/entornos/blob/main/images/Ejemplo_2_casos_de_uso.png?raw=true) 



Para hospitalizar en un hospital, se tiene que estar registrado en el hospital que quiere.

Para ello, la recepcionista tiene que acceder a la hospitalización del paciente, y luego al registro del paciente para poder programar el ingreso al hospital del paciente mediante una cita. A parte, el paciente debe presentar a la recepcionista sus informes médicos y los formularios/reclamaciones de seguros.

En la hospitalización del paciente, el paciente puede estar ingresado en el ambulatorio o en los pacientes internados con su camas asignados a cada pacientes.



## Diagramas de secuencia

**1).** Nombra y describe brevemente los elementos que se utilizan en un diagrama de secuencia. Busca información si es necesario.

Los elementos de **Diagramas de secuencia** : 

- **Objetos** : son bloques de construcción básicos de los diagramas UML y representan ciertas características de un elemento del sistema, que varían  dependiendo del diagrama.

- **Líneas de vida** : son *líneas discontinuas* que sale del objeto y avanza en el tiempo desde arriba hacia abajo.

- **Mensajes** : es un elemento con nombre que define un tipo específico de comunicación entre *líneas de vida* de una interacción.

- **Ocurrencias  de Ejecución** : *periodo de tiempo* durante el cual *un objeto* está *en ejecución*.

- **Ocurrencias de destrucción** : *momento* en el cual *un objeto es destruido*.

  

![diagrama_secuencia.png](https://github.com/Yammy468/entornos/blob/main/images/diagrama_secuencia.png?raw=true)



**2).** Por cada ejemplo de diagrama de secuencia que aparece en las diapositivas, realiza su interpretación. Escribe la descripción con tus palabras.

- **Ejemplo 1** :

  ![Ejemplo_1_secuencia.png](https://github.com/Yammy468/entornos/blob/main/images/Ejemplo_1_secuencia.png?raw=true) 



En la librería online, el cliente online/ de la web puede acceder a la librería online o poder comprar en una librería digital. 

Se repite siempre las opciones/actividades:

=> El cliente puede buscar en la librería online, en la que le devuelve el resultado de su búsqueda.

=> El cliente puede optar si quiere ver una resumen o una descripción del libro.

=> También puede optar por si le gusta un libro y añadirlo a la cesta de compra.

Luego se opta para finalizar con un atributo de verificar la compra, por si  ya no quiere comprar el libro.



------



- **Ejemplo 2** :

  ![Ejemplo_2_secuencia.png](https://github.com/Yammy468/entornos/blob/main/images/Ejemplo_2_secuencia.png?raw=true) 



En un sistema de autentificación de usuarios de Facebook, el personal/usuario obtiene su recurso FB para acceder al navegador web con un formulario de permiso. O puede entrar con su permiso de usuario, y luego se accede al servidor de Facebook, después de pasar el proceso de permiso.

Luego desde la web se accede a la aplicación con una solicitud de acceso FB.

O también puede acceder desde la web al servidor de autorización de Facebook con una autorización para permitir su acceso.

Desde el acceso con el usuario, luego de acceder con el permiso de usuario, el sistema tiene como alternativa conceder el permiso de entrada a la aplicación (autentificando el código FB) y luego acceder al servidor de Facebook (autentificando también el código FB) o al servidor de contenido del Facebook (con recurso FB de acceso de usuario protegido). El sistema protege el usuario luego de haber tenido el permiso de entrada.

O desde el acceso con el usuario, como alternativa, cuando no concede el permiso de usuario, el sistema automáticamente, no permite la entrada a la aplicación desde la web.



## Diagramas de estados

**1).** Nombra y describe brevemente los elementos que se utilizan en un diagrama de estados. Busca información si es necesario.

Los elementos de **Diagramas de estados** : 

- **Estados** : es una *situación durante la cual se cumple alguna condición invariante* (generalmente implícita). Esta situación invariante puede representar una situación estática (como un objeto que espera que ocurra algún evento externo o cualquier otra situación). También puede  modelar condiciones dinámicas (como efectuar algún tipo de  comportamiento, es decir, el elemento ingresa al estado cuando el comportamiento comienza y lo deja tan pronto como se completa).

  Los tipos de estados:

  - Simple: aquel que no tiene regiones ni estados de submáquina. 

    ![diagram_de_estado_1.png](https://github.com/Yammy468/entornos/blob/main/images/diagram_de_estado_1.png?raw=true) 

    ![diagram_de_estado_2.png](https://github.com/Yammy468/entornos/blob/main/images/diagram_de_estado_2.png?raw=true) 

  - Compuesto: es aquel que tiene subestados.

    ![diagram_de_estado_2-2.png](https://github.com/Yammy468/entornos/blob/main/images/diagram_de_estado_2-2.png?raw=true) 

  - De submáquina (pseudoestados): se usan generalmente para *conectar múltiples transiciones* en rutas de transición de estado más complejas. Siendo los más comunes los pseudoestados inicial y final.

    ![diagram_de_estado_3.png](https://github.com/Yammy468/entornos/blob/main/images/diagram_de_estado_3.png?raw=true) (Pseudoestado inicial)

     ![diagram_de_estado_4.png](https://github.com/Yammy468/entornos/blob/main/images/diagram_de_estado_4.png?raw=true) (Pseudoestado final)

- **Transiciones**: es una *relación dirigida entre un estado de origen y un estado de destino*. 

  ![diagram_de_estado_5.png](https://github.com/Yammy468/entornos/blob/main/images/diagram_de_estado_5.png?raw=true) 

**2).** Por cada ejemplo de diagrama de estados que aparece en las diapositivas, realiza su interpretación. Escribe la descripción con tus palabras.

- **Ejemplo 1** :

  ![Ejemplo_1_estado.png](https://github.com/Yammy468/entornos/blob/main/images/Ejemplo_1_estado.png?raw=true) 



Para representar los diferentes estados del agua, donde pasa de estado de hielo a liquido, esta a su vez pasa a vapor de agua y que termina en plasma, o también puede ser viceversa.

Primero, desde el estado de hielo puede pasar a ser:

=> Estado liquido, con una transición que *derrite* el hielo y se transforma en agua liquida. Y si es al contrario, la transición se llama *congelación*.

=> Vapor de agua, con una transición que se llama *sublimación*. Y viceversa es *deposición* o cristalización.

Ahora desde el estado liquido puede pasar a ser:

=> Vapor de agua, con una transición denominado *vaporización*. Y viceversa se llama *condensación*.

=> Estado de hielo.

Y además de que el vapor de agua puede pasar a ser estado liquido y estado de hielo, esta también puede ser:

=> Estado de plasma, con la transición de *ionización*, y viceversa, es *desionización*.



------



- **Ejemplo 2** :

  ![Ejemplo_2_estado.png](https://github.com/Yammy468/entornos/blob/main/images/Ejemplo_2_estado.png?raw=true) 



Para ver los estados de una maquinaria de hilos, se hace uso de un diagrama de estado.

El estado se inicia con un nuevo estado que empieza a ejecutarse, y esta a su vez, es decir, dentro de lo ejecutado, se inicia de nuevo y que pasa del estado preparado a corriendo o funcionando, donde se selecciona los hilos por un programador de hilo. Y así pasa se termina el estado de ejecutable y se termina el hilo. También, puede ser viceversa (del estado corriendo a estar preparado), en la que se puede ver el rendimiento del hilo y se suspende el estado por un programador de hilo.

Unas de las alternativas del estado ejecutable es que pase a tiempo de espera, y desde aquí se puede pasar a ejecutable, o bien puede directamente terminar. Y si hay un error se notifica el error y la operación se obstruye.

Otra de las alternativas es que pasa a espera, donde el estado puede pasar a ser obstruido y se notifica el error, o pasa directamente a terminado.

La última alternativa es que pase al estado obstruido y luego a estado ejecutable o se termina/finaliza.



## Diagramas de actividades

**1).** Nombra y describe brevemente los elementos que se utilizan en un diagrama de actividades. Busca información si es necesario.

Los elementos de **Diagramas de actividades** : 

- **Actividades** : es una conducta parametrizada representada como *flujo coordinado de acciones*. Puede ser simple o compuesto.

  ![diagrama_de_actividades_1.png](https://github.com/Yammy468/entornos/blob/main/images/diagrama_de_actividades_1.png?raw=true) 

   ![diagrama_de_actividades_2.png](https://github.com/Yammy468/entornos/blob/main/images/diagrama_de_actividades_2.png?raw=true)

- **Nodos** (acción): es un elemento con nombre que representa un solo paso atómico dentro de la actividad, para hacer una tarea dada.

  - **Nodo final **: detiene todos los flujos en una actividad.

    ![diagrama_de_actividades_6.png](https://github.com/Yammy468/entornos/blob/main/images/diagrama_de_actividades_6.png?raw=true) 

  - **Nodo inicial** : inicia el flujo cuando se invoca la actividad.

    ![diagrama_de_actividades_5.png](https://github.com/Yammy468/entornos/blob/main/images/diagrama_de_actividades_5.png?raw=true) 

  - **Nodo de decisión** : flujo de actividad que pueden usar condiciones para su actuación.

    ![diagrama_de_actividades_3.png](https://github.com/Yammy468/entornos/blob/main/images/diagrama_de_actividades_3.png?raw=true) 

  - **Nodo de fusión** : fusiona dos o más flujos y luego lo emite en un flujo.

    ![diagrama_de_actividades_4.png](https://github.com/Yammy468/entornos/blob/main/images/diagrama_de_actividades_4.png?raw=true) 

  - **Nodo de bifurcación** : divide una acción en flujos concurrentes (se representa con una **barra negra gruesa**).

    ![diagrama_de_actividades_7.png](https://github.com/Yammy468/entornos/blob/main/images/diagrama_de_actividades_7.png?raw=true)  

    Nodo Bifurcación  -----------------------------------------------------  Nodo Unión

  - **Nodo de unión** : recoge flujos concurrentes en una sola acción (se representa con una **barra negra gruesa**).

    

**2).** Por cada ejemplo de diagrama de actividades que aparece en las diapositivas, realiza su interpretación. Escribe la descripción con tus palabras.

- **Ejemplo 1** :

  ![Ejemplo_1_actividades.png](https://github.com/Yammy468/entornos/blob/main/images/Ejemplo_1_actividades.png?raw=true) 



En un sistema de compra online, se inicia la actividad B con un nodo de decisión, que decide entre buscar y navegar en los artículos. Esta se fusiona cuando ya tiene la decisión de buscar artículos, como resultado acaba en otro nodo de decisión, en la que encuentra o no encuentra los artículos seleccionado, y que acaba con poder ver los artículos que ha seleccionado. 

A continuación, puede tomar la decisión de añadirlo a la cesta de compra, en la que toma la decisión de si quiere procesar la actividad B o ver la cesta de la actividad A. Esta última lleva a la acción de ver la cesta de compra y lo dirige a un nodo de decisión, en la cual puede hacer más compra o actualizar la cesta de compra por si quiere cambiar algo, o bien puede finalizar/acabar la compra de la actividad C.

A parte, con una recepción de señal, que comprueba la cesta de compra de la actividad A. Acompañado de una nota, en que la dice que la cesta de compra puede ser comprobado las veces que quiere.

Una vez, comprobado la compra, se procede al pago de los artículos, con otro recepción de señal. Con la cual se fusiona con la actividad C y acaba con al acción de pago, y esta a su vez se finaliza y termina todo el sistema de compra.



------



- **Ejemplo 2** :

  ![Ejemplo_2_actividades.png](https://github.com/Yammy468/entornos/blob/main/images/Ejemplo_2_actividades.png?raw=true) 



Para que funcione el sistema que procesa ordenes, se inicia con que recibe una orden que anteriormente lo solicita. Esta sigue adelante, hasta que tiene que tomar una decisión de que la orden fue aceptada o la orden fue rechazada. Si la orden fue rechazada la acción termina con una orden cerrada  y finaliza todo el proceso. 

Pero si la orden es aceptada, se completa las ordenes recibidas. Luego el flujo de la acción se ramifica/divide en dos flujos paralelos, ambos son para enviar la orden. Una es directamente y la otra pasa por la factura y acaba en la aceptación del pago. Para finalizar, ambos flujos de unen otra vez en un solo flujo, y desde ahí se cierra el orden y finaliza todo.



------



- **Ejemplo 3** :

  ![Ejemplo_3_actividades.png](https://github.com/Yammy468/entornos/blob/main/images/Ejemplo_3_actividades.png?raw=true) 



En un proceso de documentación, tiene que pasar por varios secciones: autor, revisión, aprobador y dueño.

Primero en la sección de autor, donde se inicia la creación de los documentos  o borradores, en la que luego se pasa a la sección de revisión, donde se revisa los borradores. 

A continuación, los documentos revisados son llevado a la sección de aprobador, donde se aprueba los documentos revisado. Esta puede tomar la decisión de si el documento es aprobado o no aprobado. En caso de que el documento no es aprobado, se vuelve a la sección del autor para actualizar los cambios. Pero en caso de que es aceptado, los documentos aprobados/eficaz son revisado de nuevo en la sección de revisión, en que la decide que los documentos necesita cambio o no. 

Si se necesita cambio, el documento de actualiza con los cambios que se le solicitaron en la sección del autor. Pero si no necesita cambio, es decir, que esta obsoleto, pasa a la sección de dueño, en archivado en archivo, y son dominados documentos archivados y finaliza el proceso de documentación.





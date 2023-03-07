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







------



- **Ejemplo 2** :

  ![Ejemplo_2_estado.png](https://github.com/Yammy468/entornos/blob/main/images/Ejemplo_2_estado.png?raw=true) 







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

    Nodo Bifurcación																				Nodo Unión

  - **Nodo de unión** : recoge flujos concurrentes en una sola acción (se representa con una **barra negra gruesa**).

    

**2).** Por cada ejemplo de diagrama de actividades que aparece en las diapositivas, realiza su interpretación. Escribe la descripción con tus palabras.

- **Ejemplo 1** :

  ![Ejemplo_1_actividades.png](https://github.com/Yammy468/entornos/blob/main/images/Ejemplo_1_actividades.png?raw=true) 







------



- **Ejemplo 2** :

  ![Ejemplo_2_actividades.png](https://github.com/Yammy468/entornos/blob/main/images/Ejemplo_2_actividades.png?raw=true) 







------



- **Ejemplo 3** :

  ![Ejemplo_3_actividades.png](https://github.com/Yammy468/entornos/blob/main/images/Ejemplo_3_actividades.png?raw=true) 









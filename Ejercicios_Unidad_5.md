# Ejercicios Unidad 5

## UML

**1).** ¿Qué significan las siglas UML? Busca información acerca de su  historia y las versiones que han existido y el año de publicación.

Las siglas UML significa **Unified Modeling Language** (lenguaje unificado de modelado), es un lenguaje visual de propósito general para representar modelos que pretende proporcionar una forma estándar de representar el diseño de un sistema. En la que dispone de numerosos tipos de diagramas, cada tipo de diagrama tiene diferente modelo.

**Historia** :

El lenguaje UML comenzó a gestarse en octubre de 1994, cuando Rumbaugh se  unió a la compañía Rational fundada por Booch (dos reputados investigadores en el área de metodología del software).

Cuyos objetivo era unificar dos métodos que habían desarrollado: el método Booch y el OMT (Object Modelling Tool ). El primer borrador apareció en octubre de 1995. Más tarde se unió otro reputado investigador, Jacobson, y se icluyeron ideas suyas. Estas tres personas son conocidas como los “*tres amigos*”. Además, este lenguaje se abrió a la colaboración de otras empresas para que aportaran sus ideas. Todas estas colaboraciones condujeron a la definición de la primera versión de UML.

De las tres metodologías de partida: las de Booch y Rumbaugh pueden ser descritas como centradas en objetos (se enfocan hacia el modelado de los objetos) y la metodología de Jacobson es más centrada a usuario (su método se deriva de los escenarios de uso).
Por otro lado, UML se ha ido fomentando y aceptando como estándar desde el OMG. En 1997 UML 1.1 fue aprobada por la OMG convirtiéndose en la notación estándar de facto para el análisis y el diseño orientado a objetos.

**Versiones** :

- Unified Modeling Language (UML) Versión 0.8 y 0.9 (1995)
- Unified Modeling Language (UML) Versión 1.0 y 1.1 (Año 1997)
- Unified Modeling Language (UML) Versión 1.3 (2000)
- Unified Modeling Language (UML) Versión 1.4 (2001)
- Unified Modeling Language (UML) Versión 1.5 (2003)

- Unified Modeling Language (UML) Versión 1.4.2 y 2.0 (Año 2005)
- Unified Modeling Language (UML) Versión 2.1 (2006)
- Unified Modeling Language (UML) Versión 2.1.1 y 2.1.2 (2007)
- Unified Modeling Language (UML) Versión 2.2 (2009)
- Unified Modeling Language (UML) Versión 2.3 (2010)
- Unified Modeling Language (UML) Versión 2.4.1 (2011)
- Unified Modeling Language (UML) Versión 2.5 (2015)

**2).** Indica los tipos de diagramas de estructura que existen en UML.

- **Diagramas de estructura** (aspecto estático):
  - Diagrama de Clases
  - Diagrama de Componentes
  - Diagrama de Objetos
  - Diagrama de Estructura compuesta
  - Diagrama de Despliegue
  - Diagrama de Paquetes

**3).** Indica los tipos de diagramas de comportamiento que existen en UML.

- **Diagramas de comportamiento** (aspecto dinámico):
  - Diagrama de Actividad
  - Diagrama de Casos de uso
  - Diagrama de Maquina de estado
  - Diagrama de Interacción
     - Digrama de Tiempos
     - Diagrama de Secuencias
     - Diagrama de Comunicación
     - Diagrama Global de interacciones


## Diagramas de clases

**1).** Siguiendo la notación UML, pon 2 ejemplos de clases distintos a los vistos en este tema.

![imagen](https://user-images.githubusercontent.com/113978794/212862936-6baddb1b-b2f9-4202-af07-f6d76b342f25.png)

![imagen](https://user-images.githubusercontent.com/113978794/212862986-986b6109-eb59-49ed-adbb-8a00342df41c.png)


**2).** Siguiendo la notación UML, pon 2 ejemplos de interfaces distintos a los vistos en este tema.

![imagen](https://user-images.githubusercontent.com/113978794/212863061-6b8ec5f3-ce28-4f6a-b112-dd3f16a9e710.png)

![imagen](https://user-images.githubusercontent.com/113978794/212863115-9a33e41b-e53b-421b-b5f7-1e80ad73615b.png)


**3).** Indica los tipos de relaciones que pueden darse y explica brevemente.

- **Asociación** : es una relación estructural que describe una conexión entre objetos. Se muestra como una línea continua que une las clases relacionadas entre sí.
  - **Agregación** : es un tipo de asociación más específico que indica que una clase es "parte de" otra clase (composición débil). 
 
  ![imagen](https://user-images.githubusercontent.com/113978794/212854263-8aede102-752a-43c9-95fc-bd012b21a8fa.png)

  - **Composición** : es una forma fuerte de composición donde la vida de la clase contenida debe coincidir con la vida de la clase contenedor. Este tipo de relación se utiliza para representar la dependencia de los objetos de la entidad focal.
  
  ![imagen](https://user-images.githubusercontent.com/113978794/212854394-2682679a-964f-4629-8636-e3d1c0107c40.png)

- **Dependencia** : este es un tipo de relación más débil que se usa cuando un objeto no está contenido en ningún campo.

![imagen](https://user-images.githubusercontent.com/113978794/212854488-49befd73-2a46-466a-afae-f409e6705252.png)

- **Generalización** : se utiliza para representar las relaciones de la clase principal y la clase secundaria. Se puede ver una "especie de" relación entre los clasificadores y cómo una entidad se basa en la otra, heredando los  atributos, las operaciones y las relaciones de los padres.

![imagen](https://user-images.githubusercontent.com/113978794/212854570-b8c09f6f-cbb8-4243-a6ce-f527829a1a6a.png)

- **Realización** : es una relación que vincula dos elementos del modelo con un clasificador realizando el comportamiento de otro clasificador. Esta relación ayuda a comprender cómo afecta la interfaz a la clase de implementación. 

![imagen](https://user-images.githubusercontent.com/113978794/212854672-dc4c0bc7-8a7a-4a6a-8f17-3a71d53b5820.png)


**4).** Siguiendo la notación UML, indica la representación gráfica de las relaciones de la actividad anterior.


## Software

**1).** En Netbeans/IntelliJ, instala el plugin **EasyUML/Diagrama.net**.

![imagen](https://user-images.githubusercontent.com/113978794/212883025-39acac03-45ad-47f4-8e7a-012900825a75.png)


**2).** Escoge uno de tus proyectos realizado en Java que disponga de varias clases. Genera el diagrama de clases haciendo uso del plugin **EasyUML/Diagrama.net**.

![imagen](https://user-images.githubusercontent.com/113978794/212883077-12230680-9dcd-43f8-95b7-154e5ba1a133.png)

![imagen](https://user-images.githubusercontent.com/113978794/212883120-12931f77-d3d9-4500-9bc6-50f9b07bbe88.png)


**3).** Haciendo uso del plugin **EasyUML/Diagrama.net** diseña un proyecto con varias clases y genera el código automáticamente.

![imagen](https://user-images.githubusercontent.com/113978794/212883189-4805c79d-8d98-4af0-9e71-f99d664961bc.png)

![imagen](https://user-images.githubusercontent.com/113978794/212883229-6137f4a5-400d-423e-b527-b82ab5c818ef.png)

![imagen](https://user-images.githubusercontent.com/113978794/212883268-03b96752-087e-46c7-9f81-ed834477b7d3.png)


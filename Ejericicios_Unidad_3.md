# Pruebas

**1)** ¿Qué diferencia existe entre las pruebas estáticas y dinámicas?

La diferencia entre ambos es:

- En las **pruebas estáticas**: las pruebas se realiza sin ejecutar el código de la aplicación. Y se examinan o revisa el código fuente.

- Y en las **pruebas dinámicas**: todas las pruebas se realiza ejecutando el código de la aplicación. También se permite el uso de caja negra y caja blanca con mayor amplitud.

  Y permiten medir el comportamiento de la aplicación desarrollada.

Puedes consultar: https://es.wikipedia.org/wiki/Pruebas_de_software



**2)** ¿Qué diferencia existe entre las pruebas de caja negra y caja blanca?

La diferencia entre ambos es:

* Las pruebas de **caja negra**: son casos de pruebas donde se diseñan considerando exclusivamente las entradas y las salidas del sistema, sin preocuparse de la estructura interna del mismo. En resumen, se estudia el sistema desde fuera. Son *pruebas de funcionalidad*.

  ![pruebas_de_cajas_negras.png.png](https://github.com/Yammy468/entornos/blob/main/images/pruebas_de_cajas_negras.png.png?raw=true)

  

* Las pruebas de **caja blanca**: son casos de pruebas que examina el código fuente y su ejecución. Son *pruebas estructurales*.

  ![pruebas_de_cajas_blancas.png](https://github.com/Yammy468/entornos/blob/main/images/pruebas_de_cajas_blancas.png?raw=true)

Puedes consultar: https://es.wikipedia.org/wiki/Pruebas_de_software



**3)** ¿Qué diferencia existe entre las pruebas funcionales y no funcionales?

La diferencia entre ambos es:

* Las pruebas **funcionales**: es una prueba basada en la ejecución, revisión y retroalimentación de las funcionalidades previamente diseñadas para el software. *Evalúan el cumplimiento de los requisitos funcionales*.
* Las pruebas **no funcionales**: es una prueba cuyo objetivo es la verificación de un requisito que  especifica criterios que pueden usarse para juzgar la operación de un  sistema. *Evalúan aspectos adicionales como rendimiento, seguridad, ...* 

Puedes consultar: https://es.wikipedia.org/wiki/Pruebas_de_software



**4)** Nombra al menos 4 pruebas funcionales.

**Pruebas funcionales**:

- Pruebas unitarias (o de unidad)
- Pruebas de regresión
- Pruebas de integración
- Pruebas del sistema



**5)** Nombra al menos 4 pruebas no funcionales.

**Pruebas NO funcionales**:

- Pruebas de usabilidad
- Pruebas de rendimiento
- Pruebas de seguridad
- Pruebas de compatibilidad



**6)** ¿Qué son las pruebas unitarias o pruebas de unidad?

Las **pruebas unitarias** (o de unidad) consisten en verificar el correcto funcionamiento de las unidades individuales más pequeñas de los programas informáticos. Se utiliza para garantizar que la unidad de código funciona correctamente y cumple con los requisitos especificados.



**7)** ¿Qué son las pruebas de regresión?

Las **pruebas de regresión**: es el proceso de probar un producto de software después de que se hayan realizado cambios para garantizar que no se hayan introducido nuevos errores como resultado de los cambios.



**8)** ¿Qué son las pruebas de integración?

Las **pruebas de integración**: se realizan a continuación de las unitarias, su objetivo es comprobar que todos los elementos unitarios que componen el software, funcionan correctamente cuando cooperan entre sí para realizar las tareas encomendadas al programa.



**9)** ¿Qué son las pruebas de humo?

Las **pruebas de humo**: son una revisión rápida de un producto de software para comprobar que funciona y no tiene defectos evidentes que interrumpan la operación básica del mismo.



**10)** ¿Qué son las pruebas alpha?

Las **pruebas alpha**: es un proceso interno que llevan a cabo los desarrolladores para identificar y corregir errores de software. Esta prueba garantiza que los usuarios obtengan una aplicación libre de fallas y errores al evaluar su calidad y preparación para la prueba Beta.



**11)** ¿Qué son las pruebas beta?

Las **pruebas beta**: es la fase que le sigue a las pruebas alpha, es un proceso que permite verificar y demostrar la calidad de un programa cuando está terminado de forma completa o parcial. En ella involucran a usuarios reales que evalúan el software para proporcionar comentarios sobre la funcionalidad y la usabilidad. 



**12)** ¿Qué son las pruebas de aceptación?

Las **pruebas de aceptación**: son las últimas pruebas realizadas donde el cliente prueba el software, a fin de determinar si cumplen con las necesidades y/o requerimientos de las empresas y sus usuarios.



**13)** Instala el plugin Gradle para Netbeans.

![T03_E13.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E13.png?raw=true)



**14)** Crea un proyecto nuevo de tipo *`Single Gradle Project`* y nombre *`empleado`*, que contenga la clase principal *`Empleado`*. 

![T03_E14-2.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E14-2.png?raw=true)



![T03_E14-1.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E14-1.png?raw=true)



**15)** En *`Sources Packages`* edita el código de la clase *`Empleado`* y en *`Test Packages`* edita el código de la clase *`EmpleadoTest`*. 

Sigue los pasos indicados en el siguiente tutorial:

- https://www.discoduroderoer.es/como-hacer-una-aplicacion-de-prueba-con-junit/

NOTA: En JUnit, el método con anotación *`@BeforeClass`* debe ser estático y, por tanto, las variables y objetos de los que haga uso también deben serlo.

![T03_E15-1.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E15-1.png?raw=true)



![T03_E15-2.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E15-2.png?raw=true)



**16)** Pulsa **`Alt+F6`** para construir y ejecutar las pruebas. 

NOTA: Existen muchas otras tareas que pueden realizarse en Gradle. Sin embargo, la tarea `run` fallará puesto que no existe método `main`.

![T03_E16.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E16.png?raw=true)



**17)** Clona el repositorio https://github.com/jamj2000/DAW1-ED-Pruebas-Ejemplo1 en tu equipo local.

![T03_E17.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E17.png?raw=true)



**18)** Comprueba que en el archivo `build.gradle`  aparece la línea:

```lang-gradle
apply plugin: "jacoco"
```

![T03_E18.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E18.png?raw=true)



**19)** Comprueba que en el archivo `build.gradle`  aparecen también las líneas:

```lang-gradle
jacocoTestReport {
 reports {
     xml.enabled false
     csv.enabled false
     html.destination file("${buildDir}/jacocoHtml")
 }
}
```

![T03_E19.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E19.png?raw=true)



**20)** Ejecuta el comando `gradle tasks` para ver las tareas disponibles.

![T03_E20.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E20.png?raw=true)



**21)** Ejecuta el comando `gradle test` para construir y pasar los tests.

![T03_E21.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E21.png?raw=true)



**22)** Ejecuta el comando `gradle jacocoTestReport` para generar informe de cobertura de código.
Para visualizar dicho informe ejecuta `firefox build/jacocoHtml/index.html`.

![T03_E22.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E22.png?raw=true)



**23)** Modifica y añade los tests necesarios para que la cobertura de código sea completa.

![T03_E23-1.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E23-1.png?raw=true)



![T03_E23-2.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E23-2.png?raw=true)



**24)** Modifica el código fuente de la clase `Utilidades.java` para solucionar los errores que aparecen y superar los tests.

![T03_E24.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E24.png?raw=true)



#  Integración

**1)** ¿Indica al menos 3 servicios web de Integración Continua?

**Servicios web de Integración Continua**:

- Jenkins
- Bamboo
- TravisCI



**2)** En GitHub, haz un fork del repositorio https://github.com/jamj2000/DAW1-ED-Pruebas-Ejemplo1.

![T03_E2-Integracion.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E2-Integracion.png?raw=true)



**3)** Edita el archivo `.travis.yml` de tu repositorio bifurcado, en caso de ser necesario.

![T03_E3-Integracion.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E3-Integracion.png?raw=true)



**4)** Regístrate con tu cuenta de GitHub en TravisCI (https://travis-ci.org/)

![T03_E4-1-Integracion.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E4-1-Integracion.png?raw=true)



![T03_E4-2-Integracion.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E4-2-Integracion.png?raw=true)



**5)** En TravisCI, añade tu repositorio remoto (bifurcado) para construir y realizar los tests en dicho sitio web. 

![T03_E5-1-Integracion.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E5-1-Integracion.png?raw=true)



**6)** En TravisCI, haz click en el ***badge\*** o insignia que aparece en la parte superior derecha, y copia el código en formato Markdown.

[![Build Status](https://app.travis-ci.com/Yammy468/DAW1-ED-Pruebas-Ejemplo1.svg?branch=master)](https://app.travis-ci.com/Yammy468/DAW1-ED-Pruebas-Ejemplo1) 



**7)** En GitHub, en tu repositorio bifurcado, copia el código Markdown anterior en el archivo README.md.

![T03_E7-Integracion.png](https://github.com/Yammy468/entornos/blob/main/images/T03_E7-Integracion.png?raw=true)



**8)** [**Opcional. Vale por 1 pto en la nota de esta Unidad**]
En una plataforma Linux (preferiblemente Ubuntu), realiza la instalación  de un servicio de Integración Continua basado en Jenkins.
Explica los pasos seguidos y elabora un documento PDF donde quede reflejado todo el proceso y las pruebas que has realizado.

Deberás seguir los pasos indicados en el enlace de instrucciones que aparece a continuación.
INSTRUCCIONES: https://yeiei.net/es/como-construir-un-entorno-de-integracion-continua-con-jenkins-y-docker/



#  Calidad

**1)** ¿Qué significan las siglas QA y QC? ¿Qué diferencia existe entre ellas?

* **QA = Quality Assurance.**

  QA es un conjunto de actividades para garantizar la **calidad en los procesos** mediante los cuales se desarrollan los productos.

* **QC = Quality Control.**

  QC es un conjunto de actividades para garantizar **la calidad de los productos**. Las actividades se centran en identificar defectos en los productos reales producidos.


**2)** Explica brevemente cada uno de los factores de calidad que aparecen en las diapositivas.

**Factores de calidad**:

- *Correción*: el software cumple las especificaciones.
- *Fiabilidad*: grado en el que el software es confiable, es decir, no tiene fallos.
- *Eficiencia*: cantidad de recursos hardware y software que necesita un producto para realizar las operaciones.
- *Seguridad*: grado en el que puede controlarse el acceso al software y a los datos.
- *Facilidad de uso*: grado de esfuerzo necesario para utilizar el software.
- *Mantenibilidad*: esfuerzo requerido para localizar y reparar errores.
- *Flexibilidad*: esfuerzo necesario para modificar un programa en funcionamiento.
- *Facilidad de prueba*: esfuerzo requerido para probar un programa de forma que cumpla con lo especificado en los requisitos.
- *Portabilidad*: facilidad para transferir la aplicación a otro hardware o sistema operativo.
- *Reusabilidad*: grado en el que un programa o parte del mismo se puede utilizar en otras aplicaciones.
- *Interoperatividad*: esfuerzo necesario para que un software opere o comunique conjuntamente con otros sistemas.



 



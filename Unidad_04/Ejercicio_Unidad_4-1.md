# Ejercicios Unidad 4

## Optimización

**1).** ¿Qué se entiende por hediondez del código? Pon al menos 5 ejemplos.

La **hediondez del código** (***code smell*** en inglés) es cualquier síntoma en el código fuente de un programa que posiblemente indica un problema más profundo. Las hediondeces del código usualmente no son bug de programación (errores): no son técnicamente incorrectos y no impiden que el programa funcione correctamente. Mas bien, indican deficiencias  en el diseño de software que puede ralentizar el desarrollo o aumentan el riesgo de errores o fallos en el futuro.

Ejemplos:

* Checkstyle
* PMD 
* FindBugspara Java
* LibreríasReek 
* Cane


**2).** ¿Qué tipo de herramienta utilizamos para hacer análisis estático del código?

Tipos de herramientas:

* Linters

* Continuous Inspection o Continuous Analysis


**3).** ¿Qué sitios web nos permiten hacer análisis estático del código o **Continuous Inspection**?

Sitios web:

* Scrutinizer

* SonarQube


**4).** Instala en Netbeans/IntelliJ el plugin **FindBugs/SpotBugs**, si no lo tienes aún instalado.

![imagen](https://user-images.githubusercontent.com/113978794/211783961-839adcd3-49f6-4c8e-a965-1617ea01cedf.png)

![imagen](https://user-images.githubusercontent.com/113978794/211801034-69db1e8e-1f1c-4fd0-b840-2e47e0bcf42d.png)


**5).** Realiza **análisis estático de código** para las clases del proyecto *miapp*. Consulta el siguiente enlace: [análisis estático con FindBugs](https://github.com/jamj2000/DAW1-ED-Pruebas-Ejemplo1#análisis-estático-de-código-con-findbugs-en-netbeans)

![imagen](https://user-images.githubusercontent.com/113978794/211816991-ffcd2d4d-a7dc-4d2e-9054-ebd0ebf31bcc.png)

![imagen](https://user-images.githubusercontent.com/113978794/211817037-645ac42d-a4b4-4be4-99a5-dbaec99ab0ca.png)



**6).** Indica al menos un `code smell` relevante de cada clase. Explica cómo podría solucionarse.

* Análisis dinámico: unit tests

* Análisis estático: lint


**7).** ¿Qué es la refactorización?

Es el proceso de reestructurar un código fuente, alterando su estructura interna sin cambiar su comportamiento externo.


**8).** ¿Qué técnicas se utilizan a menudo a la hora de refactorizar?

Técnicas:

- Renombrado de variables

- Pasar código duplicado a funciones

- Eliminación de código inalcanzable

- Eliminación de código redundante

- Eliminación de código muerto

  


# Entorno de desarrollo

## Heramientas de desarrollo

**1).** Ejecuta el programa "Hola mundo" en los siguientes lenguajes:

- bash
- python
- php
- javascript (nodejs)
- C
- C++
- java
- ruby
- go
- rust
- lisp
- ensamblador (nasm)

<img src="https://github.com/Yammy468/entornos/blob/main/images/T2_E1-1.png?raw=true" alt="T2_E1-1" style="zoom:80%;" />
<img src="https://github.com/Yammy468/entornos/blob/main/images/T2_E1-2.png?raw=true" />
<img src="https://github.com/Yammy468/entornos/blob/main/images/T2_E1-3.png?raw=true" />

Los paquetes a instalar en Ubuntu son: `python`, `php`, `nodejs`, `gcc`, `g++`, `openjdk-8-jdk`, `ruby`, `golang`, `rustc` , `clisp` y `nasm`.

El código fuente para distintos lenguajes de programación está disponible en: https://es.wikipedia.org/wiki/Anexo:Ejemplos_de_implementaci%C3%B3n_del_%C2%ABHola_mundo%C2%BB

Instrucciones en https://github.com/jamj2000/DAW1-ED-HolaMundo.



**2).** Para cada uno de los lenguajes anteriores, indica el proceso realizado para conseguir ejecutar el código: ¿compilación o interpretación?

- bash  --->  interpretación 
- python  --->  interpretación 
- php  --->  interpretación 
- javascript (nodejs)  --->  interpretación 
- C  --->  compilación 
- C++  --->  compilación 
- java  --->  compilación 
- ruby  --->  interpretación 
- go  --->  compilación 
- rust  --->  compilación 
- lisp  --->  interpretación 
- ensamblador (nasm)  --->  compilador cruzado 



**3).** Para cada uno de los lenguajes anteriores, indica el nombre del compilador o interprete utilizado en GNU/Linux.

- bash  --->  SCRIPTS
- python  --->  CPYTHON 
- php  --->  NETBEANS 
- javascript (nodejs)  --->  GCC 
- C  --->  GCC 
- C++  --->  GCC 
- java  --->  JAVAC
- ruby  --->  compilador JIT 
- go  --->  GO BUILD 
- rust  --->  RUSTC
- lisp  --->  CAR/ CDR
- ensamblador (nasm)  --->  GCC 



**4).** Investiga y averigua que extensión tienen los archivos de código fuente de los siguientes lenguajes:

   - bash = ``` .sh```
   - python = ``` .py```
   - php = ``` .php```
   - javascript = ``` .js```
   - C = ``` .c```
   - C++ = ``` .cpp```
   - java = ``` .java```
   - ensamblador (nasm) = ``` .asm```
   - ruby = ``` .rb```
   - go = ``` .go```
   - rust = ``` .rs```
   - lisp= ``` .lisp```



**5).** Scripts ejecutables para los lenguajes interpretados. Edita los scripts para los siguientes lenguajes:

   - bash
   - python
   - php
   - javascript
   - java
   - ruby
   - go
   - rust
   - lisp

![image](https://user-images.githubusercontent.com/113978794/195017507-6835b31b-95fe-4ce6-8258-b3b2846939d5.png) 

![image](https://user-images.githubusercontent.com/113978794/195017734-4f1f2258-ea15-41f0-908f-17f6a1621d48.png)


Instrucciones en https://github.com/jamj2000/DAW1-ED-HolaMundo.



**6).** ¿Qué extensión tienen los archivos de código objeto?

Los archivo la de código objeto tiene extensión ``` .obj```
.

**7).** Lenguaje C. Código en varios archivos. Obtener el código objeto a partir del código fuente de los 3 archivos siguientes:

```lang-c
//-------------
// datos.c
//-------------

char *mensaje="Hola a todos y todas";
int  num1 = 8;
int  num2 = 10; 
```

```lang-c
//-------------
// suma.c
//-------------

int suma (int a, int b) {
  return a + b;
}
```

```lang-c
//-------------
// main.c
//-------------

/#include <stdio.h>

int suma (int a, int b);

extern char *mensaje;
extern int  num1, num2;

int main(){
  printf("%s\n", mensaje);
  printf("%d\n", suma (num1, num2) );
  return 0;
}
```

```lang-c
# Para obtener código objeto

gcc  -c  main.c  datos.c  suma.c
```

Deberemos obtener 3 archivos:  `main.o`,  `suma.o`  y `datos.o`

![image](https://user-images.githubusercontent.com/113978794/195024456-d1283e50-2ff2-49b1-a32a-346199d87855.png)


**8).** Lenguaje C. Código en varios archivos. Obtener el código binario ejecutable a partir del código objeto de los 3 archivos anteriores:

```lang-c
# Para obtener código binario

gcc  -o  programa  main.o  datos.o  suma.o
```

Deberememos obtener un archivo `programa` binario ejecutable. Si lo ejecutamos obtenemos el siguiente resultado:

```lang-c
./programa
Hola a todos y todas
18
```

![image](https://user-images.githubusercontent.com/113978794/195024540-a115644a-d2c7-4d13-b6cc-33bf8a66fc68.png)




## Bibliotecas

**11).** Bibliotecas. Define que se entiende por biblioteca o librería y los tipos que existen.

En este sentido, una biblioteca o librería es un conjunto de archivos que se utiliza para desarrollar software. Suele estar compuesta de código y datos, y su fin es ser utilizada por otros programas de forma totalmente autónoma. 
- Biblioteca estática.
- Bibliotecas dinámica.


**12).** Bibliotecas. ¿Qué tipo es el más utilizado actualmente? ¿Por qué?

La más utilizada son las bibliotecas dinámicas (.DLL o .so) (.jar en Java). Ejemplos de librerías más usados: JavaScript, C++ y Python.
Porque facilitan la gestión y aprovechamiento de la memoria del sistema. Permite al sistema operativo aplicar algoritmos que mejoren el rendimiento del sistema cuando se carguen estas bibliotecas. Además, al estar compartidas, basta con mantener una copia en memoria para todos los programas que la utilicen.

Más información en https://github.com/jamj2000/DAW1-ED-Bibliotecas


**13).** Bibliotecas. Crea una biblioteca dinámica en C que proporcione  las funciones para sumar, restar, multiplicar y dividir 2 números  enteros. Crea un programa que haga uso de ella y comprueba que se ejecuta  correctamente.

Instrucciones en https://github.com/jamj2000/DAW1-ED-Bibliotecas

![image](https://user-images.githubusercontent.com/113978794/195039740-b90174f1-dce7-425f-9f74-bdf287751fd9.png)


**14).** Bibliotecas. Crea una biblioteca dinámica en Java que proporcione las funciones para sumar, restar, multiplicar y dividir 2 números  enteros. Crea un programa que haga uso de ella y comprueba que se ejecuta  correctamente.

Instrucciones en https://github.com/jamj2000/DAW1-ED-Bibliotecas

![image](https://user-images.githubusercontent.com/113978794/195039800-b45a75e7-4993-46fd-b732-c91c39149d24.png)


**15).** Bibliotecas. Busca información y explica las ventajas y desventajas de usar bibliotecas estáticas.

*Ventaja*:
- No es necesario proporcionar las bibliotecas correspondientes al publicar el programa.
- Biblioteca de carga rápida.

*Desventaja*: 
- La biblioteca está empaquetada en la aplicación, lo que resulta en una gran biblioteca.
- La biblioteca ha cambiado y es necesario volver a compilar el programa.


**16).** Bibliotecas. Busca información y explica las ventajas y desventajas de usar bibliotecas dinámicas.

*Ventajas*:
1. La programación se centra completamente en la esencia del diseño del programa, se mejora la simplicidad del código y la eficiencia del desarrollo.
2. Debido a que la escala del programa se reduce, la inteligibilidad del programa también se mejora.

*Desventajas*:
1. La velocidad de ejecución del programa es lenta debido al lenguaje de tipo dinámico, la verificación de tipo se realiza en tiempo de ejecución. 
2. No se pueden detectar errores sin ejecución. 




## Buildfile

**17).** Build. Automatiza el proceso de compilación de ejecutable y  biblioteca, su enlazado y la generación del archivo ejecutable para  código fuente en C con make. Haz uso de un buildfile.    

Instrucciones en https://github.com/jamj2000/DAW1-ED-Bibliotecas/blob/master/Build.md 

![imagen](https://user-images.githubusercontent.com/113978794/195527682-f70cf53b-9e8a-4423-bf0f-7659865e46d7.png)


**18).** Build. Automatiza el proceso de compilación de ejecutable y  biblioteca, su enlazado y la generación del archivo .jar para código  fuente en Java con Ant. Haz uso de un buildfile.    

Instrucciones en https://github.com/jamj2000/DAW1-ED-Bibliotecas/blob/master/Build.md 

![imagen](https://user-images.githubusercontent.com/113978794/195527749-ad625172-02b3-469a-9b71-89e80d834049.png)

![imagen](https://user-images.githubusercontent.com/113978794/195527798-0450b382-e6b6-428c-9532-b6268198e9d3.png)


**19).** Build. Automatiza el proceso de compilación de ejecutable y  biblioteca, su enlazado y la generación del archivo .jar para código  fuente en Java con Maven. Haz uso de un buildfile.    

Instrucciones en https://github.com/jamj2000/DAW1-ED-Bibliotecas/blob/master/Maven.md 



**20).** Build. Automatiza el proceso de compilación de ejecutable y  biblioteca, su enlazado y la generación del archivo .jar para código  fuente en Java con Gradle. Haz uso de un buildfile.    

Instrucciones en https://github.com/jamj2000/DAW1-ED-Bibliotecas/blob/master/Gradle.md 


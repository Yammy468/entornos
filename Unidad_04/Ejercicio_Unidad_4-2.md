# Entorno de desarrollo

## Documentación

**0.1).** Genera la documentación técnica de Javadoc para el codigo fuente de algún ejercicio Java que hayas realizado en clase.

```java
 /**
  * Inserta un título en la clase descripción.
  * Al ser el título obligatorio, si es nulo o vacío se lanzará
  * una excepción.
  *
  * @param titulo El nuevo título de la descripción.
  * @throws IllegalArgumentException Si titulo es null, está vacío o contiene sólo espacios.

  */
 public void setTitulo (String titulo) throws IllegalArgumentException
 {
   if (titulo == null || titulo.isBlank())
   {
       throw new IllegalArgumentException("El título no puede ser nulo o vacío");
   }
   else
   {
       this.titulo = titulo;
   }
 }
```

**0.2).** En tu repositorio "Apuntes-ED" de GitHub, crea un archivo `SUMMARY.md` con un contenido similar al siguiente:

```lang-markdown
# Summary

* [Unidad 1: Elementos de desarrollo del software](1.ELEMENTOS.md)    
* [Unidad 2: Entornos integrados de desarrollo](2.ENTORNOS.md)  
* [Unidad 3: Diseño y realización de prueba](3.PRUEBAS.md)  
* [Unidad 4: Documentación y optimización](4.DOCUMENTACION.md)  
* [Unidad 5: Elaboración de diagramas de clases](5.DIAGRAMAS_CLASES.md)  
* [Unidad 6: Elaboración de diagramas de comportamiento](6.DIAGRAMAS_COMPORTAMIENTO.md)
```

Esto nos servirá más adelante para generar la tabla de contenido de un futuro libro en GitBook.


**0.3).** En tu repositorio "Apuntes-ED" de GitHub, crea otro archivo `book.json` con el siguiente contenido:

```lang-json
{
 "gitbook": "3.x.x",
 "plugins" : [
     "include-codeblock",
     "ace"
 ],
 "pluginsConfig": {
     "include-codeblock": {
        "template":"acefull",
        "unindent": true
     }
 }
}
```

Esto nos servirá más adelante para el coloreado de código fuente de un futuro libro en GitBook.


**1).** Ahora vamos a generar un libro en distintos formatos (PDF, Mobi y ePub) para tus apuntes de ED. Para ello registrate en https://www.gitbook.com con tu cuenta de GitHub.

![imagen](https://user-images.githubusercontent.com/113978794/208885631-2066235b-dd40-4d46-b1b9-e4e4b2445827.png)


**2).** Inicia sesión de GitBook y pulsa en "+New Book" y después en "Book & Manual". Rellena los campos de "Title" y "Description". Finalmente pulsa en "Create Book".

![imagen](https://user-images.githubusercontent.com/113978794/208886095-c8cf7e9c-bbdb-409a-a6f8-f2189812749b.png)


**3).** Pulsa en el logotipo que aparece en la parte superior izquierda  para ir a la página principal de GitBook. Luego, en la sección referida  al libro que has creado, pulsa en la flecha que aparece al lado de  "Edit" y después en "Settings".

![T04_E3.png](https://github.com/Yammy468/entornos/blob/main/images/T04_E3.png?raw=true)


**4).** Después pulsa en "GitHub" y "Select a Repository" y marca tu repositorio "Apuntes-ED" y finalmente "Sync".

![T04-E4-1.png](https://github.com/Yammy468/entornos/blob/main/images/T04-E4-1.png?raw=true)

![T04-E4-2.png](https://github.com/Yammy468/entornos/blob/main/images/T04-E4-2.png?raw=true)

![imagen](https://user-images.githubusercontent.com/113978794/208886269-fd27cabc-1eef-4dd5-956f-f0195591668b.png)


**5).** Para ver y descargar el resultado en distintos formatos (PDF,  Mobi y ePub) vuelve a la página principal pinchando en el logotipo que  aparece en la parte superior izquierda. Y después pulsa en el título del libro.

![imagen](https://user-images.githubusercontent.com/113978794/208886410-d7a55b2e-3e83-4442-a781-73392759aea0.png)


**6).** Verás un botón para descargar el libro en distintos formatos. Haz una descarga del libro en formato PDF.

![T04-E6.png](https://github.com/Yammy468/entornos/blob/main/images/T04-E6.png?raw=true)

![imagen](https://user-images.githubusercontent.com/113978794/208886481-b83ac6b8-e445-47ce-bfbf-bcbc91c5a40c.png)



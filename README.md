# ficherosss
FICHEROS APE 5
# APE 5 – Primera parte: Manejo de ficheros en Java

## Datos del estudiante

| | |
|---|---|
| **Estudiante** | Andres Vayas |
| **Carrera** | Ingeniería en Software |
| **Curso** | 1ero B |
| **Docente** | Ing. José Rubén Caiza Caizabuano |

## Descripción

Desarrollo individual de los 3 ejercicios de la actividad APE 5, usando las clases `File`, `FileWriter` y `Scanner` para crear, escribir y eliminar ficheros en Java.

## Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `Ejercicio1.java` | Crea el archivo `curso.txt` y comprueba si se creó o ya existe. |
| `Ejercicio2.java` | Lee un mensaje por teclado y lo agrega al final de `estudiantes.txt`. |
| `Ejercicio3.java` | Elimina el archivo `estudiantes.txt` y confirma el resultado. |

## Ejercicio 1. Crear un fichero
- Clases y métodos: `File`, `IOException`, `createNewFile()`, `getName()`.
- Muestra un mensaje si el archivo se creó o si ya existía.
- Usa `try-catch` para controlar errores.

## Ejercicio 2. Escribir información en un fichero
- Clases y métodos: `Scanner`, `FileWriter`, `IOException`, `write()`, `close()`.
- Usa `new FileWriter("estudiantes.txt", true)` para **conservar** la información anterior y agregar el mensaje al final.
- **Importante:** `estudiantes.txt` debe existir antes de ejecutar este programa.

## Ejercicio 3. Eliminar un fichero
- Clases y métodos: `File`, `delete()`, `if-else`, `System.out.println()`.
- Muestra un mensaje de confirmación si se eliminó, o un aviso si no fue posible.

## Cómo ejecutar

Requiere tener instalado el JDK (Java 11 o superior).

```bash
# Compilar
javac Ejercicio1.java Ejercicio2.java Ejercicio3.java

# Ejecutar en este orden
java Ejercicio1        # crea curso.txt
touch estudiantes.txt  # (Windows: type nul > estudiantes.txt)
java Ejercicio2        # agrega un mensaje a estudiantes.txt
java Ejercicio3        # elimina estudiantes.txt
```

## Ejemplo de salida

```text
Archivo creado correctamente: curso.txt
Escriba un mensaje: Hola, soy un estudiante
La información se guardó correctamente en estudiantes.txt
El archivo estudiantes.txt se eliminó correctamente.
```

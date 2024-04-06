# Teoría de Lenguajes de Programación - Programación Funcional en Racket 🚀

## Proyecto 2 - Equipo 6

**Integrantes:**
1. Canto Paredes Eduardo Alexander
2. González Álvarez María Fernanda
3. González Aranda Mario Joel

*Descripción:*
Este proyecto consiste en la implementación de un conjunto de ejercicios en el paradigma de programación funcional, utilizando el lenguaje Racket dentro de un entorno Jupyter Notebook. Los ejercicios abarcan desde operaciones matemáticas básicas hasta la manipulación de estructuras de datos complejas, demostrando la potencia y flexibilidad de la programación funcional.

---

## Contenido

1. [¿Qué es Jupyter Notebook?](#qué-es-jupyter-notebook)
2. [Qué es Racket?](#qué-es-racket)
   1. [iRacket](#iracket)
2. [Instalar Python](#instalar-python)
   1. [Descargar Python de la página oficial](#descargar-python-de-la-página-oficial)
   2. [Verifique que Python esté agregado en PATH](#verifique-que-python-esté-agregado-en-path)
   3. [Verifique que pip se haya instalado correctamente](#verifique-que-pip-se-haya-instalado-correctamente)
3. [Instalar Racket y iRacket](#instalar-racket)
   1. [Descargar Racket de la página oficial](#descargar-racket-de-la-página-oficial)
   2. [Verifique que Racket esté agregado en PATH](#verifique-que-racket-esté-agregado-en-path)
   3. [Instalando y registrando la biblioteca iRacket](#instalando-la-biblioteca-iracket)
4. [Instalar Jupyter](#instalar-jupyter)
5. [Configuración de Jupyter](#configuración-de-jupyter)
6. [Ejecución de Jupyter Notebook](#ejecución-de-jupyter-notebook)
7. [Crea un Notebook](#crea-un-notebook)
8. [Abra el Notebook del proyecto](#abra-el-notebook-del-proyecto)
9. [Descripción y ejecución](#descripción-y-ejecución)
   1. [Factorial de N](#factorial-de-n)
   2. [Fibonacci](#fibonacci)
   3. [Torres de Hanoi](#torres-de-hanoi)
   4. [Multiplicación Entera](#multiplicación-entera)
   5. [Exponenciación Entera](#exponenciación-entera)
   6. [Máximo Común Divisor](#máximo-común-divisor)
   7. [Número Mayor](#número-mayor)
   8. [Número Menor](#número-menor)
   9. [Número Combinatorio](#número-combinatorio)
   10. [Reversa de una Lista](#reversa-de-una-lista)
10. [Comentarios Grupales](#comentarios-grupales)
11. [Referencias Bibliográficas](#referencias-bibliográficas)

---

## ¿Qué es Jupyter Notebook?

Jupyter Notebook es un entorno de trabajo interactivo web que permite desarrollar código en Python de manera dinámica, a la vez que integrar en un mismo documento tanto bloques de código como texto, gráficas o imágenes. Te permite editar y ejecutar documentos de notebook a través de cualquier navegador web, e incluso dentro de Pycharm.

## ¿Qué es Racket?

Racket es un lenguaje de programación de amplio espectro de la familia de Lisp y Scheme. Uno de sus principales objetivos tras su diseño es posibilitar la creación de nuevos lenguajes o dialectos. El lenguaje es usado en una variedad de entornos tales como scripting, enseñanza en ingeniería informática o la investigación.

La plataforma nos ofrece la herramienta `DrRacket`, un entorno de desarrollo integrado programado en Racket, que nos facilitará la tarea de programar en Racket. También nos ofrece `raco`, un herramienta para la línea de comandos que nos permitirá instalar paquetes o compilar librerías.

### iRacket

iRacket es una implementación del kernel de Racket para Jupyter, lo que permite la programación interactiva estilo bloc de notas con Racket. Esta biblioteca facilita la creación de documentos interactivos que combinan código ejecutable y visualizaciones en un solo lugar. Con iRacket, los usuarios pueden aprovechar las capacidades de Jupyter para explorar y experimentar con código Racket de manera fluida y colaborativa.

## Instalar Python

Para instalar Jupyter Notebook es necesario que su computadora tenga instalado Python, y este se encuentre agregado al _PATH_ de Windows.

### Descargar Python de la página oficial

1. Visitar [https://www.python.org/](https://www.python.org/).
2. Ir a la pestaña de descargas y seleccionar la versión deseada.
3. Ejecutar el archivo .exe descargado, asegurándose de seleccionar la opción "Add Python.exe to PATH" durante la instalación.

### Verifique que Python esté agregado en PATH

Para verificar, puede usar la consola (cmd en Windows, Terminal en Mac) e ingresar el comando `python`. Si Python está correctamente instalado y en PATH, se abrirá el intérprete de Python. De lo contrario, es probable que le aparezca el mensaje:

```
'python' is not recognized as an internal or external command, operable program or batch file.
```
Si su caso es el segundo, visite esta página: [Agregar Python al PATH](https://www.scielo.org.mx/avaliacao/manual_marcacion/instalacion_markup_paths.html)

### Verifique que pip se haya instalado correctamente

`pip` es necesario para la instalación de Jupyter. Para verificar su instalación, use el comando `python -m pip --version` en la consola.

## Instalar Racket y iRacket



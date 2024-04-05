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
2. [Instalar Python](#instalar-python)
   1. [Descargar Python de la página oficial](#descargar-python-de-la-página-oficial)
   2. [Verifique que Python esté agregado en PATH](#verifique-que-python-esté-agregado-en-path)
3. [Verifique que pip se haya instalado correctamente](#verifique-que-pip-se-haya-instalado-correctamente)
4. [Instalar Jupyter](#instalar-jupyter)
5. [Configuración de Jupyter](#configuración-de-jupyter)
6. [Ejecución de Jupyter Notebook](#ejecución-de-jupyter-notebook)
   1. [Activar autollenado de código](#activar-autollenado-de-código)
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
9. [Comentarios Grupales](#comentarios-grupales)
10. [Referencias Bibliográficas](#referencias-bibliográficas)

---

## ¿Qué es Jupyter Notebook?

Jupyter Notebook es un entorno de trabajo interactivo web que permite desarrollar código en Python de manera dinámica, a la vez que integrar en un mismo documento tanto bloques de código como texto, gráficas o imágenes. Te permite editar y ejecutar documentos de notebook a través de cualquier navegador web, e incluso dentro de Pycharm.

## Instalar Python

Para instalar Jupyter Notebook es necesario que su computadora tenga instalado Python, y este se encuentre agregado al _PATH_ de Windows.

### Descargar Python de la página oficial

1. Visitar [https://www.python.org/](https://www.python.org/).
2. Ir a la pestaña de descargas y seleccionar la versión deseada.
3. Ejecutar el archivo .exe descargado, asegurándose de seleccionar la opción "Add Python.exe to PATH" durante la instalación.

### Verifique que Python esté agregado en PATH

Para verificar, puede usar la consola (cmd en Windows, Terminal en Mac) e ingresar el comando `python`. Si Python está correctamente instalado y en PATH, se abrirá el intérprete de Python. De lo contrario, es probable que le aparezca el mensaje `'python' is not recognized as an internal or external command, operable program or batch file`. Si su caso es el segundo, visite esta página: [Agregar Python al PATH](https://www.scielo.org.mx/avaliacao/manual_marcacion/instalacion_markup_paths.html)

### Verifique que pip se haya instalado correctamente

`pip` es necesario para la instalación de Jupyter. Para verificar su instalación, use el comando `python -m pip --version` en la consola.


# Teoría de Lenguajes de Programación - Programación Funcional en Racket 🚀

## Proyecto 2 - Equipo 6

**Integrantes:**
1. Canto Paredes Eduardo Alexander
2. González Álvarez María Fernanda
3. González Aranda Mario Joel

*Descripción:*
Este proyecto consiste en la implementación de un conjunto de ejercicios en el paradigma de programación funcional, utilizando el lenguaje Racket dentro de un entorno Jupyter Notebook. Los ejercicios abarcan desde operaciones matemáticas básicas hasta la manipulación de estructuras de datos complejas, demostrando la potencia y flexibilidad de la programación funcional.

---

## Contenido 🔎

1. [¿Qué es Jupyter Notebook?](#qué-es-jupyter-notebook)
2. [Qué es Racket?](#qué-es-racket)
   1. [iRacket](#iracket)
2. [Instalar Python](#instalar-python)
   1. [Descargar Python de la página oficial](#descargar-python-de-la-página-oficial)
   2. [Verifique que Python esté agregado en PATH](#verifique-que-python-esté-agregado-en-path)
   3. [Verifique que pip se haya instalado correctamente](#verifique-que-pip-se-haya-instalado-correctamente)
3. [Instalar Racket y iRacket](#instalar-racket-y-iracket)
   1. [Descargar Racket de la página oficial](#descargar-racket-de-la-página-oficial)
   2. [Verifique que Racket esté agregado en PATH](#verifique-que-racket-esté-agregado-en-path)
   3. [Instalando y registrando la biblioteca iRacket](#instalando-y-registrando-la-biblioteca-iracket)
4. [Instalar Jupyter](#instalar-jupyter)
5. [Ejecución de Jupyter Notebook](#ejecución-de-jupyter-notebook)
6. [Crea un Notebook](#crea-un-notebook)
7. [Abra el Notebook del proyecto](#abra-el-notebook-del-proyecto)
8. [Descripción y ejecución](#descripción-y-ejecución)
   1. [Número Combinatorio](#número-combinatorio)
   2. [Máximo Común Divisor de Números Negativos](#máximo-común-divisor-de-números-negativos)
   3. [Generación de Lista de Números Primos](#generación-de-lista-de-números-primos)
   4. [Búsqueda en Lista](#búsqueda-en-lista)
   5. [Inversión de Lista](#inversión-de-lista)
   6. [Eliminación de Elemento de una Lista](#eliminación-de-elemento-de-una-lista)
   7. [Detección de Palíndromos](#detección-de-palíndromos)
   8. [Suma de Dígitos](#suma-de-dígitos)
   9. [Conversión de Decimal a Binario](#conversión-de-decimal-a-binario)
   10. [Cálculo de PI mediante la Serie de Leibniz](#cálculo-de-pi-mediante-la-serie-de-leibniz)
9. [Comentarios Grupales](#comentarios-grupales)
10. [Referencias Bibliográficas](#referencias-bibliográficas)

---

## ¿Qué es Jupyter Notebook?

Jupyter Notebook es un entorno de trabajo interactivo web que permite desarrollar código en Python de manera dinámica, a la vez que integrar en un mismo documento tanto bloques de código como texto, gráficas o imágenes. Te permite editar y ejecutar documentos de notebook a través de cualquier navegador web, e incluso dentro de Pycharm.

---

## ¿Qué es Racket? 

Racket es un lenguaje de programación de amplio espectro de la familia de Lisp y Scheme. Uno de sus principales objetivos tras su diseño es posibilitar la creación de nuevos lenguajes o dialectos. El lenguaje es usado en una variedad de entornos tales como scripting, enseñanza en ingeniería informática o la investigación.

La plataforma nos ofrece la herramienta `DrRacket`, un entorno de desarrollo integrado programado en Racket, que nos facilitará la tarea de programar en Racket. También nos ofrece `raco`, un herramienta para la línea de comandos que nos permitirá instalar paquetes o compilar librerías.

### iRacket 

iRacket es una implementación del kernel de Racket para Jupyter, lo que permite la programación interactiva estilo bloc de notas con Racket. Esta biblioteca facilita la creación de documentos interactivos que combinan código ejecutable y visualizaciones en un solo lugar. Con iRacket, los usuarios pueden aprovechar las capacidades de Jupyter para explorar y experimentar con código Racket de manera fluida y colaborativa.

---

## Instalar Python

Para instalar Jupyter Notebook es necesario que su computadora tenga instalado Python, y este se encuentre agregado al _PATH_ de Windows.

### Descargar Python de la página oficial

1. Visitar [https://www.python.org/](https://www.python.org/).
2. Ir a la pestaña de descargas y seleccionar la versión deseada.
3. Ejecutar el archivo `.exe` descargado, asegurándose de seleccionar la opción "Add Python.exe to PATH" durante la instalación.

### Verifique que Python esté agregado en PATH

Para verificar, puede usar la consola (cmd en Windows, Terminal en Mac) e ingresar el comando `python`. Si Python está correctamente instalado y en PATH, se abrirá el intérprete de Python. De lo contrario, es probable que le aparezca el mensaje:

```
'python' is not recognized as an internal or external command, operable program or batch file.
```
Si su caso es el segundo, visite esta página: [Agregar Python al PATH](https://www.scielo.org.mx/avaliacao/manual_marcacion/instalacion_markup_paths.html)

### Verifique que pip se haya instalado correctamente

`pip` es necesario para la instalación de Jupyter. Para verificar su instalación, use el comando `python -m pip --version` en la consola.

---

## Instalar Racket y iRacket

Para poder utilizar la biblioteca de iRacket en conjunto con Jupyter Notebook, es necesario tener instalado Racket.

### Descargar Racket de la página oficial

1. Visitar la página de descargas de Racket: [https://download.racket-lang.org/](https://download.racket-lang.org/)
2. Seleccionar la versión deseada para el sistema operativo de su conveniencia.
3. Ejecutar el archivo `.exe` descargado y seguir los pasos del instalador.

### Verifique que Racket esté agregado en PATH

Para verificar, puede usar la consola (cmd en Windows, Terminal en Mac) e ingresar el comando `raco`. Si Racket está correctamente instalado y en el PATH, le aparecerá el siguiente mensaje:

```
Usage: raco <command> <option> ... <arg> ...

Frequently used commands:
  docs                 search and view documentation
  make                 compile source to bytecode
  setup                install and build libraries and documentation
  pkg                  manage packages
  exe                  create executable
  test                 run tests associated with files/directories

A command can be specified by an unambiguous prefix.
See `raco help' for a complete list of commands.
See `raco help <command>' for help on a command.
```
De lo contrario, es probable que le aparezca el mensaje:
```
'raco' is not recognized as an internal or external command,
operable program or batch file.
```
Si su caso es el segundo, visite esta página: [Agregar Racket al PATH](https://docs.racket-lang.org/pollen/Installation.html#(part._.How_to_install))

### Instalando y registrando la biblioteca iRacket

Para instalar la biblioteca de iRacket, solo basta con ingresar el siguiente comando en la terminal:

```
raco pkg install iracket
```
Después de instalar la biblioteca, debe registrar el kernel iRacket con Jupyter. El registro del kernel se puede hacer a través del siguiente comando en la terminal:

```
raco iracket install
```

---

## Instalar Jupyter

Ahora que tenemos instalado Python correctamente, será mucho más sencillo instalar Jupyter. Para ello, abra una nueva consola. A continuación, ingrese el comando:

```
pip install notebook
```
Automáticamente, Python descargará e instalará las librerías necesarias para utilizar Jupyter.

---

## Ejecución de Jupyter Notebook

Al ser Jupyter Notebook un entorno de desarrollo basado en web requiere de un servidor web que atienda las peticiones. El servidor se levanta cuando ejecuta el Jupyter Notebook, se abre una consola de servicios y el Notebook Dashboard. Para ejecutar el Notebook, abra la consola e ingrese:

```
jupyter notebook
```
Se iniciará el servidor y se abrirá el Notebook Dashboard en la pestaña `Files`.

---

## Crea un Notebook

Para crear un notebook con el kernel de iRacket, en la pestaña de `Files` del Notebook Dashboard, de click en `New` y luego en `Racket`. Se generará una libreta en modo de edición, ahora solo pruebe escribir algo de código. La opción de `Racket` está disponible ya que anteriormente registramos el kernel de iRacket con Jupyter. Si la opción de crear un notebook con el kernel de Racket no está disponible, regrese al apartado: [Instalando y registrando la biblioteca iRacket](#instalando-y-registrando-la-biblioteca-iracket).

---

## Abra el Notebook del proyecto

Ahora, importaremos el Notebook del proyecto para ejecutarlo en Jupyter. Primero, regrese a la pestaña de `Files` de Jupyter. A continuación, de click en `Upload` y se abrirá su explorador de archivos. Seleccione el archivo del proyecto y de click en `Abrir`.

Finalmente haga click en `Upload`. Ahora, podrá ver el archivo entre los demás. Haga click para abrirlo. Ahora, en la siguiente sección se describirá cada ejercicio del proyecto, así como algunos casos prueba.

---

## Descripción y ejecución

La recursividad es una técnica en programación que permite que una función se llame a sí misma para resolver un problema. Esta técnica se utiliza comúnmente en algoritmos que involucran la repetición de una acción o la exploración de una estructura de datos.

En este proyecto, nos enfocaremos en crear programas en Racket que utilicen la recursividad para resolver problemas específicos. A través de la implementación de algoritmos recursivos, podremos explorar los beneficios y limitaciones de esta técnica en diferentes escenarios.

### Número Combinatorio

> **Datos de entrada**: `n`,es el número total de elementos, y `k` el número de elementos a seleccinar.  
**Datos de salida**: El número de combinaciones totales de `n` en `k`.

Este código es una implementación de la fórmula matemática para calcular el número combinatorio de $n$ en $k$, también conocido como coeficiente binomial.

Para elegir $k$ elementos de un conjunto de $n$ elementos, podemos tomar un elemento específico como parte de esos $k$ elementos o no. Si tomamos un elemento específico como parte de los $k$ elementos, entonces debemos elegir $k-1$ elementos de los $n-1$ elementos restantes. Si no tomamos ese elemento específico como parte de los $k$ elementos, entonces debemos elegir $k$ elementos de los $n-1$ elementos restantes.

Al sumar estas dos opciones, obtenemos el número total de formas de elegir $k$ elementos de un conjunto de $n$ elementos. Y debido a que la fórmula se define recursivamente, podemos utilizarla para calcular el número combinatorio de cualquier par de valores $n$ y $k$. 

Recursivamente, esto es: $C_{n, k}=C_{n-1,~k-1}+C_{n-1,~k}$

La función definida al inicio, `combinaciones`, utiliza recursión para calcular el número combinatorio. Si $k=0 \vee k=n$, entonces retorna $1$, porque la fórmula combinatoria de un conjunto vacío o del conjunto completo siempre es $1$. De lo contrario, utiliza la fórmula recursiva mencionada anteriormente.

El programa luego solicita al usuario que ingrese los valores de `n` y `k`, y los valida para asegurarse de que no sean números negativos. Si $k$ es mayor que $n$, significa que el número combinatorio no está definido y se imprime un mensaje que indica esto. Si $k$ es menor o igual que $n$, el programa utiliza la función `combinaciones` para calcular el número combinatorio y lo imprime en pantalla.

#### Código y casos de prueba

``` racket
(define (C n k)
  (if (or (< n 0) (< k 0)) 
      (displayln "Solo números positivos") 
      (if (= k 0)
          1
          (if (= n k)
              1
              (if (> k n)
                 (displayln "Está combinación no está definida, n debe ser mayor a k")
                  (+ (C (- n 1) (- k 1))  (C (- n 1 ) k)) 
              )
          )
      )
  )
)

(display "Evaluación del número combinatorio C(n,k): ") (newline)
(display "Introduzca n: ")
(let ((n (read)))
  (display "Introduzca k: ")
  (let ((k (read)))
    (display "C(n, k) = ")
    (display (C n k))))
```





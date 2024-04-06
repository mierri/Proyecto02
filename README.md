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

`pip` es necesario para la instalación de Jupyter. Para verificar su instalación, use el siguiente comando en la consola:
```
python -m pip --version
```

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

La función definida al inicio, `C`, utiliza recursión para calcular el número combinatorio. Si $k=0 \vee k=n$, entonces retorna $1$, porque la fórmula combinatoria de un conjunto vacío o del conjunto completo siempre es $1$. De lo contrario, utiliza la fórmula recursiva mencionada anteriormente.

El programa luego solicita al usuario que ingrese los valores de `n` y `k`, y los valida para asegurarse de que no sean números negativos. Si $k$ es mayor que $n$, significa que el número combinatorio no está definido y se imprime un mensaje que indica esto. Si $k$ es menor o igual que $n$, el programa utiliza la función `C` para calcular el número combinatorio y lo imprime en pantalla.

#### Código y casos de prueba

``` racket
(define (mcd a b)
  ; Comprueba si 'a' o 'b' son negativos al inicio de cada llamada recursiva.
  (if (< a 0) (mcd (* a -1) b)
      (if (< b 0) (mcd a (* b -1))
          (if (= a 0)
              b
              (if (= b 0)
                  a
                  (if (< a b)
                      (mcd a (- b a)) ; Aplica la propiedad MCD(a, b) = MCD(a, b-a).
                      (mcd (- a b) b) ; Aplica la propiedad MCD(a, b) = MCD(a-b, b).
                  )
              )
          )
      )
  )
)

(display "Evaluación del máximo común divisor MCD(a, b) \n")
(display "Introduzca el valor de a (debe ser negativo): ")
(let loop ((a (read)))
  (if (< a 0)
      (begin
        (display "Introduzca el valor de b (debe ser negativo): ")
        (let loop ((b (read)))
          (if (< b 0)
              (begin
                (display "El Máximo Común Divisor (MCD) de ")(display a) (display " y ") (display b)(display " es: ")(display (mcd a b))
                (newline))
              (begin
                (display "El valor de 'b' debe ser negativo.\n")
                (loop (read)))))
        )
      (begin
        (display "El valor de 'a' debe ser negativo.\n")
        (loop (read)))))
```

```
Evaluación del número combinatorio C(n,k): 
Introduzca n: 
 5
Introduzca k: 
 3
C(n, k) = 10

Evaluación del número combinatorio C(n,k): 
Introduzca n: 
 2
Introduzca k: 
 3
C(n, k) = Está combinación no está definida, n debe ser mayor a k
#<void>

Evaluación del número combinatorio C(n,k): 
Introduzca n: 
 5
Introduzca k: 
 5
C(n, k) = 1

Evaluación del número combinatorio C(n,k): 
Introduzca n: 
 -9
Introduzca k: 
 -7
C(n, k) = Solo números positivos
#<void>
```

---

### Máximo Común Divisor de Números Negativos

> **Datos de entrada**: `a` y `b`, dos números enteros donde `a < b`. Para los propósitos de este ejercicio, se permiten números únicamente negativos.  
**Datos de salida**: Máximo Común Divisor (MCD) entre `a` y `b`.

Este ejercicio introduce una función llamada `mcd`, destinada a calcular el MCD de dos números enteros negativos `a` y `b` utilizando una adaptación del algoritmo de Euclides. La función asegura que ambos números sean negativos antes de proceder con el algoritmo.

El algoritmo modificado se basa en la propiedad matemática de que el MCD de dos números no cambia si el mayor número se reduce por el menor. En otras palabras, $MCD(a, b) = MCD(a, b-a)$ para $a < b$, lo cual es una variación del algoritmo tradicional de Euclides que normalmente utiliza el resto de la división de `a` por `b` en lugar de la diferencia.

La función `mcd` opera bajo las siguientes reglas:
- Si `a` es negativo, se convierte a `a` en positivo llamando recursivamente a `mcd` con `-a` y `b`.
- Si `b` es negativo, se convierte a `b` en positivo llamando recursivamente a `mcd` con `a` y `-b`.
- Si `a` es menor que `b`, aplica la propiedad $MCD(a, b) = MCD(a, b-a)$.
- De lo contrario, aplica la propiedad $MCD(a, b) = MCD(a-b, b)$.

#### Código y casos de prueba

```racket
(define (mcd a b)
  ; Comprueba si 'a' o 'b' son negativos al inicio de cada llamada recursiva.
  (if (< a 0) (mcd (* a -1) b)
      (if (< b 0) (mcd a (* b -1))
          (if (= a 0)
              b
              (if (= b 0)
                  a
                  (if (< a b)
                      (mcd a (- b a)) ; Aplica la propiedad MCD(a, b) = MCD(a, b-a).
                      (mcd (- a b) b) ; Aplica la propiedad MCD(a, b) = MCD(a-b, b).
                  )
              )
          )
      )
  )
)

(display "Evaluación del máximo común divisor MCD(a, b) \n")
(display "Introduzca el valor de a (debe ser negativo): ")
(let loop ((a (read)))
  (if (< a 0)
      (begin
        (display "Introduzca el valor de b (debe ser negativo): ")
        (let loop ((b (read)))
          (if (< b 0)
              (begin
                (display "El Máximo Común Divisor (MCD) de ")(display a) (display " y ") (display b)(display " es: ")(display (mcd a b))
                (newline))
              (begin
                (display "El valor de 'b' debe ser negativo.\n")
                (loop (read)))))
        )
      (begin
        (display "El valor de 'a' debe ser negativo.\n")
        (loop (read)))))
```

```
Evaluación del máximo común divisor MCD(a, b) 
Introduzca el valor de a (debe ser negativo): 
 -8
Introduzca el valor de b (debe ser negativo): 
 -16
El Máximo Común Divisor (MCD) de -8 y -16 es: 8

Evaluación del máximo común divisor MCD(a, b) 
Introduzca el valor de a (debe ser negativo): 
 8
El valor de 'a' debe ser negativo.
 -16
Introduzca el valor de b (debe ser negativo): 
 9
El valor de 'b' debe ser negativo.
 -12
El Máximo Común Divisor (MCD) de -16 y -12 es: 4
```

---

### Generación de Lista de Números Primos 

> **Datos de entrada**: `a` y `b`, dos números enteros donde `a < b`. Este ejercicio no se restringe a números negativos o positivos, permitiendo cualquier rango entero donde `a` es menor que `b`.  
**Datos de salida**: Una lista de todos los números primos entre `a` y `b` (no inclusivo).

Este ejercicio introduce una función denominada `primos`, diseñada para generar y devolver una lista de todos los números primos entre dos números enteros `a` y `b`. La función explora de manera incremental cada número en el rango especificado y determina si cada uno es primo.

La detección de números primos se basa en la prueba de divisibilidad: un número es primo si solo es divisible entre sí mismo y la unidad. La implementación específica realiza una iteración comenzando desde el número inmediatamente superior a `a` y continúa hasta `b`, revisando cada número para determinar si es primo mediante un proceso de prueba de divisores.

La función `primos` opera bajo las siguientes premisas:
- Inicia la iteración con el primer número después de `a` para asegurar que el rango sea `(a, b)` y no `[a, b]`.
- Utiliza una función interna `iteracion` que se llama a sí misma recursivamente, avanzando a través de cada número en el rango hasta que supera `b`, punto en el cual retorna una lista vacía indicando el fin de la iteración.
- Dentro de `iteracion`, se utiliza un bucle interno `loop` para probar divisores, comenzando con 2 (el primer número primo) hasta `n` (el número actual siendo probado en el rango).
  - Si se encuentra que `n` es divisible por cualquier número que no sea él mismo (indicado por `n mod i = 0`), `n` no es primo y la iteración continúa con el siguiente número.
  - Si `i` alcanza `n` sin encontrar divisores, entonces `n` es primo y se agrega a la lista de resultados mediante `cons`.
  - El bucle `loop` incrementa `i` y se repite hasta que se determina si `n` es primo o no.

#### Código y casos de prueba

```racket
(define (primos a b)
  (define (iteracion n)
    (if (> n b) ; Si n > b entonces terminamos de iterar y regresamos una lista vacía
        '()
        (let loop ((i 2)) ; Comienza el loop donde se prueban valores desde 2 hasta el valor de n para ver 
          (cond
            ((= i n) (cons n (iteracion (+ n 1)))) ; Si i = n entonces es primo por lo que juntamos la lista con la siguiente lista que se generará al usar iterar
            ((= 0 (modulo n i)) (iteracion (+ n 1))) ; Si n mod i = 0 entonces no es primo ya que tuvo un divisor, continuamos con la siguiente iteracion
            (else (loop (+ i 1))))))) ; Si no pasa ninguna de las anteroires entonces incrementamos i y volvemos a ejecutar el loop
  (iteracion (+ a 1))) ; Volvemos a ejcutar iteracion para verificar otro valor de la lista

(display "Genera una lista de números primos dentro de un rango.")(newline)
(let loop ((a 0) (b 0))
  (display "Introduce el valor de a: ")
  (set! a (read))
  (display "Introduce el valor de b: ")
  (set! b (read))
  (if (< a b)
      (begin
        (display "Los números primos entre ")
        (display a)
        (display " y ")
        (display b)
        (display " son: ")
        (display (primos a b))
        (newline))
      (begin
        (display "Los valores deben ser a < b. Inténtelo de nuevo.\n")
        (loop a b))))
```

```
Genera una lista de números primos dentro de un rango.
Introduce el valor de a: 
 3
Introduce el valor de b: 
 20
Los números primos entre 3 y 20 son: (5 7 11 13 17 19)

Genera una lista de números primos dentro de un rango.
Introduce el valor de a: 
 9
Introduce el valor de b: 
 3
Los valores deben ser a < b. Inténtelo de nuevo.
Introduce el valor de a: 
 7
Introduce el valor de b: 
 33
Los números primos entre 7 y 33 son: (11 13 17 19 23 29 31)
```

---

### Búsqueda en Lista

> **Datos de entrada**: `n`, el elemento a buscar, y `lista`, una lista de elementos.  
**Datos de salida**: Un booleano que indica si el elemento `n` se encuentra o no en `lista`.

Este ejercicio presenta una función denominada `busca`, diseñada para verificar la presencia de un elemento `n` dentro de una lista dada `lista`. Utiliza un enfoque recursivo para iterar a través de la lista, comparando cada elemento con `n`.

El procedimiento de la función `busca` es sencillo pero efectivo, implementando la técnica de búsqueda lineal, la cual recorre cada elemento de la lista secuencialmente hasta encontrar el elemento objetivo o hasta que la lista se agote. La función opera bajo las siguientes reglas:

- Si la lista está vacía (`null? lista`), la función retorna `#f`, indicando que el elemento `n` no se encontró en la lista.
- Si el primer elemento de la lista (`car lista`) es igual a `n`, entonces retorna `#t`, señalando que el elemento ha sido encontrado.
- Si el primer elemento no es `n`, la función se llama a sí misma recursivamente con el resto de la lista (`cdr lista`), omitiendo el primer elemento ya comparado.

La búsqueda termina tan pronto como se encuentra una coincidencia, retornando `#t`, o cuando se ha recorrido toda la lista sin encontrar el elemento, retornando `#f`. Este enfoque asegura que cada elemento de la lista será examinado exactamente una vez, ofreciendo una manera eficiente y directa de determinar la presencia de un valor específico dentro de una estructura de datos lineal.

#### Código y casos de prueba

```racket
(define (busca n lista)
    (cond
        ((null? lista) #f) ; Si la lista está vacía entonces falso
        ((equal? n (car lista)) #t) ; Si el primer elemento = n entonces true
        (else (busca n (cdr lista))) ; Si no, ejecutamos de nuevo la función pero sin el primer elemento
    )
)

(display "Determina si un elemento se encuentra en una lista.")(newline)
(display "Introduzca el elemento a buscar: ")
(let ((n (read)))
  (display "Introduza la lista (ejemplo: (1 2 3 4)): ")
  (let ((lista (read)))
    (display "Resultado: ")
    (display (busca n lista))))
```

```
Determina si un elemento se encuentra en una lista.
Introduzca el elemento a buscar: 
 8
Introduza la lista (ejemplo: (1 2 3 4)): 
 (3 7 5 2 1 4 6 8 4 2 4)
Resultado: #t

Determina si un elemento se encuentra en una lista.
Introduzca el elemento a buscar: 
 1
Introduza la lista (ejemplo: (1 2 3 4)): 
 (3 7 5 2 4 6 8 4 2 4)
Resultado: #f
```

---

### Inversión de Lista

> **Datos de entrada**: `lista`, una lista de elementos que se desea invertir.  
**Datos de salida**: La `lista` ingresada pero con sus elementos en orden inverso.

Este ejercicio introduce una función llamada `invierte`, la cual está diseñada para invertir el orden de los elementos dentro de una lista dada. La función aplica un método recursivo para descomponer y reconstruir la lista en el orden opuesto, demostrando una aplicación práctica y elegante de la recursividad en la manipulación de estructuras de datos lineales.

El funcionamiento de `invierte` se basa en los siguientes principios operativos:

- Cuando la función recibe una lista vacía (`null? lista`), retorna una lista vacía (`'()`). Este caso base es crucial para la recursividad, proporcionando un punto de terminación claro.
- Si la lista no está vacía, la función procede a llamarse a sí misma recursivamente con el resto de la lista (`cdr lista`), excluyendo el primer elemento (`car lista`). Esta llamada recursiva continúa descomponiendo la lista hasta que se alcanza el caso base.
- En cada etapa de la recursión, el primer elemento de la lista en el momento de esa llamada se agrega al final de la lista reconstruida mediante `append`. Esto se logra concatenando el resultado de la llamada recursiva, que eventualmente construye la parte invertida de la lista, con el elemento actual envuelto en `list` para asegurar que se trate como una lista durante la concatenación.

#### Código y casos de prueba

```racket
(define (invierte lista)
    (if (null? lista)
        '()                            ; Si es null entonces devuelve una lista vacia
        (append (invierte (cdr lista)) ; Si no, ejecutamos de nuevo el invierte pero sin el primer elemento
        (list (car lista)))            ; concatenamos el valor al final de la lista
    )
)

(display "Invierte el orden de una lista.")(newline)
(display "Introduce una lista para invertirla (ejemplo: (1 2 3)): ")
(let ((lista (read)))
  (display "La lista invertida es: ")
  (display (invierte lista)))
```

```
Invierte el orden de una lista.
Introduce una lista para invertirla (ejemplo: (1 2 3)): 
 (6 9 8 3 5 0 0)
La lista invertida es: (0 0 5 3 8 9 6)
```

---

### Eliminación de Elemento de una Lista

> **Datos de entrada**: `n`, el elemento a eliminar, y `lista`, una lista de elementos donde se buscará y eliminará `n`.  
**Datos de salida**: Una nueva lista que resulta de eliminar todas las instancias de `n` en `lista`.

Este ejercicio introduce una función llamada `elimina`, que se propone eliminar todas las instancias de un elemento `n` específico de una lista dada `lista`. Se emplea un método recursivo para atravesar la lista, eliminando cualquier ocurrencia de `n`.

El mecanismo de `elimina` se basa en la técnica de filtrado recursivo, donde la función se despliega a lo largo de la lista elemento por elemento, reconstruyendo una nueva lista sobre la marcha, pero omitiendo las instancias de `n`. La operación de la función sigue estas reglas esenciales:

- Si la lista está vacía (`null? lista`), retorna una lista vacía, ya que no hay elementos para eliminar ni conservar.
- Si el primer elemento de la lista (`car lista`) coincide con `n`, ese elemento se omite, y la función continúa su proceso con el resto de la lista (`cdr lista`), no incluyendo el elemento actual en la nueva lista construida.
- En caso contrario, si el primer elemento no es `n`, este se añade a la nueva lista que está siendo construida, y la función procede recursivamente con el resto de la lista.

#### Código y casos de prueba

```racket
(define (elimina n lista)
    (cond
        ((null? lista) '()) ; Si la lista es vacía, regresa una lista vacía.
        ((equal? n (car lista)) (elimina n (cdr lista))) ; Si el elemento está presente, no hace nada con y continua eliminando
        (else (cons (car lista) (elimina n (cdr lista)))) ; Si no se encuentra lo añade a la nueva lista
    )
)

(display "Elimina un elemento de una lista.")(newline)
(display "Introduzca el elemento a eliminar de la lista: ")
(let ((n (read)))
  (display "Introduzca la lista (ejemplo: (1 2 3)): ")
  (let ((lista (read)))
    (display "La lista después de eliminar todas las ocurrencias de ")
    (display n)
    (display " es: ")
    (display (elimina n lista)))
  )
```

```
Elimina un elemento de una lista.
Introduzca el elemento a eliminar de la lista: 
 8
Introduzca la lista (ejemplo: (1 2 3)): 
 (6 9 8 3 5 8 0)
La lista después de eliminar todas las ocurrencias de 8 es: (6 9 3 5 0)
```

---

### Detección de Palíndromos

> **Datos de entrada**: `x`, un número entero positivo del cual se verificará si es un palíndromo.  
**Datos de salida**: Un valor booleano, `#t` si `x` es un palíndromo, y `#f` si no lo es.

El código proporcionado define una función `palindromo` que determina si un número entero positivo dado es un palíndromo. Un palíndromo es un número que se lee igual hacia adelante que hacia atrás, como 12321 o 1331. Para lograr esta verificación, la función sigue un enfoque de dos pasos:

- Primero, el número `x` se convierte en una lista de sus dígitos individuales mediante `numToList`. Después, esta lista se invierte utilizando la función `invierte`, que no se define dentro del ejemplo proporcionado pero se asume realiza la inversión de los elementos de la lista.
   
- A continuación, la función compara la lista invertida con la lista original de dígitos. Si ambas listas son iguales, significa que el número `x` es un palíndromo, y la función devuelve `#t`. De lo contrario, devuelve `#f`.

El algoritmo aprovecha la representación de los números en forma de listas para facilitar la comparación directa entre la secuencia original de dígitos y su versión invertida, evitando así el uso de la función `reverse` de Racket y manteniendo el proceso dentro del marco de la recursividad y el manejo manual de listas.

#### Código y casos de prueba

```racket
(define (invierte lista)
    (if (null? lista)
        '()
        (append (invierte (cdr lista))
        (list (car lista)))
    )
)

(define (numToList x)
    (if (= x 0)
        '()
        (append (numToList (quotient x 10))(list (remainder x 10))
        )
    )
)

(define (palindromo x)
  (let ([m (numToList x)]) ; Convierte el número en una lista
    (let ([i (invierte m)]); Invierte la lista
      (if (equal? i m) ; Compara la lista invertida con la original
          #t
          #f)
        )
    )
)

(display "Determina si un número entero positivo es un palíndromo.")(newline)
(display "Introduzca un número positivo: ")
(let loop ((x (read)))
  (if (<= x 0)
      (begin
        (display "Introduzca un número positivo: ")
        (loop (read)))
      (begin
        (display "Resultado: ")
        (display (palindromo x))
        )
      )
  )
```

```
Determina si un número entero positivo es un palíndromo.
Introduzca un número positivo: 
 1234532
Resultado: #f

Determina si un número entero positivo es un palíndromo.
Introduzca un número positivo: 
 123454321
Resultado: #t
```

---

### Suma de Dígitos

> **Datos de entrada**: `x`, un número entero del cual calcularemos la suma de sus dígitos.  
**Datos de salida**: La suma de los dígitos de `x`.

La función presentada se denomina `SumaDigitos` y recibe como argumento el número entero `x`. Esta función se encarga de calcular la suma de todos los dígitos que componen a `x`, haciendo uso de una estrategia recursiva sin depender de funciones incorporadas específicas de Racket para el manejo de números o cadenas.

El algoritmo opera bajo un simple principio de recursividad, donde:
- Si `x` es menor que 10 (es decir, es un único dígito), la función simplemente devuelve `x`, puesto que la "suma de sus dígitos" es el mismo número.
- Para números mayores o iguales a 10, la función se descompone en la suma del dígito menos significativo (`modulo x 10`) y la suma de los dígitos del cociente de `x` dividido entre 10 (`quotient x 10`). Esta operación se repite recursivamente hasta que se descompone completamente el número.

La expresión `(+ (modulo x 10) (SumaDigitos (quotient x 10)))` representa el núcleo de esta lógica recursiva, donde `(modulo x 10)` obtiene el último dígito de `x` y `(quotient x 10)` reduce `x` al excluir el último dígito, permitiendo así la suma iterativa de cada dígito individual hasta que solo queda un dígito.

#### Código y casos de prueba

```racket
(define (SumaDigitos x)
    (cond
        ((< x 10) x) 
        (else (+ (modulo x 10) (SumaDigitos (quotient x 10))))
    )
)

(display "Suma los dígitos de un número entero.")(newline)
(display "Introduzca un número entero: ")
(let loop ((a (read)))
  (if (integer? a)
      (let ((x (abs a)))
        (display "La suma de los dígitos de ")
        (display x)
        (display " es: ")
        (display (SumaDigitos x))
        (newline))
      (begin
        (display "Por favor, introduzca un número entero válido: ")
        (loop (read))))
)
```

```
Suma los dígitos de un número entero.
Introduzca un número entero: 
 2345
La suma de los dígitos de 2345 es: 14

Suma los dígitos de un número entero.
Introduzca un número entero: 
 3.5643
Por favor, introduzca un número entero válido: 
 123
La suma de los dígitos de 123 es: 6
```

---

### Conversión de Decimal a Binario

> **Datos de entrada**: Un número entero decimal `n`, el cual será convertido a su equivalente binario.  
**Datos de salida**: Una lista que representa el número binario equivalente de `n`.

La función descrita, `Binario`, es una implementación recursiva para convertir un número entero decimal a su representación en binario sin utilizar funciones incorporadas específicas para este propósito en Racket. La función devuelve una lista de dígitos binarios, donde cada elemento de la lista representa un bit en la secuencia binaria del número decimal proporcionado.

El proceso de conversión se basa en el algoritmo clásico que divide sucesivamente el número decimal por 2 y toma el resto como un dígito binario, proceso que se repite hasta que el cociente es 0. La construcción binaria se realiza de abajo hacia arriba, iniciando desde el bit menos significativo hasta el más significativo.

La función opera bajo la siguiente lógica:
1. **Caso base**: Si `n` es 0 o 1, la función retorna una lista conteniendo el propio `n`. Esto se debe a que 0 y 1 son sus propias representaciones en binario.
2. **Caso recursivo**: Para cualquier otro valor de `n`, la función:
   - Calcula el cociente de `n` dividido por 2 y pasa este valor a una llamada recursiva de sí misma. Este paso descompone el número hacia su base, dividiéndolo sucesivamente por 2 hasta alcanzar el caso base.
   - Calcula el resto de `n` dividido por 2 (`n % 2`), que determina el bit actual en la posición binaria correspondiente.
   - Usa `append` para concatenar el resultado de la llamada recursiva (que construye la porción binaria de los dígitos más significativos) con el resto actual (bit menos significativo). Esto ensambla la secuencia binaria en el orden correcto, desde el bit más significativo hasta el menos significativo.
  
#### Código y casos de prueba

```racket
(define (Binario n)
  (cond
    ((or (= n 0) (= n 1)) (list n)) ; Si n=0 o n=1, regresa n
    (else
     (append (Binario (quotient n 2)) ; Llamamos a Binario pero con la mitad de n
             (list (remainder n 2)))))) ; Agregamos el residuo al final de la lista

(display "Convierte un número decimal a binario.")(newline)
(display "Introduzca un número entero positivo: ")
(let loop ((n (read)))
  (if (and (integer? n) (> n 0))
      (begin
        (display "La representación binaria de ")
        (display n)
        (display " es: ")
        (display (Binario n))
        (newline))
      (begin
        (display "Introduzca un número entero positivo válido: ")
        (loop (read)))))
```

```
Convierte un número decimal a binario.
Introduzca un número entero positivo: 
 1234
La representación binaria de 1234 es: (1 0 0 1 1 0 1 0 0 1 0)

Convierte un número decimal a binario.
Introduzca un número entero positivo: 
 -345
Introduzca un número entero positivo válido: 
 5.13
Introduzca un número entero positivo válido: 
 450
La representación binaria de 450 es: (1 1 1 0 0 0 0 1 0)
```

---

### Cálculo de PI mediante la Serie de Leibniz

> **Datos de entrada**: `n`, el número máximo de iteraciones para aproximar el valor de PI.  
> **Datos de salida**: `pi`, la aproximación del valor de PI tras `n` iteraciones.

La serie de Leibniz es una fórmula matemática que permite calcular el valor de PI mediante una serie infinita. Esta serie representa una forma simple, aunque convergente lentamente, de aproximar PI. La implementación proporcionada utiliza una función recursiva denominada `Leibniz` que acepta dos argumentos: `x`, que actúa como un iterador, y `n`, que define el número máximo de iteraciones deseado para la aproximación.

La fórmula de la serie de Leibniz para $\pi$ es la siguiente:  
$$\pi = 4 \times \sum_{k=0}^{\infty} \frac{(-1)^k}{2k+1} = 4 \times (1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \frac{1}{9} - ... )$$

La función `Leibniz` opera de acuerdo con las siguientes reglas:
- Si `n` es 0, entonces la aproximación de PI es 4, ya que no se realiza ninguna iteración de la serie.
- Si el iterador `x` es igual a `n + 1`, se detiene la sucesión, devolviendo 0, ya que se ha alcanzado el número máximo de iteraciones.
- Cuando `x` es 0, se inicia la serie multiplicando por 4 el resultado de la recursividad para obtener el valor aproximado de PI.
- Para `x` mayor a 0, la función determina si `x` es par o impar, sumando o restando, respectivamente, el término $$\frac{1}{2x+1}$$ de la serie. Esto se ajusta al patrón alternante de sumas y restas de la fórmula de Leibniz.

La recursión continúa alternando entre sumar y restar los términos de la serie basados en si el iterador `x` es par o impar. Esta ejecución recursiva se repite hasta que `x` alcanza el valor de `n`, en cuyo punto se habrá calculado el valor aproximado de PI después de `n` iteraciones.

#### Código y casos de prueba

```racket
(define (Leibniz n)
  (define (Leibniz-aux x n) ; Usamos x como iterador y n como el numero maximo de iteraciones que deseamos hacer
    (cond
      ((equal? 0 n)  4) ; Si mi n = 0 entonces Pi = 4
      ((equal? x (+ n 1)) + 0) ; Si mi x = n+1 entonces termina la sucesión
      ((equal? x 0) (* 4 (+ 1 (Leibniz-aux (+ x 1) n)))) ; En caso de x = 0 entonces multiplicamos por 4 las siguientes sumas que se provocarán recursivamente
      ((> x 0) (if (even? x) 
                   (+ (/ 1.0 (+ 1 (* 2 x))) (Leibniz-aux (+ x 1) n)) ; Si es par entonces sumamos la siguiente llamada
                   (+ (/ -1.0 (+ 1 (* 2 x))) (Leibniz-aux (+ x 1) n))) ; Si es impar etnonces restamos la siguiente llamada
      )
    )
  )
  (Leibniz-aux 0 n)
)

(display "Aproxima el valor de PI con la serie de Leibniz.")(newline)
(display "Introduzca un número entero positivo para las iteraciones de la serie de Leibniz: ")
(let loop ((n (read)))
  (if (and (integer? n) (>= n 0))
      (begin
        (display "El valor aproximado de PI después de ")
        (display n)
        (display " iteraciones es: ")
        (display (Leibniz n))
        (newline))
      (begin
        (display "Introduzca un número entero positivo válido: ")
        (loop (read)))))
```

```
Aproxima el valor de PI con la serie de Leibniz.
Introduzca un número entero positivo para las iteraciones de la serie de Leibniz: 
 0
El valor aproximado de PI después de 0 iteraciones es: 4

Aproxima el valor de PI con la serie de Leibniz.
Introduzca un número entero positivo para las iteraciones de la serie de Leibniz: 
 4
El valor aproximado de PI después de 4 iteraciones es: 3.33968253968254

Aproxima el valor de PI con la serie de Leibniz.
Introduzca un número entero positivo para las iteraciones de la serie de Leibniz: 
 100000
El valor aproximado de PI después de 100000 iteraciones es: 3.141602653489794
```

---

## Comentarios Grupales

### Dificultades Encontradas

Este proyecto ha sido tanto un desafío como una oportunidad de aprendizaje, permitiéndonos explorar en profundidad el paradigma de la programación funcional y el manejo del lenguaje Racket dentro de un entorno Jupyter Notebook.

Estamos más familiarizados con los paradigmas de programación imperativos, por lo que adaptarnos al enfoque funcional, donde las funciones y la inmutabilidad son la norma, fue un reto.

Aunque Racket es un lenguaje poderoso y flexible, su sintaxis y enfoque fueron nuevos para nosotros. Familiarizarnos con un lenguaje prefijo, y entender cómo aprovechar sus capacidades para resolver problemas fue un proceso que requirió tiempo y paciencia.

La depuración en Racket, especialmente dentro de DrRacket, presentó sus propias complicaciones. Aprender a interpretar los mensajes de error y a utilizar estrategias efectivas de debugging fue esencial para avanzar en el proyecto.

### Aprendizajes Obtenidos:

Sin embargo, este proyecto nos permitió comprender realmente los principios de la programación funcional, como la pureza de funciones, el uso extensivo de la recursividad, y el manejo de listas y estructuras de datos inmutables de manera eficiente.

 A través de la práctica y la experimentación, adquirimos una sólida comprensión de Racket. Aprendimos a utilizar sus características, lo que nos permitió entender su función para la creación y manipulación de nuevos lenguajes o dialectos.

En conclusión, este proyecto no solo nos permitió aplicar un nuevo paradigma de programación, sino que también enriqueció nuestro entendimiento teórico y práctico de la programación funcional.

---

## Referencias Bibliográficas

1. Installation. (n.d.). Pip Documentation v23.1.2. [https://pip.pypa.io/en/stable/installation/](https://pip.pypa.io/en/stable/installation/)
2. Project Jupyter. (2015). Install and Use. Jupyter. [https://docs.jupyter.org/en/latest/install.html](https://docs.jupyter.org/en/latest/install.html)
3. Project Jupyter. (2015). Running the Notebook. Jupyter. [https://docs.jupyter.org/en/latest/running.html](https://docs.jupyter.org/en/latest/running.html)
4. Python.org. (2023, May 11). Python Setup and Usage. Python Documentation. [https://docs.python.org/3/using/index.html](https://docs.python.org/3/using/index.html)
5. Racket documentation. (s. f.). [https://docs.racket-lang.org/](https://docs.racket-lang.org/)
6. Recursividad (artículo) | Algoritmos (n.d.). Khan Academy. [https://es.khanacademy.org/computing/computer-science/algorithms/recursive-algorithms/a/recursion](https://es.khanacademy.org/computing/computer-science/algorithms/recursive-algorithms/a/recursion)


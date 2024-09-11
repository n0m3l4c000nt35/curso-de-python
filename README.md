# Curso de Python

[Web oficial de Python](https://www.python.org/)

[Guía de estilo - PEP 8](https://peps.python.org/)

## Índice

- [Comentarios](#comentarios)
- [Variables](#variables)
- [Operadores matemáticos](#operadores-matematicos)
- [Operadores lógicos](#operadores-logicos)
- [Funciones incorporadas](#funciones-incorporadas)
- [Estructura de datos](#estructura-de-datos)

## Comentarios

Los comentarios son líneas de código no ejecutadas por el programa.

- Explicar código.
- Prevenir que el código sea ejecutado.

Comentarios de una línea

```python
# Comentario de una línea
```

```python
"""
Comentarios
multilínea
"""
```

## Variables

Objeto con un valor almacenado en memoria que puede cambiar con el tiempo. Se definen con un nombre. Se pone un signo `=` para indicar que se le asigna un valor y se le asigna el valor. No se requiere definir el tipo de dato.

La función `type()` permite conocer el tipo de dato de una variable.

### Tipos de variables

- String o cadena de texto.
- Números enteros.
- Números decimales o flotantes.
- Booleanos.

#### String

Cadena de caracteres, unión de letras y símbolos. Al encerrar el valor entre comillas simples o dobles Python identifica variables de tipo texto.

**Type**: `<class 'str'>`

```python
name = "Juan"
```

#### Entero

Números que no tienen parte decimal o fracción. Se identifica solo con el número.

**Type**: `<class 'int'>`

```python
age = 30
```

#### Decimal

Números que tienen parte decimal o fraccionaria. Se identifica con el punto como separador decimal.

**Type**: `<class 'float'>`

```python
height = 1.70
```

#### Booleano

**Type**: `<class 'bool'>`

```python
positive = True
negative = False
```

## Operadores matematicos

### Suma

```python
2 + 2 # 4
```

### Resta

```python
2 - 2 # 0
```

### Multiplicación

```python
2 * 2 # 4
```

### División

```python
2 / 2 # 1.0
```

El resultado de las divisiones siempre es un número decimal.

### Módulo

```python
2 % 2 # 0
```

### Potencia

```python
2 ** 2 # 4
```

El primer número es la base y el segundo número es la potencia.

### Concatenar texto

```python
"Hola" + "Mundo" # HolaMundo
```

### Multiplicar texto

```python
"Hola" * 2 # HolaHola
```

## Operadores logicos

Devuelve `True` o `False`

### Mayor

```python
1 > 2 # False
```

### Menor

```python
1 < 2 # True
```

### Mayor o igual

```python
1 >= 2 # False
```

### Menor o igual

```python
1 <= 2 # True
```

### Comparación de igualdad

```python
1 == 2 # False
```

### Comparación de diferencia

```python
1 != 2 # True
```

## Funciones incorporadas

### int

Convierte un valor a un número entero.

```python
int(1.23) # 1
```

### float

Convierte un número entero a un número decimal.

```python
float(3) # 3.0
```

### str

Convierte cualquier valor a una cadena de texto

```python
str(True) # "True"
```

### type

Devuelve el tipo de una variable u objeto.

```python
type(1) # <class 'int'>
```

### help

Devuelve la documentación de una función.

```python
help(int)

"""Help on class int in module builtins:

class int(object)
 |  int([x]) -> integer
 |  int(x, base=10) -> integer
 |
 |  Convert a number or string to an integer, or return 0 if no arguments
 |  are given.  If x is a number, return x.__int__().  For floating-point
 |  numbers, this truncates towards zero.
 |
 |  If x is not a number or if base is given, then x must be a string,
 |  bytes, or bytearray instance representing an integer literal in the
 |  given base.  The literal can be preceded by '+' or '-' and be surrounded
 |  by whitespace.  The base defaults to 10.  Valid bases are 0 and 2-36.
 |  Base 0 means to interpret the base from the string as an integer literal.
 |  >>> int('0b100', base=0)
 |  4
 |
 |  Built-in subclasses:
 |      bool
 |
 |  Methods defined here:
 |
 |  __abs__(self, /)
 |      abs(self)
 |
-- Más  --"""
```

## Estructura de datos

Conjuntos o colecciones de datos que permiten orgenizarlos, manipularlos, extraerlos, buscarlos o insertarlos. Son eficientes. Pueden modificarse después de ser creados (mutables).

- Listas
- Tuplas
- Diccionarios
- Sets

### Listas

Se definen entre corchetes. Permite duplicados. Ordenado, mantiene el orden en el que fue definida. Mutable. Puede contener todo tipo de datos.

```python
lista = [1, True, 2, "Juan", 3.0]
```

Acceder a un elementos a través de su índice

```python
lista[0] # 1
```

Longitud de la lista

```python
len(lista) # 5
```

Último elemento índice negativo

```python
lista[-1] # 3.0
```

Primer elemento índice negativo

```python
lista[-len(lista)] # 1
```

Acceder a una parte de la lista `a:b`, `a` el primer elemento, `b` el elemento siguiente al último que se quiere acceder.

```python
lista[1:3] # [True, 2]
```

Lista anidada

```python
lista_anidada = [lista, False, 4, "Carlos", 1.0] # [[1, True, 2, 'Juan', 3.0], False, 4, 'Carlos', 1.0]
```

Acceder a un elemento de una lista anidada

```python
lista_anidada[0][1] # True
```

Modificar un elemento

```python
lista[3] = "Juan Carlos" # [1, True, 2, 'Juan Carlos', 3.0]
```

Añadir elemento en la última posición

```python
lista.append(False) # [1, True, 2, 'Juan Carlos', 3.0, False]
```

Agregar elementos de un iterable

```python
lista.extend(["Batman", 13, True]) # [1, True, 2, 'Juan Carlos', 3.0, False, 'Batman', 13, True]
```

### Tuplas

Se definen entre paréntesis o elementos separados por coma. Permiten duplicados. Ordenadas. No son mutables. Se utilizan cuando sus valores no se deben modificar o si se requiere menor tiempo de procesamiento.

```python
nums = (1, 2, 3)
nums = 1, 2, 3
```

### Diccionarios

Se definen entre llaves. Cada elementos es una combinación de una clave y un valor. No es ordenado. Mutable. No permite duplicados. Las claves son únicas. Las claves y valores pueden ser de cualquier tipo de dato.

```python
person = {"name": "Juan", "age": 30}
```

Acceder al valor de una clave

```python
person["name"] # Juan
```

Agregar clave y valor

```python
person["height"] = 1.7
```

Acceder a todas las claves y valores

```python
person.items() # dict_items([('name', 'Juan'), ('age', 30), ('height', 1.7)])
```

Acceder a las claves

```python
person.keys() # dict_keys(['name', 'age', 'height'])
```

Acceder a los valores

```python
person.values() # dict_values(['Juan', 30, 1.7])
```

### Sets

Se definen entre llaves. No permite duplicados. No es ordenado. Mutable.

```python
set_test = {1, 2, 3, 3} # {1, 2, 3}
```

Agregar un elemento

```python
set_test.add(4)
```

Agregar varios elementos

```python
set_test.update(["uno", "dos", "tres"])
```

Obtener la cantidad de elementos

```python
len(set_test) # 7
```

Eliminar un elemento

```python
set_test.discard("dos")
```

```python
set_test.remove("uno")
```

> [!WARNING]
> Arroja un error si el elemento no existe.

Vaciar el set

```python
set_test.clear()
```

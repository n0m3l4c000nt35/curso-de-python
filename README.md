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

Se definen entre corchetes. Permite duplicados. Ordenado. Mutable.

```python
nums = [1, 2, 3]
```

### Tuplas

Se definen entre paréntesis. Permite duplicados. Ordenado. No es mutable.

```python
nums = (1, 2, 3)
```

### Diccionarios

Se definen entre llaves. Cada elementos es una combinación de una clave y un valor. No es ordenado. Mutable. No permite duplicados.

```python
person = {name: "Juan", age: 30}
```

### Sets

Se definen entre llaves. No permite duplicados. No es ordenado. Mutable.

```python
set = {1, 2, 3, 3} # {1, 2, 3}
```

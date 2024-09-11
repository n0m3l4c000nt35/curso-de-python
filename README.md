# Curso de Python

[Web oficial de Python](https://www.python.org/)

## Índice

- [Comentarios](#comentarios)
- [Variables](#variables)

### Comentarios

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

### Variables

Objeto con un valor almacenado en memoria que puede cambiar con el tiempo. Se definen con un nombre. Se pone un signo `=` para indicar que se le asigna un valor y se le asigna el valor. No se requiere definir el tipo de dato.

La función `type()` permite conocer el tipo de dato de una variable.

#### Tipos de variables

- String o cadena de texto.
- Números enteros.
- Números decimales o flotantes.
- Booleanos.

##### String

Cadena de caracteres, unión de letras y símbolos. Al encerrar el valor entre comillas simples o dobles Python identifica variables de tipo texto.

**Type**: `<class 'str'>`

```python
name = "Juan"
```

##### Entero

Números que no tienen parte decimal o fracción. Se identifica solo con el número.

**Type**: `<class 'int'>`

```python
age = 30
```

##### Decimal

Números que tienen parte decimal o fraccionaria. Se identifica con el punto como separador decimal.

**Type**: `<class 'float'>`

```python
height = 1.70
```

##### Booleano

**Type**: `<class 'bool'>`

```python
positive = True
negative = False
```

# Resumen del Módulo 2: Sintaxis Básica de Python

En este módulo se repasaron conceptos fundamentales de la sintaxis de Python, incluyendo variables, tipos de datos, operadores y estructuras condicionales. A continuación, se presenta un resumen detallado:

---

## Variables
- **Buenas prácticas**: 
  - No comenzar los nombres de las variables con números.
  - Usar nombres descriptivos pero no excesivamente largos.
  - El código debe ser autodocumentado, es decir, los nombres de las variables deben reflejar su propósito.

**Ejemplo:**
```python
Bucle_Lapices = []  # Colección de lápices

for lapiz in Bucle_Lapices:  # Iterar sobre cada lápiz
    print(lapiz)
```
De esta forma, el código es más legible y fácil de entender.

---

## Tipos de Datos
- **Principales tipos de datos en Python:**
  - `str` (cadenas de texto)
  - `int` (números enteros)
  - `float` (números decimales)
  - `bool` (valores booleanos: `True` o `False`)
  - Colecciones:
    - Listas (`list`)
    - Diccionarios (`dict` - clave/valor)
    - Tuplas (`tuple` - inmutables)

---

## Operadores
### Operadores de Comparación
| Símbolo | Nombre                  | Expresión   | Descripción               |
|---------|-------------------------|-------------|---------------------------|
| `==`    | Operador de igualdad    | `a == b`    | `a` es igual a `b`        |
| `!=`    | Operador de no igualdad | `a != b`    | `a` no es igual a `b`     |
| `>`     | Operador mayor que      | `a > b`     | `a` es mayor que `b`      |
| `>=`    | Operador mayor o igual  | `a >= b`    | `a` es mayor o igual a `b`|
| `<`     | Operador menor que      | `a < b`     | `a` es menor que `b`      |
| `<=`    | Operador menor o igual  | `a <= b`    | `a` es menor o igual a `b`|

**Nota:** Los operadores `>` y `<` también pueden usarse para comparar cadenas alfabéticamente, basándose en los valores Unicode de las letras.

### Operadores Lógicos
- **`and`**: Ambas condiciones deben cumplirse.
- **`or`**: Al menos una condición debe cumplirse.
- **`not`**: Niega la condición.

---

## Condicionales
- **Estructura básica:**
```python
if condicion:
    # Código si la condición es verdadera
elif otra_condicion:
    # Código si la otra condición es verdadera
else:
    # Código si ninguna condición es verdadera
```
- `elif` se utiliza como un "else if" en Python.

---

## Ejemplo Práctico: Cálculo de Bloques
El problema consiste en calcular cuántos bloques de 4096 bytes se necesitan para almacenar un archivo de tamaño dado.

**Código:**
```python
block_size = 4096
filesize = 6000

full_blocks = filesize // block_size  # Bloques completos
partial_block_remainder = filesize % block_size  # Bytes restantes

if partial_block_remainder > 0:
    total_size = (full_blocks + 1) * block_size
else:
    total_size = full_blocks * block_size

print(total_size)
```

**Ejemplos:**
- `filesize = 1` → 1 bloque → Resultado: 4096 bytes.
- `filesize = 4096` → 1 bloque → Resultado: 4096 bytes.
- `filesize = 6000` → 2 bloques → Resultado: 8192 bytes.

**Regla mental:**
> "Divido para ver bloques completos y uso `%` para ver si sobra algo. Si sobra → sumo 1 bloque."

---

## Términos Clave
- **Funciones integradas**: Funciones predefinidas en Python que se pueden usar directamente.
- **Comentarios**: Notas en el código para explicar su propósito.
- **Conversión explícita**: Conversión manual de un tipo de dato a otro.
- **Conversión implícita**: Conversión automática realizada por Python.
- **Refactorización**: Mejorar el código para hacerlo más claro y legible.
- **Valor de retorno**: Resultado que una función devuelve al ser llamada.

---

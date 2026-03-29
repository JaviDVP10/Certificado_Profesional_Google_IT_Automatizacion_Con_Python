# Cadenas, Listas, Tuplas y Diccionarios

En esta lección, repasaremos los conceptos básicos de cadenas (strings), listas, tuplas y diccionarios en Python. Cada uno de estos tipos de datos es fundamental para trabajar con Python y se utilizan en una variedad de contextos.

## Cadenas (Strings)
Las cadenas son secuencias de caracteres. Puedes crear cadenas utilizando comillas simples o dobles.

### Ejemplo:
```python
# Crear una cadena
greeting = "Hola, mundo!"
print(greeting)  # Salida: Hola, mundo!

# Concatenar cadenas
name = "Juan"
message = "Hola, " + name + "!"
print(message)  # Salida: Hola, Juan!

# Métodos comunes
texto = "python es divertido"
print(texto.upper())  # Salida: PYTHON ES DIVERTIDO
print(texto.replace("divertido", "genial"))  # Salida: python es genial
```

## Listas (Lists)
Las listas son colecciones ordenadas y mutables. Puedes almacenar diferentes tipos de datos en una lista.

### Ejemplo:
```python
# Crear una lista
frutas = ["manzana", "banana", "cereza"]
print(frutas)  # Salida: ['manzana', 'banana', 'cereza']

# Acceder a elementos
print(frutas[0])  # Salida: manzana

# Modificar elementos
frutas[1] = "pera"
print(frutas)  # Salida: ['manzana', 'pera', 'cereza']

# Métodos comunes
frutas.append("naranja")
print(frutas)  # Salida: ['manzana', 'pera', 'cereza', 'naranja']
frutas.remove("pera")
print(frutas)  # Salida: ['manzana', 'cereza', 'naranja']
```

## Tuplas (Tuples)
Las tuplas son colecciones ordenadas e inmutables. Una vez creadas, no puedes modificar sus elementos.

### Ejemplo:
```python
# Crear una tupla
coordenadas = (10, 20)
print(coordenadas)  # Salida: (10, 20)

# Acceder a elementos
print(coordenadas[0])  # Salida: 10

# Desempaquetar tupla
x, y = coordenadas
print(x, y)  # Salida: 10 20
```

## Diccionarios (Dictionaries)
Los diccionarios son colecciones desordenadas de pares clave-valor. Son útiles para almacenar datos relacionados.

### Ejemplo:
```python
# Crear un diccionario
persona = {
    "nombre": "Ana",
    "edad": 25,
    "ciudad": "Madrid"
}
print(persona)  # Salida: {'nombre': 'Ana', 'edad': 25, 'ciudad': 'Madrid'}

# Acceder a valores
print(persona["nombre"])  # Salida: Ana

# Modificar valores
persona["edad"] = 26
print(persona)  # Salida: {'nombre': 'Ana', 'edad': 26, 'ciudad': 'Madrid'}

# Métodos comunes
persona["profesión"] = "Ingeniera"
print(persona)  # Salida: {'nombre': 'Ana', 'edad': 26, 'ciudad': 'Madrid', 'profesión': 'Ingeniera'}
del persona["ciudad"]
print(persona)  # Salida: {'nombre': 'Ana', 'edad': 26, 'profesión': 'Ingeniera'}
```


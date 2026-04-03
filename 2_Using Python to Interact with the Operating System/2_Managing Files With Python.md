# Gestión de Archivos con Python

En este módulo, aprendí cómo trabajar con archivos y directorios utilizando el módulo `os` de Python. Aquí están los conceptos clave y las funciones más importantes:

---

## Rutas en Python
- **Rutas absolutas**: Especifican la ruta completa desde la raíz del sistema hasta el archivo o directorio.
- **Rutas relativas**: Son relativas al archivo que se está ejecutando.

### Buenas prácticas
- Usar `os.getcwd()` para obtener la ruta actual del programa. Esto asegura que el código sea más portátil y funcione correctamente si se mueve a otros sistemas.
- Utilizar `os.path.join()` para construir rutas de manera segura y evitar errores de formato.

---

## La variable `PATH`
La variable global `PATH` en Python indica dónde buscar librerías y directorios. Por defecto, apunta al directorio donde se encuentra el archivo actual, pero se puede modificar para apuntar a otros directorios si es necesario.

---

## Funciones útiles del módulo `os`

### Directorios
- `os.getcwd()`: Devuelve la ruta actual.
- `os.listdir()`: Lista los archivos y directorios en la ruta actual.

### Archivos
- `os.remove()`: Elimina un archivo.
- `os.rename()`: Renombra un archivo.

### Comprobaciones
- `os.path.exists()`: Verifica si un archivo o directorio existe.
- `os.path.getsize()`: Devuelve el tamaño de un archivo.
- `os.path.getmtime()`: Obtiene la fecha de modificación de un archivo (en formato timestamp).
- `os.path.abspath()`: Devuelve la ruta absoluta de un archivo.

---

## Ejemplo práctico
```python
import os

# Obtener la ruta actual
ruta_actual = os.getcwd()
print(f"Ruta actual: {ruta_actual}")

# Listar archivos y directorios
contenido = os.listdir(ruta_actual)
print("Contenido del directorio:", contenido)

# Verificar si un archivo existe
archivo = "ejemplo.txt"
if os.path.exists(archivo):
    print(f"El archivo {archivo} existe.")
else:
    print(f"El archivo {archivo} no existe.")
```
# Resumen del Módulo 3: Bucles en Python

En este módulo se estudiaron los bucles en Python, incluyendo `while`, `for` y conceptos como recursividad. A continuación, se presenta un resumen detallado con ejemplos prácticos:

---

## Bucle `while`
- **Descripción**: Ejecuta un bloque de código mientras una condición sea verdadera.
- **Precaución**: Es importante actualizar el valor de la condición dentro del bucle para evitar bucles infinitos.

**Ejemplo:**
```python
contador = 0
while contador < 5:
    print(f"Contador: {contador}")
    contador += 1  # Actualizamos la condición
```
En este ejemplo, el bucle imprime los valores de `contador` desde 0 hasta 4.

---

## Bucle `for`
- **Descripción**: Se utiliza para iterar sobre una colección (listas, cadenas, etc.) o un rango de números.
- **Función `range()`**:
  - `range(inicio, fin, paso)` genera una secuencia de números.
  - El valor `fin` no está incluido.

**Ejemplo:**
```python
for n in range(0, 51, 5):
    print(n)
```
Este bucle imprime los números desde 0 hasta 50 en pasos de 5.

---

## Recursividad
- **Descripción**: Una función que se llama a sí misma para resolver problemas repetitivos.
- **Precaución**: Asegúrate de incluir una condición de parada para evitar una recursión infinita.

**Ejemplo:**
```python
def cuenta_regresiva(n):
    if n <= 0:
        print("¡Despegue!")
    else:
        print(n)
        cuenta_regresiva(n - 1)  # Llamada recursiva

cuenta_regresiva(5)
```
Este ejemplo realiza una cuenta regresiva desde 5 hasta 0.

---

## Comparación: Bucles anidados vs. Recursividad
- **Bucles anidados**: Se utilizan para recorrer múltiples colecciones.
- **Recursividad**: Se utiliza para problemas que pueden dividirse en subproblemas similares.

**Ejemplo de bucles anidados:**
```python
matriz = [[1, 2], [3, 4], [5, 6]]
for fila in matriz:
    for elemento in fila:
        print(elemento)
```
Este ejemplo recorre e imprime cada elemento de una matriz.

---

## Buenas Prácticas
1. **Evitar bucles infinitos**: Revisa las condiciones y utiliza `break` si es necesario.
2. **Usar nombres descriptivos**: Asegúrate de que las variables dentro de los bucles sean claras.
3. **Optimizar el rendimiento**: Evita bucles innecesarios o anidados si no son requeridos.

---


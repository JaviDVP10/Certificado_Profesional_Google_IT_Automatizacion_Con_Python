### Resumen del módulo: Expresiones Regulares en Python

1. **Librería `re`**: Es la librería de Python para trabajar con expresiones regulares.
   
2. **Funciones principales**:
   - **`re.search(r"expresion_regular", "texto")`**: Busca la primera coincidencia de la expresión regular en el texto.
     - La `r""` delante del texto indica que es una cadena "raw" (sin procesar), lo que evita que caracteres especiales como `\` sean interpretados por Python.
   - **`re.findall(expresion_regular, texto)`**: Encuentra todas las coincidencias de la expresión regular en el texto.
   - **`re.split(r"expresion_regular", "texto")`**: Divide el texto en partes usando la expresión regular como delimitador.

3. **Grupos en expresiones regulares**:
   - Se pueden usar grupos para buscar múltiples subtextos en el mismo texto.
   - Ejemplo: `re.search(r"expresion1", r"expresion2", texto)` devuelve una colección de resultados:
     - `resultado[0]`: Contiene todas las agrupaciones.
     - `resultado[1]`: Contiene lo encontrado por el primer grupo.
     - `resultado[2]`: Contiene lo encontrado por el segundo grupo.

4. **Ejemplo práctico**:
   - Usar `re.split` para dividir un texto como `"hola, que tal?"` con una coma como delimitador, resultando en `["hola", " que tal?"]`.

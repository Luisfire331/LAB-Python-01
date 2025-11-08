# Laboratorio 1 - Python

## 📌 Descripción  
Este laboratorio tiene como objetivo que los estudiantes fortalezcan sus conocimientos relacionados con **Python** y la programación imperativa.

---

## 🛠️ Instrucciones Generales  

1. **Fork del repositorio**  
   - Realice un **fork** de este repositorio en su cuenta personal de GitHub.  
   - No realice cambios directamente sobre el repositorio original.  

2. **Estructura de carpetas**  
   - Dentro de su fork, cree una carpeta llamada **`lab01/`**.  
   - Cada ejercicio debe resolverse en un archivo **independiente** con el siguiente formato:  
     ```
     lab01/ejercicio01.ipynb
     lab01/ejercicio02.ipynb
     ...
     ```  

3. **Resolución de ejercicios**  
   - Desarrolle los programas en el entorno de programacion Google colab [https://colab.research.google.com/]  
   - Una vez finalizados, copie el código a los archivos `.ipynb` correspondientes en su repositorio.  
   - Cada archivo debe contener:
     - La implementación de su solución.  

5. **Buenas prácticas**  
   - Use **nombres de predicados claros y significativos**.
---

## 🚀 Entrega  

- **Plazo**: La entrega debe realizarse a mas tardar el proximo lunes, se habilitara una tarea en Moodle para adjuntar el link del repositorio.

---

## ✅ Criterios de Evaluación  

1. **Correctitud de las soluciones** (funcionalidad de los predicados).  
2. **Cumplimiento de la estructura solicitada** (archivos independientes en `lab01/`).  
3. **Claridad en la codificación** (nombres, comentarios y legibilidad).  
4. **Uso adecuado de variables** (incluyendo variables anónimas donde corresponda).  

---

## 💡 Recomendaciones  

- Antes de subir sus archivos, **ejecute y verifique** cada consulta en el compilador en linea.  
- Mantenga su repositorio organizado y actualizado.

---

## Ejercicio 1 - Datos — Simples y Estructurados

1. **Teniendo como base el siguiente codigo**
```
# Estado inicial
saldo = 500_000      # Saldo de la cuenta
deposito = 150_000   # Monto a depositar
retiro = 80_000      # Monto a retirar

# Actualización del estado
saldo = saldo + deposito   # Se deposita dinero
saldo = saldo - retiro     # Se retira dinero

# Salida del estado final
print("Saldo final de la cuenta:", saldo)
```

* Declara nuevas variables:
  - interes = 0.02 (2% mensual)
  - saldo_final como el saldo actualizado con el interés aplicado.

* Muestra el resultado usando un f-string, por ejemplo:
  - print(f"Saldo final con interés: ${saldo_final:.2f}")

* Modifica el código para que el usuario pueda ingresar los valores por teclado usando input() y convierte las entradas a float.

* ¿Qué representa el estado inicial y el estado final del programa?
  - Explica cómo cada instrucción afecta la memoria.


2. **Teniendo como base el siguiente codigo**

```
# Lista inicial de temperaturas en °C
temperaturas = [22.5, 23.0, 21.8, 24.3, 25.1]

# Operaciones básicas
print("Temperaturas:", temperaturas)
```

* Agrega una nueva temperatura al final de la lista.
* Elimina la primera temperatura registrada.
* Inserta una temperatura en la segunda posición.
* Muestra la lista ordenada de menor a mayor.
* Calcula la diferencia entre la temperatura más alta y la más baja, y calcula el promedio de todas las temperaturas.
* Encuentra el índice (posición) de la temperatura 23.7.
* Muestra las temperaturas de la 2da posicion a la 4ta posicion
* Muestra las tres primeras temperaturas.


3. **Teniendo como base el siguiente codigo**

```
# Lista de productos en una tienda
inventario = [
    {"nombre": "Pan", "precio": 1500, "stock": 30},
    {"nombre": "Leche", "precio": 3500, "stock": 15},
    {"nombre": "Café", "precio": 8000, "stock": 10},
]

```


* Muestra el nombre del primer producto.
* Agrega un nuevo producto al inventario.
* Disminuye el stock de “Leche” en 2 unidades (venta).
* Calcula el valor total del inventario (precio * stock por producto).
* Muestra los productos cuyo stock sea menor a 10.
* Aumenta el precio de todos los productos en un 10%.
* Redondea los precios con round(p["precio"], 2) para evitar decimales largos.
* Busca un producto por nombre (ingresado por el usuario) y muestra el producto encontrado, ten en cuenta que no puede estar.
* Elimina un producto del inventario si su stock es 0.
* Ordena la lista por precio ascendente.

4. **Teniendo en cuenta el siguiente codigo**

```
# Tupla: coordenadas (x, y)
punto = (3, 7)
print("Punto:", punto)
```

* Crea una tupla rectangulo = (ancho, alto).
* Calcula su área y perímetro.
* Intenta cambiar el valor de ancho.
  - ¿Qué error obtienes? ¿Por qué?

```
posiciones = [(0, 0), (1, 2), (3, 4)]
```

* Calcula la distancia total recorrida dadas las posiciones anteriores

5. **Teniendo como base el siguiente codigo**

```
biblioteca = {
    "libros": [
        {"titulo": "1984", "autor": "George Orwell", "prestado": False},
        {"titulo": "El Principito", "autor": "Antoine de Saint-Exupéry", "prestado": True},
    ],
    "usuarios": ["Ana", "Luis", "María"]
}

```

* Muestra cuántos libros están prestados y cuántos disponibles.
* Agrega un nuevo libro.
* Marca como prestado el libro “1984”.
* Muestra el estado actualizado del sistema (usa print(biblioteca)).

---


## Ejercicio 2 - Instrucciones simples y estructuradas

1. **Teniendo en cuenta el siguiente codigo**

```
edad = int(input("Ingrese su edad: "))
tiene_licencia = input("¿Tiene licencia? (s/n): ")
```

* Complementa el codigo para mediante condicionales determinar si el usuario puede conducir o no
* Añade otro requisito (por ejemplo: “no estar sancionado”).


2. **Teniendo en cuenta el siguiente codigo**

```
for i in range(1, 6):
    print(f"Iteración número {i}")

```

* Calcula la suma de los primeros n números naturales.
* Imprime solo los números pares usando if.
* Agrega un acumulador y muestra el resultado final.
* Usando el ejercicio anterior de las temperaturas, encuentra las temperaturas mayores al promedio


3. **Teniendo en cuenta el siguiente codigo**

```
contador = 0
while contador < 5:
    print("Contador:", contador)
    contador += 1
```

* Modifica el ciclo para contar hacia atrás.
* Crea un programa que solicite números hasta que el usuario ingrese 0.
* Explica qué parte del código representa el estado del ciclo.

---

4. **Teniendo en cuenta el siguiente codigo**

```
suma_pares = 0
for i in range(1, 11):
    if i % 2 == 0:
        suma_pares += i

print("Suma de los pares:", suma_pares)
```

* Agrega otra variable para acumular los impares.
* Representa el estado final como un diccionario (suma_pares y suma_impares)
* Explica cómo el estado cambia dentro del bucle.

5. **Teniendo en cuenta el siguiente codigo**

```
productos = []
while True:
    nombre = input("Ingrese producto (o 'fin' para salir): ")
    if nombre == "fin":
        break
    precio = float(input("Precio: "))
    cantidad = int(input("Cantidad: "))
    productos.append({"nombre": nombre, "precio": precio, "cantidad": cantidad})

# Mostrar total
total = 0
for p in productos:
    total += p["precio"] * p["cantidad"]

print("Total del inventario:", total)
```

* Usa continue para saltar productos con precio negativo o cantidad menor a 0.
* Muestra el producto más caro usando max().
* Representa el estado final del inventario como lista de diccionarios.

---

## Ejercicio 3 - Aplicación práctica (integración + API)

1. **Teniendo en cuenta el siguiente codigo**

```
import requests

# Llamado a una API pública
url = "https://jsonplaceholder.typicode.com/users"
response = requests.get(url)
usuarios = response.json()
# Procesamiento imperativo
nombres = []
for u in usuarios:
    nombres.append(u["name"])

print("Usuarios encontrados:")
for n in nombres:
    print("-", n)

```

* Filtrar solo los usuarios cuyo correo termine en .biz.
  - Mostrar el nombre de estos usuarios

2. **Teniendo en cuenta el siguiente codigo**
   
```
import requests

# Entrada de datos
nombre_pokemon = input("Ingrese el nombre de un Pokémon: ").lower()

# Llamado a la API
url = f"https://pokeapi.co/api/v2/pokemon/{nombre_pokemon}"
respuesta = requests.get(url)

# Verificación del estado de la respuesta
if respuesta.status_code == 200:
    datos = respuesta.json()

    # Modelado del estado del Pokémon
    pokemon = {
        "nombre": datos["name"],
        "altura": datos["height"],
        "peso": datos["weight"],
        "tipos": [t["type"]["name"] for t in datos["types"]],
        "habilidades": [h["ability"]["name"] for h in datos["abilities"]]
    }

    # Salida del estado actual
    print("\n📘 Información del Pokémon")
    print(f"Nombre: {pokemon['nombre'].capitalize()}")
    print(f"Altura: {pokemon['altura']}")
    print(f"Peso: {pokemon['peso']}")
    print(f"Tipos: {', '.join(pokemon['tipos'])}")
    print(f"Habilidades: {', '.join(pokemon['habilidades'])}")

else:
    print("Pokémon no encontrado. Verifique el nombre ingresado.")

```

* Agregar condicionales adicionales (if / elif / else):
  - Si el Pokémon tiene más de un tipo, mostrar "Pokémon de tipo mixto".
  - Si el peso es mayor a 100, mostrar "Pokémon de gran tamaño".
  - En caso contrario, "Pokémon ligero".

* Usar for para listar las habilidades una por una
* Añade algun otro uso que consideres interesante para la respuesta de la api
  
---

## Retrospectiva
1. ¿Cuál fue el tiempo total invertido en el laboratorio por cada uno de ustedes? (Horas/Hombre)
2. ¿Cuál es el estado actual del laboratorio? ¿Por qué?
3. ¿Cuál consideran fue el mayor logro? ¿Por qué?
4. ¿Cuál consideran que fue el mayor problema técnico? ¿Qué hicieron para resolverlo?
5. ¿Qué hicieron bien como equipo? ¿Qué se comprometen a hacer para mejorar los resultados?
6. ¿Qué referencias usaron? ¿Cuál fue la más útil? Incluyan citas con estándares adecuados.

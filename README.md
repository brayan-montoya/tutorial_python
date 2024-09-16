# Tutorial básico de python

Python admite varios tipos de datos nativos:

- **Enteros (int):** Números enteros, como `10`, `-5`.
- **Punto Flotante (float):** Números decimales, como `3.14`, `-0.1`.
- **Cadenas de Texto (str):** Secuencias de caracteres, como `"Hola, Mundo!"`.
- **Booleanos (bool):** Valores de verdad, `True` o `False`.  .



##  Operaciones entre Tipos de Datos

### Operaciones Numéricas
Python permite realizar operaciones matemáticas básicas:
- Suma (+), resta (-), multiplicación (*), división (/), módulo (%), exponenciación (**).

```python
a = 10
b = 4
suma = a + b          
resta = a - b         
producto = a * b     
division = a / b      
potencia = a ** b     
modulo = a % b     
print(suma)
print(resta)
print(producto)
print(potencia)
print(modulo)
```

### Operaciones Lógicas
Los operadores lógicos (and, or, not) se utilizan para combinar condiciones.

```python 
x = True
y = False

print(x and y) 
print(x or y)   
print(not x)   
```

### Operaciones con cadenas de texto
Podemos concatenar (+) o repetir (*) cadenas de texto.
```python
nombre = "Python"
saludo = "Hola, " + nombre
repetir = nombre * 3

print(saludo)    
print(repetir)   
```
##  Estructuras de Datos Básicas 

### Tupla
Una tupla es una colección ordenada e inmutable.
```python
mi_tupla = (1, 2, 3)
print(mi_tupla[1])
```
### Lista
Una lista es una colección ordenada y mutable.

````python
mi_lista = [1, 2, 3]
mi_lista[0] = 10  
mi_lista.append(4)  
print(mi_lista) 
````
### Set (conjunto)
Un set es una colección desordenada de elementos únicos.

````python
mi_set = {1, 2, 3, 3}
print(mi_set) 
````

### Diccionario
Un diccionario es una colección de pares clave-valor.

````python
mi_diccionario = {"nombre": "Brayan", "edad": 27}
print(mi_diccionario["nombre"])  
mi_diccionario["edad"] 
````

## Modificar información 
### Modificar lista 
Puedes modificar los elementos de una lista asignando nuevos valores a posiciones específicas o usando métodos incorporados para agregar, eliminar o cambiar elementos.

```python
mi_lista = [10, 20, 30, 40, 50]

# Modificar un elemento
mi_lista[0] = 15 

# Agregar elementos al final de la lista
mi_lista.append(60)

# Insertar un elemento en una posición específica
mi_lista.insert(2, 25)  

# Eliminar un elemento específico por su valor
mi_lista.remove(40)

# Eliminar un elemento por su índice
elemento_eliminado = mi_lista.pop(3) 

print(mi_lista)  # [15, 20, 25, 50, 60]
print("Elemento eliminado:", elemento_eliminado)
```
### Modificar Diccionarios
Puedes modificar los diccionarios añadiendo nuevos pares clave-valor, actualizando los existentes o eliminando pares específicos.

````python
mi_diccionario = {"nombre": "Brayan", "edad": 27, "ciudad": "Medellín"}

# Modificar un valor existente
mi_diccionario["edad"] = 27  

# Agregar un nuevo par clave-valor
mi_diccionario["profesion"] = "Economía"

# Eliminar un par clave-valor
del mi_diccionario["ciudad"]

# Obtener y eliminar un elemento utilizando pop()
ciudad = mi_diccionario.pop("ciudad", "No encontrada")  

print(mi_diccionario)  
print("Ciudad eliminada:", ciudad)
````
### Modificar sets (conjuntos)
Los sets son colecciones desordenadas de elementos únicos. Puedes agregar o eliminar elementos de un set, pero no puedes acceder a ellos por índice.

````python
mi_set = {1, 2, 3, 3}

# Agregar un nuevo elemento
mi_set.add(4)

# Eliminar un elemento (si existe)
mi_set.discard(2)  # No arroja error si el elemento no existe
mi_set.remove(1)   # Arroja un error si el elemento no existe

# Eliminar un elemento aleatorio
elemento_eliminado = mi_set.pop()  
print(mi_set)  
print("Elemento eliminado:", elemento_eliminado)
````
### Modificar Tuplas
Las tuplas son inmutables, lo que significa que no puedes cambiar sus elementos directamente después de crearlas. Sin embargo, puedes convertir una tupla en una lista, modificarla, y luego convertirla de nuevo en una tupla.

```python
mi_tupla = (1, 2, 3)

# Convertir tupla a lista para modificarla
lista_temporal = list(mi_tupla)
lista_temporal[0] = 10  

# Convertir de nuevo a tupla
mi_tupla = tuple(lista_temporal)

print(mi_tupla)  
```
## Estructuras de Control
### Condicionales
Los condicionales permiten ejecutar código basado en condiciones.

```python
edad = 18
if edad >= 18:
    print("Eres mayor de edad.")
else:
    print("Eres menor de edad.")
```

## Loops (bucles)
### Bucle for
El bucle for se utiliza para iterar sobre una secuencia.

```python
for i in range(5):
    print(i)  
```
### Bucle while
El bucle while se repite mientras una condición sea verdadera.

```python
contador = 0
while contador < 5:
    print(contador)
    contador += 1
```

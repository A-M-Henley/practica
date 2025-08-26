En este capítulo se introduce *El tipo de dato más importante en Python: las listas*.  
Las listas permiten almacenar múltiples valores en una sola variable, manipularlos fácilmente y son muy utilizadas en programación.  

---

## ¿Qué es una lista?
Una *lista* es una colección ordenada de elementos, que pueden ser números, cadenas de texto u otros objetos.  
Se define entre corchetes [], separando los elementos con comas:

```python
bicycles = ['trek', 'cannondale', 'redline', 'specialized']
print(bicycles)


---
 Acceder a elementos de una lista

El índice comienza en 0.

Se puede acceder tanto desde el inicio como desde el final con índices negativos.


print(bicycles[0])         # trek
print(bicycles[1].title()) # Cannondale
print(bicycles[-1])        # specialized (último elemento)


---
 Usar valores individuales de una lista

Podemos usar un valor dentro de un mensaje o en cálculos:

message = f"My first bicycle was a {bicycles[0].title()}."
print(message)


---
 Cambiar, agregar y eliminar elementos

Modificar elementos

motorcycles = ['honda', 'yamaha', 'suzuki']
motorcycles[0] = 'ducati'
print(motorcycles)  # ['ducati', 'yamaha', 'suzuki']

Agregar elementos

Al final con append():


motorcycles.append('kawasaki')

En una posición específica con insert():


motorcycles.insert(0, 'bmw')

Eliminar elementos

Con del:


del motorcycles[0]

Con pop() (elimina y devuelve el valor):


popped_motorcycle = motorcycles.pop()
print(popped_motorcycle)

Con remove() (elimina por valor):


motorcycles.remove('yamaha')


---
 Organizar una lista

Podemos ordenar y reordenar listas de varias formas:

Orden permanente con sort():


cars = ['bmw', 'audi', 'toyota', 'subaru']
cars.sort()
print(cars)  # ['audi', 'bmw', 'subaru', 'toyota']

Orden inverso:


cars.sort(reverse=True)

Orden temporal con sorted():


print(sorted(cars))

Invertir el orden actual con reverse():


cars.reverse()


---

Podemos contar los elementos con len():

len(cars)

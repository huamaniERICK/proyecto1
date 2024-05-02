# CONTROL DE FLUJO
Un programa o script de Python es un conjunto de instrucciones analizadas y ejecutadas por el intérprete de arriba hacia abajo y de izquierda a derecha. Cuando todas las instrucciones se han ejecutado, el programa termina.
# Condicional
Una de estas herramientas es el condicional. A partir de la palabra reservada if, le indicamos a Python que queremos ejecutar una porción de código solo si se cumple una determinada condición (es decir, si el resultado es True, como vimos anteriormente).
> ejemplo.
```python
edad = 30

if edad >= 18:
    print("Eres un adulto.")
```
Primero definimos una variable edad, cuyo valor es un entero, 30. Luego, a través del condicional indicamos que queremos imprimir "Eres un adulto." en pantalla si se cumple la condición de que el valor de edad sea mayor o igual a 18.
>ejemplo
```python
if edad >= 18:
    print("Eres un adulto.")
print("¡Hola, mundo!")
```
Ahora bien, para ejecutar un bloque de código en caso que no se cumpla la condición, empleamos la palabra reservada else.
>ejemplo

```python
if edad >= 18:
    print("Eres un adulto.")
else:
    print("Aún no eres un adulto.")
```    
Por último, podemos especificar otras condiciones en caso que la primera no se cumpla vía elif.
>ejemplo
```python

if edad >= 18 and edad < 65:
    print("Eres un adulto.")
elif edad >= 65:
    print("Eres un adulto mayor.")
else:
    print("Aún no eres un adulto.")
```    
# Interacción con el usuario
Python incluye una función llamada input(), similar a print(), pero que exhorta al usuario a escribir algo en la consola, que luego es retornado como una cadena.
>ejemplo
```python
nombre = input("Escribe tu nombre: ")
print("Hola", nombre)
```
Así, este código solicita al usuario que escriba su nombre y, una vez obtenido, imprime un saludo personalizado en la pantalla. Sabido esto, podemos adaptar nuestro código anterior para solicitar la edad del usuario y en consecuencia mostrar el mensaje correspondiente.
>ejemplo
```python
edad = int(input("Escribe tu edad: "))

if edad >= 18 and edad < 65:
    print("Eres un adulto.")
elif edad >= 65:
    print("Eres un adulto mayor.")
else:
    print("Aún no eres un adulto.")
```
Dado que input() siempre retorna una cadena de caracteres, debemos primero convertirla a un entero vía la función incorporada int() para poder efectuar las comparaciones pertinentes.
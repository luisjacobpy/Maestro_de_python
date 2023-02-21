

````python
"""
Enumerate
- Multiple asignation

"""
#
elements  = ["Hi!", 4, "Bye!", [1,2,3]]

# Multiple assignment
a, b, c = 10, 50, 100
print(a, b, c)

# Tupla
(a,b,c) = (10,50,100)

# Enumerator function
#cast use function list
print(list(enumerate(elements))) # [(0, 'Hi!'), (1, 4), (2, 'Bye!'), (3, [1, 2, 3])]

for tupla in enumerate(elements):
    print(tupla)
"""
(0, 'Hi!')
(1, 4)
(2, 'Bye!')
(3, [1, 2, 3])
"""

for indice, valor in enumerate(elements):
    print(indice, valor)

```
## Challenge enumerate
 
### Función enumerate
En este ejercicio se te va a facilitar una variable iniciales que contiene una lista con un número indeterminado de cadenas de texto.

Tu objetivo es modificar las cadenas de esa lista por la letra inicial de cada cadena en la lista utilizando, si lo requieres, la función enumerate.

Supongamos que iniciales tiene el siguiente valor ["Hola", "Mundo"], tu objetivo sería transformar esos valores a ["H", "M"].

Notas:

Recuerda que para modificar los valores en una lista necesitas hacerlo mediante el índice de cada elemento:

```python
from evaluate import iniciales
 
# Recorremos mediante un enumerador cada cadena en la lista
for i,cadena in enumerate(iniciales):
    # Modificamos cada cadena por su letra inicial
    iniciales[i] = iniciales[i][0]s):
    
```

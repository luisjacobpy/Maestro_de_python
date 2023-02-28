# Colecciones
* Tuplas
* Conjuntos 
* Diccionarios
* Pilas
* Colas


## Tuplas / Tuple
Son inmutables, se utilizan para asegurarnos de que ciertos datos no se puedan modificar.
* Aceptan indexación y slicing
```python
tuple = (100, "Hi!", [1,2,3])
print(tuple)
```
```python
"""
Tuple object does not support item assignment
"""
tuple = (100, "Hi!", [1,2,3], -50)
print(tuple)

# Check the first element
print(tuple[0]) # 100
# Check the last element
print(tuple[-1])  # -50

# Slicing, check second element to the end
print(tuple[1:]) # ('Hi!', [1, 2, 3], -50)

# Acces to list into tuple
print(tuple[2][0]) # 1

# Function len
print(len(tuple))

# Index for search a element
print(tuple.index(100)) # 0
print(tuple.index("Hi!")) # 1

# Count
print(tuple.count(100)) # 1
print(tuple.count(34)) # 0
```

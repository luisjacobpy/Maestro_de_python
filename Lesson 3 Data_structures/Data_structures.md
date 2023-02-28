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

## Conjuntos
Son colecciones desordenadas de elementos unicos.
Se utilizan para hacer pruebas de pertenencia a grupos y eliminación de elementos duplicados.
Se dice que los conjunto s son desordenados porque a medida que añadimos elementos este orden no se conserva.

```python
# Conjunto vacio
# conjunto = set()

# COn valores
conjunto = {1,2,3}
print(conjunto) # {1, 2, 3}

# Metodo Add
conjunto.add(4)
print(conjunto) # {1, 2, 3, 4}

conjunto.add(0)
print(conjunto) # {0, 1, 2, 3, 4}

conjunto.add('H')
print(conjunto) # {0, 1, 2, 3, 4, 'H'}

conjunto.add('A')
conjunto.add('z')

print(conjunto) # {0, 1, 2, 3, 4, 'H', 'A', 'z'}
```
### Comprobar la pertenencia a grupos con conjuntos
```python
grupo = {'Hector', 'Juan', 'Mario'}

print('Hector' in grupo) # True

print('Maria' in grupo) # False

print('Hector' not in grupo) # False

```
### Conjuntos | Eliminar valores repetidos
```python
# Se eliminan los valores repetidos
test = {'Luis','Luis','Luis','Jacobo','Jacobo'}
print(test) # {'Luis', 'Jacobo'}
```
### Conjuntos | Transformando otras colecciones a conjuntos para eliminar duplicados
```python
# Transformando otras colecciones a conjuntos para eliminar duplicados
list_1 = [1,2,3,3,2,1]
# Si hacemos un 'Cast', transformamos esta list_1 a un conjunto.
c = set(list_1)
print(c) # {1, 2, 3}

# Transformamos el conjunto a una lista
list_2 = list(c)
print(list_2) # [1, 2, 3]

# En una sola linea de codigo podemos hacer el cambio
list_1 = [1,2,3,3,2,1]
print(list_1) # [1, 2, 3, 3, 2, 1]
list_2 = list(set(list_1)) #
print(list_2) # [1, 2, 3]

# Para cadenas de caracteres / Stings
s = 'This is a sttring, in string, for string'
print(set(s)) # {'a', ' ', 'r', 'g', ',', 'n', 'o', 'i', 's', 'T', 'f', 'h', 't'}
```

### Conjuntos |Learning_Challenge_Conjuntos
El siguiente ejercicio te servirá para practicar la manipulación de conjuntos.

Debes realizar las siguientes instrucciones de forma ordenada sobre la variable grupo para que el ejercicio valide correctamente:

Añade los siguientes usuarios: Ana, Ramón, Marta, Eric y David (respeta las tildes)

Elimina (*) los usuarios Mario, Miguel y Ramón.

Optativo: Cuando tu solución valide, dale una vuelta de tuerca. A ver si se te ocurre alguna forma de optimizarlo utilizando listas y bucles.

(*) Para eliminar un registro de un conjunto puedes utilizar su método interno conjunto.remove("registro").

```python
# Variables del ejercicio (no las modifiques)
grupo = {"Miguel", "Blanca", "Mario", "Andrés"}

# Completa el ejercicio
# Add
grupo.add('Ana')
grupo.add('Ramón')
grupo.add('Marta')
grupo.add('Eric')
grupo.add('David')

# Remove
grupo.remove('Mario')
grupo.remove('Miguel')
grupo.remove('Ramón')
print(grupo) # {'Blanca', 'Andrés', 'David', 'Marta', 'Eric', 'Ana'}
  
```

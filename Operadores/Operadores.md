# Expresiones
Los operadores aritmeticos (+,-,/*) dan lugar a expresiones de distintos tipos.

* Aritméticas si ambos operadores son literales.

* Algebraicas si al menos un operando es una variable.


## El tipo lógico
* Mínima expresión racional
* Representada por dos valores
* Verdadero y falso

Negación logica
No verdadero = Falso
No falso = verdadero

```python
1+1 == 3
```
```python
false
```
```python
1+1 == 2
```
```python
True
```

## Operadores relacionales
En una lista llamada expresiones encontramos diferentes operaciones relacionales, ¿podrías determinar mentalmente el resultado de cada expresión y almacenarlo en una nueva lista llamada resultados? Esta lista debe contener únicamente valores lógicos True y False. Por ejemplo, supongamos esta lista:

expresiones = [1 == 1, 1 < 0]
La respuesta que se espera que escribas es:

resultados = [True, False]
Correspondiendo True al resultado de 1==1 y False al de 1<0,  es decir, los resultados deben concordar con la posición de las expresiones, siendo resultados[0] la respuesta a la expresión expresiones[0].

La lista de expresiones que debes calcular mentalment es la siguiente (se importará automáticamente durante la comprobación de la solución):

expresiones = [False == True, 10 >= 2*4, 33/3 == 11, True > False, True*5 == 2.5*2]
Sugerencia: ¿Eres muy perezos@ como para pensar? ¡Deja que Python calcule las expresiones por ti!

Solución:
```python
# no borres esta línea
from evaluate import expresiones

# completa el ejercicio
resultados = expresiones[:]
print(resultados)
```

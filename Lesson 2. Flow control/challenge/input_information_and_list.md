Realiza un programa que pida ala usuario un número entero del 0 al 9
y que mientras el numero no sea correcto se repita el proceso.
Luego debe comprobarse si el numero se encuentra en la lista de numeros y notificarlo.

```python
numbers = [1, 3, 6, 9]

# Cicle
while True:
    number = int(input("Write a number between 0 and 9: "))
    if number >= 0 and number <=9:
        break # Break whe cicle is True
# Value in list
if number in numbers:
    print(f"The number: {number} is in the list of numbers: {numbers}")
else:
    print(f"The number: {number} is NOT in the list of numbers: {numbers}")
```

### Output
```Bash
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
[-10, -9, -8, -7, -6, -5, -4, -3, -2, -1, 0]
[0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20]
[-19, -17, -15, -13, -11, -9, -7, -5, -3, -1]
[0, 5, 10, 15, 20, 25, 30, 35, 40, 45, 50]
```

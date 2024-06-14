print("")
print("Cerradura: La suma de dos numeros reales siempre da como resultado otro numero real.")
print("")
print("a + b pertenece R")
print("")

#solicitar al usuario que ingrese dos numero.
num1 = float(input("ingresa el primer numero"))
num2 = float(input("ingresa el segundo numero"))
suma = num1 + num2

#verifica si la duma es un numero entero
if suma.is_integer():
    resultado = "entero"
else:
    resultado = "racional"

#muestra el resultado de la suma y su tipo
print("")
print("El resultado de la suma", suma)
print("El resultado es un numero", resultado)
print("")
#programa con condiciones anidadas
#solicitar al usuario numero 1
num1 = float(input("ingresa el primer numero"))
print("")
#solicitar al usuario el segundo numero
num2 = float(input("ingresa el segundo numero"))
if num1 > num2:
    print("El primer numero ({}) es mayor que el segundo numero".format(num1, num2))
elif num1 < num2:
    print("El segundop numero ({}) es mayor que el primer numero".format(num2, num1))
else:
    print("Ambos numeros son iguales")
import math

def calcular_lado_faltante():
    print("Introduce los valores de dos lados del triángulo rectangulo: ")
    print("Deja en blanco el valor del lado que desee calcular: ") 

    cate1=input("Lado cate1 : ")
    cate2 = input("Lado cate2:  ")
    h=input("h: ")

    cate1=float(cate1) if cate1 else None
    cate2=float(cate2) if cate2 else None
    h=float(h) if h else None

    if cate1 is None and cate1 is not None and h is not None:
        cate1 = math.sqrt(h**2-cate2**2)
        lado_calculado= "cate1"
    elif cate2 is None and cate1 is not None and h is not None:
        cate2=math.sqrt(h**2-cate1**2)
        lado_calculado= "cate2"
    elif h is None and cate1 is not None and cate2 is not None:
        h=math.sqrt(cate1**2+cate2**2)
        lado_calculado="h"
    else:
        return "Error: Proporcione exactamente dos lados. "

    return f"El lado faltante es {lado_calculado} y su resultado es: {cate1 if lado_calculado == 'cate1' else cate2 if lado_calculado == 'cate2' else h:.2f}"

resultado=calcular_lado_faltante()
print(resultado) 

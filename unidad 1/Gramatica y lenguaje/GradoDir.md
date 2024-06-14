import maplotlib.pyplot as plt 
#Grafo dorigido con 4 valores
#Creamos un grafo vacía 
grafo = {}

#Agregamos vertices al grafo
grafo["A"] = ["B","C"]
grafo["B"] = ["D"]
grafo["C"] = ["D"]
grafo["D"] = []

#Imprimimos el grafo
print("Grafo:")
for vertice, adyacentes in grafo.items():
    print(f"{vertice} -> {adyacentes}")
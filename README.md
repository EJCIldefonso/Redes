# Redes

#Topología básica
grafo1={
'a':{'b':3,'c':8},
'b':{'c':7,'d':5,'e':1},
'c':{'d':2},
'd':{'e':4},
'e':{},
'f':{},
'g':{},
} 

def dijkstra(grafo,inicio,destino):
    caminoMasCorto = {} 
    nodoAnterior = {} 
    nodosSinConocer = grafo 
    longitud = [] 
    for nodo in nodosSinVer:  
        longitudMasCorto[nodo] = 999
    longitudMasCorto[inicio] = 0
    while nodosSinConocer:
        minNodo = None



print("Grafo1: ")
dijkstra(grafo1, 'a', 'd') #Se busca el camino mas optimo desde "a" hacia "e" en el grafo1
print()
print("Grafo2: ")
dijkstra(grafo2, 'a', 'e') #Se busca el camino mas optimo desde "a" hacia "e" en el grafo2
print()
print("Grafo3:")
dijkstra(grafo3, 'c', 'h') #Se busca el camino mas optimo desde "a" hacia "e" en el grafo3

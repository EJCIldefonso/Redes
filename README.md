# Redes

#Topología básica

'a':{'b':3,'c':8},
'b':{'c':7,'d':5,'e':1},
'c':{'d':2},
'd':{'e':4},
'e':{},
'f':{},
'g':{},
} 

#Topología intermedia
grafo2={
'a':{'b':3,'c':1},
'b':{'d':1,'g':5},
'c':{'d':2,'f':5},
'd':{'e':4},
'e':{'h':5},
'f':{'h':5},
}

#Topología avanzada
grafo3={
'a':{'b':10,'d':8,'c':11},
'b':{'c':4,'g':10,'e':7,},
'c':{'e':2,'d':12,'f':3},
'd':{'f':2,'i':6},
'e':{'f':3,'g':4,'h':2},
'f':{'h':4,'i':3},
'g':{'h':2,'j':1},
'h':{'i':10,'j':5}
'i':{'j':2}
'j':{}

}


def dijkstra(grafo,inicio,destino):
    caminoMasCorto = {} 
    nodoAnterior = {} 
    nodosSinConocer = grafo 
    camino = [] 
    #Recorrer el grafo para asignar un valor grande al camino de todos los nodos menos al nodo inicial

    for nodo in nodosSinVer:  
        caminoMasCorto[nodo] = 999
    caminoMasCorto[inicio] = 0
 
    #Se recorre el grafo mientras exista un nodo sin ser conocer
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

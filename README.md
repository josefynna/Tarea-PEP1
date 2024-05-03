posicion_inicial = [0,0]
win = [4,4]

# Menú para preguntar la dirección que desea tomar el jugador. 
bandera1 = True
while(bandera1):
        print("¿Hacia donde te quieres mover?")
        print("1.Arriba")
        print("2.Abajo")
        print("3.Derecha")
        print("4.Izquierda")
        opcion = int(input("Usted ingreso la opcion: "))
    if (opcion == 1): 
        posicion_nueva = [posicion_inicial[0], posicion_inicial[1]+1]
    elif (opcion ==2):
        posicion_nueva = [posicion_inicial[0], posicion[1]-1]
    elif (opcion == 3):
        posicion_nueva = [posicion_inicial[0]-1, posicion_inicial[0]]
    elif (opcion == 4):
        posicion_nueva = [posicion_inicial[0]+1, posicion_inicial[0]]
    else:
        print("opción inválida")
if (0 <= posicion_nueva[0] <= 4) and (0 <= posicion_nueva[1] <= 4):
    posicion_inicial == posicion_nueva
bandera1 = False
if (posicion_nueva == win):
    print("Felicidades! ganaste!")
        

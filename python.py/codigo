tarifa = {"carro": 80, "moto": 40,}
tipos_vehiculo = {"carro": "c", "moto": "m"}

fila = 8
columnas = 8
entrada = (0,0)
salida = (fila - 1, columnas - 1)
mapa = [[ "p" for _ in range(columnas)] for _ in range(fila)]
registros = {}
minuto = 0

for i in range(fila):
    mapa[i][0] = "#"
for j in range(columnas):
    mapa[0][j] = "#"
mapa[entrada[0]][entrada[1]] = "E"
mapa[salida[0]][salida[1]] = "s"

opcion = ''
while opcion != "5":
    print("BIENVENIDO AL PARQUEADERO")
    print("1.  Mostrar mapa")
    print("2.  Ingresar vehiculo")
    print("3.  Retirar vehiculo")
    print("4.  ver estadisticas")
    print("5. salir")
    opcion = input("seleccione una opcion: ")

    if opcion == "1":
        for fila in mapa:
            print(''.join(fila)) #.join = juntar todo de filas

    elif opcion =="2":
        placa = input(("ingrese placa del vehiculo: ").upper())#.upper= combertir a mayusculas
        if placa in registros:
            print("El vehiculo esta en el parqueadero")
            continue

        print("tipos de vehiculos disponibles:")
        for tipo in tipos_vehiculo:
            print(f"- {tipo}")
        tipo = input("Ingrese el tipo de vehiculo: ").lower()#lower = minuscula
        if tipo not in tipos_vehiculo:
            print("tipo no valido")
            continue
        parqueadero = None
        for i in range(1, columnas):
            if mapa[i][j] == "p":
                parqueadero = (i, j)
                break

            if parqueadero:
                break

        if not parqueadero:
            print("no hay espacios disponibles ")
            continue

        mapa[parqueadero[0]][parqueadero[1]] = tipos_vehiculo[tipo]
        minuto += 1
        registros[placa] = {
            "entrada": minuto,
            "tipo": tipo,
            "posicion": parqueadero
        }
        print(f"vehiculo {placa} estacion en {parqueadero}")

    elif opcion =="3":
        placa = input("ingresar la placa del vehiculo a retirar: ").upper()#todo en mayuscula
        if placa not in registros:
            print("vehiculo no registrado")
            continue
        registro = registros[placa]
        entrada = registro["entrada"]
        minuto += 1
        salida = minuto
        minutos = max(1, salida - entrada)
        costo = minutos * tarifa[registro["tipo"]]
        parqueadero = registro["posicion"]
        mapa[parqueadero[0]][parqueadero[1]] = "p"
        print(f"vehiculo {placa} retirado con el tiempo: {minutos} min y el total a pagar es  de : {costo}")
        del registros[placa]
        #borrar

    elif opcion =="4":
        print(f"el vehiculo esta estacionado: {len(registros)}")
        for placa, registro in registros.items():#objetos que tiene el diccionario de regirtros
            tiempo = minuto - registro["entrada"]
            print(f" - {placa}  ({registro["tipo"]}): {tiempo}min")

    elif opcion == "5":
        print("que tenga buen dia")
    else:
        print("invalido")

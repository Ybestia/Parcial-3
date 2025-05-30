Sistema de Parqueadero
Este proyecto es un sistema básico de parqueadero en Python que Permite:
Mostrar el mapa del parqueadero (8x8)
Ingresar vehículos (carro/moto) y ubicarlos.
Retirar vehículos y calcular el costo por minuto.
Ver estadísticas de ocupación.
Tarifas
Vehículo	Tarifa por minuto
Carro	80
Moto	40
¿Para qué se implementó?

un simulador de parqueadero que hace entender el espacios, tiempos y cobros.
¿Por qué se consideró necesario?
Para practicar como se usa en manejo de las listas, condiccionales y diccionarios

¿Cómo se llevó a cabo su implementación?
Se creó una matriz para representar el parqueadero, un sistema de menú para interactuar con el usuario, y registros para gestionar los datos de los vehículos, tiempos y cobros.

Uso
Ejecuta el código y sigue las opciones del menú:
1️⃣ Mostrar mapa
2️⃣ Ingresar vehículo
3️⃣ Retirar vehículo
4️⃣ Ver estadísticas
5️⃣ Salir


mejoras:
- puede ingresar carro y moto
- cada vehiculo tiene didtintos precios

herramienta de inteligencia artificial:

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
        #del es borrar

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


Soporte para Diferentes Tipos de Vehículos
¿Para qué se implementó?
Para simular un parqueadero realista donde pueden ingresar carros y motos

¿Por qué se consideró necesario?
para que sea mas realista de la mayoria de parqueadero que se maneja actualmente

¿Cómo se llevó a cabo su implementación?
Se amplió el diccionario tarifa para incluir

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

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
Uso
Ejecuta el código y sigue las opciones del menú:
1️⃣ Mostrar mapa
2️⃣ Ingresar vehículo
3️⃣ Retirar vehículo
4️⃣ Ver estadísticas
5️⃣ Salir



 1.  Soporte para Diferentes Tipos de Vehículos
¿Para qué se implementó?
Para simular un parqueadero realista donde pueden ingresar carros y motos

¿Por qué se consideró necesario?
para que sea mas realista de la mayoria de parqueadero que se maneja actualmente

¿Cómo se llevó a cabo su implementación?
Se amplió el diccionario tarifa para incluir:
tipos_vehiculo = {"carro": "c", "moto": "m"}



2.  Sistemas de Cobro Diferenciado por Vehículo
¿Para qué se implementó?
Para calcular el costo de parqueo de forma justa, dependiendo del tipo de vehículo y el tiempo.

¿Por qué se consideró necesario?
hay una gran diferencia entre carro y moto por lo cual tambien hay diferencia en precios

¿Cómo se llevó a cabo su implementación?
Se definió un sistema de tarifas por minuto en el diccionario tarifa
tarifa = {"carro": 80, "moto": 40,}

3. Diferentes Tipos de Vehículos: Carros (c) y Motos (m)
¿Para qué se implementó?
Para simular un parqueadero realista que permita el ingreso de carros y motos, cada uno con su propio costo de parqueoy situados en donde esta.

¿Por qué se consideró necesario?
En un parqueadero real, hay distintos tipos de vehículos, y es importante diferenciar cuáles están estacionados y dónde están ubicados.

¿Cómo se llevó a cabo su implementación?
tipos_vehiculo = {"carro": "c", "moto": "m"}




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

# Prueba backend Connectivity Innovation
El ejercicio es muy simple, en el área de connectivity innovation
disponemos de una plataforma de microservicios con la que disminuir el time-to-market de 
los nuevos productos que lanzamos, la idea es replicar esta plataforma (en un modo mucho más reducido)

## Desarrollo
Utiliza Golang y Python para escribir dos microservicios que se comuniquen entre ellos usando
websockets. (Como si un chat se tratase) 

## Consideraciones
1. Elige cual será el cliente y cual será el servidor, para nosotros no es relevante.
2. Al cliente se le pasarán una serie de mensajes por stdin  que deberá enviar ordenados
por orden alfabético al servidor.
3. El servidor siempre contestará con el número de caracteres del mensaje emitido por el cliente.
4. La entrega consiste en un repositorio de github con el código de ambos microservicios, en la raíz
hay dos carpetas, client y server que contienen el código de cada una.

El servicio se levanta de la siguiente forma:
```
./server --addr localhost:8080
```
```
["hola", "que tal?", "soy el lobo"] | ./client --server-addr localhost:8080
```

## Valoración
1. Se valorará muy positivamente que se utilice Docker y docker-compose para orquestar los servicios.
2. Se valorará muy positivamente que se utilice Django y Gin como frameworks para construir los microservicios.
3. Se valorará negativamente no utilizar Python y/o Golang.
4. Se valorará la organización del código (arquitectura) así como buenas prácticas utilizadas, gestión
de errores, etc..
5. Se pueden añadir tests si lo deseas, sabemos que puede ser largo pero cuantas más aportaciones mejor.


# Practica_3
## Integrantes:  
- Francisco javier Godinez Lopez
- Pablo Axel Silva Fuentes
- Eduardo David Salas Ayala
## Introducción:  
La práctica tiene como objetivo programar una trayectoria de varios movimientos para el brazo robótico Epson utilizando el software Epson RC+. Donde se realiza la planificación de la trayectoria, que consiste en encontrar una ruta transitable entre una posición de origen y diferentes posiciones para realizar distintas acciones. Teniendo como posición de origen o "Home" unas coordenadas previamente especificadas; la trayectoria consiste en intercambiar la posiciones de dos objetos, definiendo los movimientos necesarios del brazo para poder realizar el intercambio.
## Instrucciones:  

El movimiento del brazo consiste en recoger un objeto(fusible 1) e intercambiarlo de lugar con otro objeto(fusible 2), para lograrlo el brazo realizo los siguientes pasos:
1. Mover del origen hacia una posicion arriba del fusible 1 y abrir la garra para posteriormente bajar hacia el fusible 1
2. Cerrar la garra tomando el fusible 1 y subir a la posicion anterior
4. Dirigirse a la posicion intermedia, bajar y soltar el fusible 1
6. Subir a la posicion intermedia y dirigirse a la posicion arriba del fusible 2
7. Bajar hacia el fusible 2, cerrar la garra tomando el fusible 2 y subir a la posicion anterior
8. Dirigerse a la posicion original del fusible 1
9. Bajar para soltar el fusible 2 y posteriormente volver a subir
10. Dirigirse a la posicion intermedia, bajar y tomar el fusible 1
11. Dirigerse a la posicion original del fusible 2
12. Bajar para soltar el fusible 2 y posteriormente volver a subir
13. Dirigirse a la posicion Home


![image](https://github.com/user-attachments/assets/45941ddc-1fae-4280-8c13-9384bd75e29e)


De tal manera que el codigo desarrollado quedo de la siguiente manera:
```
Function main
Home
Go Arriba1
On 2
Go Abajo1
Off 2
Go Arriba1
Go Arriba2
Go Soltar1
On 2
Go Arriba2
Go Arriba3
Go Abajo2
Off 2
Go Arriba3
Home
Go Arriba1
Go Abajo1
On 2
Go Arriba1
Go Arriba2
Go Soltar1
Off 2
Go Arriba2
Go Arriba3
Go Abajo2
On 2
Go Arriba3
Home
Fend
```

En el siguiente video se muestra el movimiento realizado utilizando el código anterior, cuyo objetivo fue intercambiar la posicion de dos fusibles. Este proceso demuestra el correcto funcionamiento del sistema y cumple con los objetivos establecidos para la práctica

[https://drive.google.com/drive/folders/1HjE7HlarkAU024qj9DKuwbbv-v8hnPId?usp=drive_link](https://drive.google.com/drive/folders/1qcI8ykO0PPjPOEMBOcoG6jSuusFKTzMy?usp=sharing)

## Conclusiones:  
### Francisco Javier Godinez Lopez:
Esta práctica permitió profundizar en la programación de trayectorias para un brazo robótico utilizando el software Epson RC+. A través del intercambio de posiciones entre dos objetos, se adquirió una comprensión más clara sobre la precisión y el control del brazo robótico. El uso de los comandos ON, GO y OFF fue clave para completar los movimientos de manera eficiente, lo que demostró las capacidades del sistema para realizar tareas automatizadas con exactitud.


### Pablo Axel Silva Fuentes: 
A través de esta práctica, se logró programar con éxito una secuencia de movimientos para el brazo robótico, lo que resaltó la importancia de los comandos básicos en la automatización de procesos. La correcta implementación de la planificación de trayectorias permitió intercambiar dos objetos de manera precisa, destacando la precisión y la eficiencia del sistema robótico.

### Eduardo David Salas Ayala: 
La práctica fue de gran ayuda para mejorar la comprensión de la programación de trayectorias y donde la ejecución de los movimientos necesarios para intercambiar dos objetos permitió comprender mejor las capacidades del software Epson RC+ y la importancia de los comandos básicos en la programación de tareas repetitivas y precisas.

## Referencias bibliográficas
- Localización y planificación de trayectorias - TEKNIKER. (s. f.). https://www.tekniker.es/es/localizacion-y-planificacion-de-trayectorias

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

https://drive.google.com/drive/folders/1HjE7HlarkAU024qj9DKuwbbv-v8hnPId?usp=drive_link

## Conclusiones:  
### Francisco Javier Godinez Lopez:
Esta práctica brindó la descubrimiento de familiarizarnos con algunas de las herramientas que ofrece el programa Epson RC+, permitiendo averiguar nuevas formas de programación para la automatización del brazo robotico utilizado en el curso, de este modo aplicamos los comandos ON, GO y OFF, los cuales son necesarios para realizar movimientos y tareas en el brazo mecánico. Esto permitió comprender de mejor manera las capacidades de control, precisión del brazo y su movimiento.


### Pablo Axel Silva Fuentes: 
 De primera instancia esta práctica se logró aprender una característica importante del software, lo que posibilitó adquirir conocimientos adicionales sobre programación, así como llevar a cabo movimientos precisos con el brazo robótico. El uso correcto de los comandos ON, GO y OFF fue necesario para completar la tarea de trasladar un objeto a una ubicación precisa, resaltando las habilidades del sistema en cuanto a exactitud y manejo.

### Eduardo David Salas Ayala: 
El desarrollo de esta practica permitio conocer una de las tantas herramientas que nos brinda del software Epson RC+, permitiendo cononocer nuevas secciones de programación y la ejecución de movimientos tanto en el simulador como en el brazo físico. El conocimiento de comandos básicos como ON, GO y OFF, junto con su correcta implementación, permitió cumplir eficazmente el objetivo de tomar un objeto y trasladarlo a otro punto, lo que ayudó a comprender mejor las capacidades de movimiento y precisión del brazo robótico.

## Referencias bibliográficas
- Localización y planificación de trayectorias - TEKNIKER. (s. f.). https://www.tekniker.es/es/localizacion-y-planificacion-de-trayectorias

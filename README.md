# Simulación de Aspiradora Inteligente en NetLogo

## Descripción

Este proyecto es una simulación de una aspiradora robótica en un entorno de cuadrícula, implementado en NetLogo. La aspiradora se mueve de manera ortogonal (arriba, abajo, izquierda y derecha) buscando y limpiando basura en el ambiente mientras su batería lo permita.

## Características

- La cuadrícula representa el ambiente, donde cada celda (patch) puede estar limpia o contener basura.
- La aspiradora comienza con una cantidad fija de batería y la consume tanto al moverse como al limpiar.
- Se utiliza una etiqueta sobre la aspiradora para mostrar el estado de la batería.
- Los parches cambian de color para representar su estado (blanco para limpio, marrón para sucio).
- El modelo se ejecuta en tics, reduciendo la batería y permitiendo el movimiento de la aspiradora.

## Instrucciones de Uso

1. Abrir NetLogo e importar el código en el editor.
2. Presionar el botón **Setup** para inicializar el mundo.
3. Presionar el botón **Go** para comenzar la simulación.
4. Crear un input de M y N para poder actualizar el tamaño del ambiente.
5. Observar el comportamiento de la aspiradora mientras limpia la cuadrícula.

![image](https://github.com/user-attachments/assets/42db1d1d-f1b5-40f6-b458-cd689331d7b0)


## Explicación del Código

### Propiedades:

- `turtles-own [status battery]`: Define el estado y la cantidad de batería de la aspiradora.
- `patches-own [dirty]`: Indica si un parche está sucio (1) o limpio (0).

### Procedimientos Clave:

- `setup`: Inicializa el mundo, genera la basura y coloca la aspiradora con batería.
- `go`: Controla el comportamiento de la aspiradora en cada tic.
- `move-orthogonal`: Define el movimiento en las cuatro direcciones cardinales.
- `recolor`: Actualiza el color de los parches según su estado.
- `update-label`: Muestra la cantidad de batería sobre la aspiradora.



## Requisitos

- NetLogo instalado en el sistema.
- Netlogo Web

Este proyecto es ideal para experimentar con conceptos de simulación, inteligencia artificial básica y optimización de rutas en entornos dinámicos.


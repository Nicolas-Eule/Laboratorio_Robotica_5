<!-- ✦✦✦ FUTURE IS AUTOMATED ✦✦✦ -->

<div align="center">

<!-- Banner superior "neón" -->
<img src="https://capsule-render.vercel.app/api?type=waving&height=200&color=0:04041A,50:14213D,100:0A4D68&text=Laboratorio%205&fontColor=E0FBFC&fontSize=60&fontAlign=50&fontAlignY=35&desc=Pincher%20Phantom%20X100%20•%20ROS%20Humble%20•%20RVIZ%20•%20Control%20y%20Conexión%20con%20Python&descSize=20&descAlign=50&descAlignY=55" width="100%" />

<br/>

# 🤖 LABORATORIO 5 – PINCHER PHANTOM X100 - ROS HUMBLE - RVIZ

<br/>

![ROS 2 Humble](https://img.shields.io/badge/ROS%202-Humble-blue?style=for-the-badge)
![Dynamixel AX-12](https://img.shields.io/badge/Dynamixel%20AX-12-green?style=for-the-badge)
![Phantom X-100](https://img.shields.io/badge/Phantom%20X-100-red?style=for-the-badge)

<br/>

<!-- Línea de texto mecanografiado (animado) -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&pause=1200&duration=3500&color=00E5FF&center=true&vCenter=true&width=1000&lines=Pincher+Phantom+X100+%E2%80%A2+ROS+2+Humble+%E2%80%A2+RVIZ;Control+de+Articulaciones+%E2%80%A2+Servicios+%E2%80%A2+Conexi%C3%B3n+con+Python" alt="typing">
</p>


---

### 🛰️ Descripción general

Este repositorio implementa el **Laboratorio No. 5** de *Robótica 2025-II*: control y conexión del robot **Phantom X100** utilizando **ROS 2 Humble** y **RVIZ**.  
Se incluyen tópicos de movimiento para las articulaciones, la conexión con los servomotores Dynamixel AX-12, y el control mediante Python para manipular el robot en RVIZ.

---

## 🧑‍🚀 Equipo

<!-- ===== INICIO BLOQUE ANIMACIONES EQUIPO (una animación por línea) ===== -->

<!-- Encabezado: Integrantes -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=800&size=22&duration=2000&pause=800&color=00E5FF&center=true&vCenter=true&width=1000&repeat=true&v=1&lines=Integrantes%3A" alt="Integrantes">
</p>

<!-- Nombre 1 -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=20&duration=2400&pause=600&color=7F5AF0&center=true&vCenter=true&width=1000&repeat=true&v=1&lines=Jorge+Nicol%C3%A1s+Garz%C3%B3n+Acevedo+%E2%80%94+jngarzona%40unal.du.co" alt="Jorge Nicolás Garzón Acevedo">
</p>

<!-- Nombre 2 -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=20&duration=2400&pause=600&color=7F5AF0&center=true&vCenter=true&width=1000&repeat=true&v=1&lines=Johan+Camilo+Pati%C3%B1o+Mogoll%C3%B3n+%E2%80%94+jopatinom%40unal.edu.co" alt="Johan Camilo Patiño Mogollón">
</p>

<!-- Nombre 3 -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=20&duration=2400&pause=600&color=7F5AF0&center=true&vCenter=true&width=1000&repeat=true&v=1&lines=Gabriel+Eduardo+Bojaca+Munar+%E2%80%94+gbojaca%40unal.edu.co" alt="Gabriel Eduardo Bojaca Munar">
</p>

<!-- Encabezado: Docentes -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=800&size=22&duration=2000&pause=800&color=00E5FF&center=true&vCenter=true&width=1000&repeat=true&v=1&lines=Docentes%3A" alt="Docentes">
</p>

<!-- Docente 1 -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=20&duration=2400&pause=600&color=39D353&center=true&vCenter=true&width=1000&repeat=true&v=1&lines=Manuel+Felipe+Carranza+Montenegro+%E2%80%94+mcarranza%40unal.edu.co" alt="Manuel Felipe Carranza Montenegro">
</p>

<!-- Docente 2 -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=20&duration=2400&pause=600&color=39D353&center=true&vCenter=true&width=1000&repeat=true&v=1&lines=Pedro+Fabi%C3%A1n+C%C3%A1rdenas+Herrera+%E2%80%94+pfcardenash%40unal.edu.co" alt="Pedro Fabián Cárdenas Herrera">
</p>

<!-- ===== FIN BLOQUE ANIMACIONES EQUIPO ===== -->

</div>

---

# Laboratorio 5 - Pincher Phantom X100 - ROS Humble - RVIZ

## Objetivos del laboratorio

1. **Crear todos los Joint Controllers** con ROS para manipular servomotores Dynamixel AX-12 del robot Phantom X Pincher.
2. **Manipular los tópicos de estado y comando** para todos los Joint Controllers del robot, entendiendo la diferencia entre:
   - Tópicos de *estado* (lectura de posición, velocidad, corriente, etc.).
   - Tópicos de *comando* (referencias de posición/velocidad para cada articulación).
3. **Manipular servicios ROS 2** asociados a los Joint Controllers (por ejemplo, habilitar/deshabilitar torque, reiniciar controladores o mover a la posición *home*).
4. **Conectar el robot Phantom X Pincher con Python usando ROS 2**, de forma que:
   - Pueda enviarse una configuración articular desde Python al robot.
   - Se reciba el estado articular para validación y visualización.
   - Se integre con herramientas de modelado (toolbox) para graficar la configuración.

## Requisitos
- Ubuntu versión 22.xx preferible 22.04 LTS con ROS Humble.
- Espacio de trabajo para `colcon build` correctamente configurado.
- Paquetes de Dynamixel Workbench: [Dynamixel Workbench GitHub](https://github.com/labsir-un/ROB_Intro_ROS2_Humble_Phantom_Pincher_X100.git)
- Paquete del robot Phantom X: [Phantom X GitHub](https://github.com/labsir-un/ROB_Intro_ROS2_Humble_Phantom_Pincher_X100_RVIZ.git)
- Python.
- Un manipulador Phantom X Pincher con su entorno de trabajo.

## Desarrollo del ejercicio en el laboratorio

### Mediciones

Se determinaron las longitudes de eslabón de cada articulación del robot Phantom X Pincher utilizando un calibrador digital. Para ello se definieron referencias fijas en la base y en cada junta, y se registraron las distancias entre ejes consecutivos. Con estos datos se elaboró un diagrama esquemático del manipulador, análogo al presentado en la Figura 2 de la guía, donde se consignaron los nombres de los eslabones y sus dimensiones efectivas.

### Análisis

A partir de las dimensiones medidas se construyó la tabla de parámetros Denavit–Hartenberg (DH) del Phantom X Pincher. Para cada junta se establecieron los parámetros \(a_i\), \(\alpha_i\), \(d_i\) y \(\theta_i\) en coherencia con la asignación de marcos de referencia utilizada en el modelo de simulación. Con esta información se generó un diagrama del robot que incluye la tabla DH y los sistemas de coordenadas por junta, verificando la compatibilidad con el modelo cinemático usado posteriormente en los paquetes de descripción y control.

### Implementación en ROS 2

Siguiendo la estructura de los paquetes de control para PhantomX en ROS 2, se trabajó sobre un workspace tipo `phantom_ws` en el que se creó y configuró el paquete de control en Python para el robot. Dentro de este paquete se desarrolló un nodo ROS 2 que:

1. Inicializa la comunicación con los servomotores Dynamixel AX-12 a través del puerto serie configurado para el bus del robot.
2. Publica los comandos de posición para cada articulación (waist, shoulder, elbow, wrist y gripper) usando los tópicos de control definidos en el workspace.
3. Ejecuta una secuencia de movimiento entre dos configuraciones articulares características: una configuración de **home** y una configuración **objetivo**.
4. Realiza el movimiento de forma secuencial, comenzando por la articulación de la base y continuando hacia las articulaciones distales, insertando pausas breves entre cada cambio articular para asegurar una transición suave y claramente observable.

Esta lógica se integró con el paquete de descripción del robot, de manera que la misma información articular que se envía al manipulador se utiliza también para actualizar la visualización en RViz a través del tópico `/joint_states`.

### Conexión con Python

Además del nodo principal de control, se desarrollaron scripts en Python que interactúan directamente con los tópicos y servicios de ROS 2:

- Un script publica en los tópicos de comando de cada controlador de articulación, recibiendo como entrada un conjunto de ángulos articulares en grados. Previo al envío, se realiza la validación de límites para cada junta, saturando o rechazando valores que excedan los rangos permitidos por los servomotores.
- Un segundo script se suscribe a los tópicos de estado de los controladores, recupera las posiciones articulares actuales, las convierte a grados y retorna la configuración resultante de 5 ángulos. Estas lecturas se usan tanto para depuración como para la actualización de la HMI y para comparar el estado real con la simulación.

### Python + ROS + Toolbox

Se implementó un código adicional en Python que integra ROS 2 con un toolbox de robótica para la representación del manipulador. Este script:

1. Utiliza la tabla DH obtenida en la sección de análisis para construir el modelo cinemático del Phantom X Pincher.
2. Recibe como entrada un vector articular \([q_1, q_2, q_3, q_4, q_5]\) (en grados o radianes, según la configuración).
3. Grafica la configuración del robot en un entorno 3D utilizando las herramientas del toolbox, mostrando la posición y orientación del TCP.
4. Sincroniza esta representación con los valores articulares leídos desde ROS 2, de modo que la pose digital coincida con la pose del robot real.

Los modelos 3D del robot (mallas `.stl` de base, hombro, brazo, antebrazo y gripper) se integraron en el paquete de descripción para que la visualización en RViz y la del toolbox representen fielmente el hardware utilizado en el laboratorio.

### Poses de prueba

Durante la práctica se ensayaron múltiples configuraciones articulares para validar tanto el modelo como la interfaz de control. En particular, se comprobaron las siguientes poses generadas a partir de los valores \((q_1, q_2, q_3, q_4, q_5)\) en grados:

1. \(0, 0, 0, 0, 0\)
2. \(25, 25, 20, -20, 0\)
3. \(-35, 35, -30, 30, 0\)
4. \(85, -20, 55, 25, 0\)
5. \(80, -35, 55, -45, 0\)

Para cada caso se verificó que los ángulos se mantuvieran dentro de los límites articulares definidos por los servomotores y que el movimiento no generara colisiones con la mesa de trabajo ni con otros elementos del entorno.

### Interfaz de Usuario (HMI)

Se desarrolló una interfaz gráfica (HMI) en Python que centraliza las principales funciones de operación del manipulador y su visualización. La HMI incluye:

1. Un panel de identificación con los nombres, logos y datos de contacto de los integrantes del grupo.
2. Un área donde se muestra la imagen o captura de la perspectiva de la última posición enviada al manipulador, tomada ya sea de la simulación o de fotografías del robot real.
3. Controles para seleccionar cualquiera de las cinco poses predefinidas y enviarlas al robot con un solo clic.
4. Un bloque de lectura numérica que presenta en tiempo real los valores articulares actuales de cada motor, a partir de los tópicos de estado.
5. Una segunda imagen que refleja la posición actual del manipulador asociada a los valores articulares medidos, permitiendo comparar inmediatamente la referencia enviada con la posición realmente alcanzada.

### Funcionalidades de la interfaz gráfica

La interfaz se organizó en varias pestañas, cada una enfocada en un modo de operación específico:

- **Pestaña de control en espacio articular**: Se incluyeron deslizadores (sliders) para cada articulación, configurados con los límites mínimos y máximos permitidos. Al modificar un slider, la HMI actualiza el valor numérico correspondiente y envía el comando articular a través del nodo de control, actualizando en paralelo la visualización del robot.

- **Pestaña de ingreso numérico articular**: Se habilitaron campos de entrada para que el operador pueda escribir directamente los valores de \(q_1\) a \(q_5\) en grados. Antes de publicar el comando, la aplicación verifica que los valores se encuentren dentro de los rangos válidos; en caso contrario, informa el error o ajusta el valor al límite más cercano.

- **Pestaña de control en el espacio de la tarea**: Se implementaron controles para manipular el TCP del robot en coordenadas cartesiano-orientacionales (X, Y, Z y ángulos RPY). La HMI calcula la configuración articular mediante la cinemática inversa y, si la solución es alcanzable y segura, envía la nueva configuración al manipulador y a la visualización.

- **Pestaña de visualización en RViz**: Desde esta pestaña se puede lanzar y cerrar RViz directamente desde la interfaz, utilizando el archivo de lanzamiento del paquete de descripción. El modelo del Phantom X Pincher se actualiza en tiempo real con los valores publicados en `/joint_states`, de manera que el movimiento del robot físico se refleja inmediatamente en la escena 3D.

- **Pestaña de visualización numérica de la pose cartesiana**: Finalmente, se dispuso un panel donde se muestra en tiempo real la posición \(X, Y, Z\) y la orientación en términos de Roll–Pitch–Yaw del TCP del robot. Estos valores se calculan a partir del modelo cinemático y permiten validar cuantitativamente la pose alcanzada tanto en el espacio de la tarea como en la simulación.


## Entregables
1. Descripción detallada de la solución planteada.
2. Diagrama de flujo de acciones del robot utilizando la herramienta Mermaid.
3. Plano de planta de la ubicación de cada uno de los elementos.
4. Descripción de las funciones utilizadas.
5. Código del script utilizado para el desarrollo de la práctica.


---

## Video de simulación y entorno físico

Video donde se evidencia la simulación en RViz y el comportamiento del robot en el entorno físico (poses y uso de la interfaz gráfica):

[![Video de simulación y entorno físico](https://img.youtube.com/vi/65TIC8xtnyM/0.jpg)](https://youtu.be/65TIC8xtnyM)


---

## Requisitos de software y hardware

- **Sistema operativo:** Ubuntu 22.xx (preferiblemente **22.04 LTS**) con **ROS 2 Humble** instalado.
- **Espacio de trabajo ROS 2** configurado para compilar con `colcon build`.
- **Paquetes de Dynamixel Workbench:**
6. Video del brazo alcanzando cada posición solicitada.
7. Video demostración de uso de la interfaz de usuario.
8. Gráfica digital de las poses comparándola con la fotografía del brazo real en la misma configuración.



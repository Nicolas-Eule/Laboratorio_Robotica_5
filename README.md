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

### Configuración del entorno (Setup)
La preparación del entorno de trabajo se realizó siguiendo la guía **`guias/Setup`** del repositorio:

- [`ROB_Intro_ROS2_Humble_Phantom_Pincher_X100_Updated/jazzy/guias/Setup`](https://github.com/ElJoho/ROB_Intro_ROS2_Humble_Phantom_Pincher_X100_Updated/tree/jazzy/guias/Setup)

En particular:

1. Se creó un workspace ROS 2 dedicado para el Phantom X Pincher (tipo `phantom_ws`) y dentro de este se ubicaron los paquetes del kit Phantom (control, descripción y utilidades).
2. Se instalaron las dependencias del proyecto y se compiló el workspace con `colcon build`, dejando el entorno accesible mediante los scripts de `setup.bash`.
3. Se verificó la conexión del manipulador real a través del adaptador USB2Dynamixel (`/dev/ttyUSBx`) y la configuración de los IDs de los servomotores, de modo que el entorno de desarrollo quedara alineado con la configuración de hardware utilizada en el laboratorio.

Esta fase dejó listos los paquetes de control y descripción sobre los que se construyó el resto de la práctica.

### Implementación en ROS 2 y MoveIt
Tomando como base el entorno anterior y la guía **`guias/Moveit`** del mismo repositorio:

- [`ROB_Intro_ROS2_Humble_Phantom_Pincher_X100_Updated/jazzy/guias/Moveit`](https://github.com/ElJoho/ROB_Intro_ROS2_Humble_Phantom_Pincher_X100_Updated/tree/jazzy/guias/Moveit)

se completó la integración de control articular y planificación de movimiento:

1. Se configuró el modelo del Phantom X Pincher en RViz2 mediante un paquete de descripción con archivos `xacro/URDF` y mallas `.stl`, de forma análoga a la estructura propuesta en las guías del kit.
2. Se añadió la configuración de **MoveIt 2** para el robot, definiendo el grupo de planificación del manipulador y las articulaciones relevantes, de modo que la interfaz *Motion Planning* de RViz2 pudiera planear trayectorias sobre el modelo del Phantom.
3. Sobre el workspace `phantom_ws` se desarrolló un nodo ROS 2 de control en Python que:
   - Inicializa la comunicación con los servomotores Dynamixel AX-12/XL-430.
   - Publica comandos de posición para cada articulación (waist, shoulder, elbow, wrist y gripper) usando los tópicos de control definidos.
   - Actualiza el estado articular en `/joint_states`, permitiendo que RViz2 y MoveIt reflejen en tiempo real la configuración del manipulador.
4. Se implementó una secuencia de movimiento entre dos configuraciones características (home y objetivo). El movimiento se realiza de forma secuencial, comenzando por la base y continuando hacia las articulaciones distales, con pausas breves entre articulaciones para facilitar la observación y evitar movimientos bruscos.
5. Desde la interfaz de MoveIt 2 en RViz2 se planearon y ejecutaron trayectorias hacia las configuraciones de prueba, comprobando tanto la viabilidad cinemática como la ausencia de colisiones en el entorno definido.

De esta manera, el mismo conjunto de valores articulares se utiliza simultáneamente en el controlador del robot, en la planificación de movimiento de MoveIt 2 y en la visualización en RViz2.

### Conexión con Python
Además del nodo de control principal, se desarrollaron scripts en Python que interactúan directamente con los tópicos y servicios de ROS 2:

- Un script publica en los tópicos de comando de cada controlador de articulación a partir de un conjunto de ángulos articulares en grados. Antes de enviar los comandos, se validan los límites de cada junta y se saturan o rechazan valores que excedan los rangos permitidos por los servomotores.
- Un segundo script se suscribe a los tópicos de estado de los controladores, recupera las posiciones articulares actuales, las convierte a grados y retorna la configuración resultante de 5 ángulos. Estas lecturas se utilizan tanto para depuración como para alimentar la HMI y para comparar el estado real con la simulación/planeación en MoveIt 2.

### Python + ROS + Toolbox
Se implementó un código adicional en Python que integra ROS 2 con un toolbox de robótica para la representación del manipulador. Este script:

1. Utiliza la tabla DH obtenida en la sección de análisis para construir el modelo cinemático del Phantom X Pincher.
2. Recibe como entrada un vector articular \([q_1, q_2, q_3, q_4, q_5]\) (en grados o radianes, según la configuración) y lo transforma a la convención utilizada por el toolbox.
3. Grafica la configuración del robot en un entorno 3D, mostrando la posición y orientación del TCP y permitiendo comparar visualmente la pose obtenida con la que se observa en RViz2 y en el robot real.
4. Sincroniza esta representación con los valores articulares leídos desde ROS 2, de modo que la pose digital (toolbox/MoveIt/RViz2) coincida con la pose del manipulador físico.

### Poses de prueba
Durante la práctica se ensayaron múltiples configuraciones articulares para validar tanto el modelo como la interfaz de control y la configuración de MoveIt 2. En particular, se comprobaron las siguientes poses generadas a partir de los valores \((q_1, q_2, q_3, q_4, q_5)\) en grados:

1. \(0, 0, 0, 0, 0\)
2. \(25, 25, 20, -20, 0\)
3. \(-35, 35, -30, 30, 0\)
4. \(85, -20, 55, 25, 0\)
5. \(80, -35, 55, -45, 0\)

Para cada caso se verificó que los ángulos se mantuvieran dentro de los límites articulares definidos por los servomotores, que las trayectorias propuestas por MoveIt 2 fueran libres de colisión y que el movimiento no generara interferencias con la mesa de trabajo ni con otros elementos del entorno.

### Interfaz de Usuario (HMI)
Se desarrolló una interfaz gráfica (HMI) en Python que centraliza las principales funciones de operación del manipulador, la visualización y la interacción con MoveIt 2. La HMI incluye:

1. Un panel de identificación con los nombres, logos y datos de contacto de los integrantes del grupo.
2. Un área donde se muestra la imagen o captura de la perspectiva de la última posición enviada al manipulador, tomada ya sea de la simulación (RViz2/MoveIt) o de fotografías del robot real.
3. Controles para seleccionar cualquiera de las cinco poses predefinidas y enviarlas al robot con un solo clic, reutilizando los mismos vectores articulares empleados en la planificación de MoveIt 2.
4. Un bloque de lectura numérica que presenta en tiempo real los valores articulares actuales de cada motor, a partir de los tópicos de estado.
5. Una segunda imagen que refleja la posición actual del manipulador asociada a los valores articulares medidos, permitiendo comparar inmediatamente la referencia enviada con la posición realmente alcanzada.

### Funcionalidades de la interfaz gráfica
La interfaz se organizó en varias pestañas, cada una enfocada en un modo de operación específico:

- **Pestaña de control en espacio articular**: Se incluyeron deslizadores (sliders) para cada articulación, configurados con los límites mínimos y máximos permitidos. Al modificar un slider, la HMI actualiza el valor numérico correspondiente y envía el comando articular a través del nodo de control, actualizando en paralelo la visualización del robot (RViz2 / MoveIt).
- **Pestaña de ingreso numérico articular**: Se habilitaron campos de entrada para que el operador pueda escribir directamente los valores de \(q_1\) a \(q_5\) en grados. Antes de publicar el comando, la aplicación verifica que los valores se encuentren dentro de los rangos válidos; en caso contrario, informa el error o ajusta el valor al límite más cercano.
- **Pestaña de control en el espacio de la tarea**: Se implementaron controles para manipular el TCP del robot en coordenadas cartesiano-orientacionales (X, Y, Z y ángulos RPY). La HMI calcula la configuración articular mediante la cinemática inversa y, si la solución es alcanzable y segura, envía la nueva configuración al manipulador y a la visualización.
- **Pestaña de visualización en RViz/MoveIt**: Desde esta pestaña se puede lanzar y cerrar RViz2 y la escena de MoveIt directamente desde la interfaz, utilizando los archivos de lanzamiento del paquete de descripción/configuración. El modelo del Phantom X Pincher se actualiza en tiempo real con los valores publicados en `/joint_states`, de manera que el movimiento del robot físico se refleja inmediatamente en la escena 3D y en la planificación.
- **Pestaña de visualización numérica de la pose cartesiana**: Finalmente, se dispuso un panel donde se muestra en tiempo real la posición \(X, Y, Z\) y la orientación en términos de Roll–Pitch–Yaw del TCP del robot. Estos valores se calculan a partir del modelo cinemático y de la solución utilizada por MoveIt 2, permitiendo validar cuantitativamente la pose alcanzada tanto en el espacio de la tarea como en la simulación.



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



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
Se determinaron las longitudes de eslabón de cada articulación del robot Phantom X Pincher utilizando un calibrador digital. Para ello se definieron referencias fijas en la base y en cada junta y se registraron las distancias entre ejes consecutivos. Con estos datos se elaboró un diagrama esquemático del manipulador —análogo al presentado en la Figura 2 de la guía— donde se consignaron los nombres de los eslabones y sus dimensiones efectivas.

### Análisis
A partir de las dimensiones medidas se construyó la tabla de parámetros Denavit–Hartenberg (DH) del Phantom X Pincher. Para cada junta se establecieron los parámetros \(a_i\), \(\alpha_i\), \(d_i\) y \(\theta_i\) en coherencia con la asignación de marcos de referencia utilizada en el modelo de simulación. Con esta información se generó un diagrama del robot que incluye la tabla DH y los sistemas de coordenadas por junta, verificando la compatibilidad con el modelo cinemático usado posteriormente en los paquetes de descripción y control.

### Organización del repositorio y workspace `phantom_ws`

Todo el desarrollo software del proyecto se consolidó en el repositorio:

- [`sergiosinlimites/robotica-proyecto-final`](https://github.com/sergiosinlimites/robotica-proyecto-final)

Dentro de este repositorio se organizó un workspace ROS 2 dedicado al Phantom X Pincher:

- Workspace: `phantom_ws`
- Código fuente: `phantom_ws/src`

En `phantom_ws/src` se alojaron los paquetes de ROS 2 desarrollados en la práctica, agrupando:

- Paquetes de **descripción** del robot (modelo URDF/XACRO y mallas).
- Paquetes de **control articular** y conexión con los servomotores Dynamixel.
- Paquetes para la **integración con RViz / MoveIt**.
- Paquetes para la **interfaz gráfica (HMI)** y los scripts de pruebas de laboratorio.

De esta forma, el repositorio `robotica-proyecto-final` quedó como contenedor único de la configuración del entorno, los nodos ROS 2, los archivos de lanzamiento y las herramientas utilizadas en el laboratorio, facilitando la compilación con `colcon` y la reutilización del código en futuras prácticas.

### Configuración del entorno (Setup)

La preparación del entorno de trabajo se realizó siguiendo las guías del kit Phantom X Pincher y se volcó en el workspace `phantom_ws` del repositorio `robotica-proyecto-final`:

1. Se creó el workspace ROS 2 `phantom_ws` y, dentro de `src`, se clonaron y/o copiaron los paquetes base del kit Phantom (descripción del robot, control de Dynamixel, paquetes de RViz y de MoveIt).
2. Se instalaron las dependencias del proyecto y se compiló el workspace con `colcon build`, dejando el entorno accesible mediante los scripts de `install/setup.bash`.
3. Se verificó la conexión del manipulador real a través del adaptador USB2Dynamixel (`/dev/ttyUSBx`), ajustando la velocidad de comunicación y los IDs de los servomotores para que coincidieran con la configuración esperada por los nodos de control.
4. Se añadieron scripts de utilidad (dentro de `phantom_ws/src`) para automatizar el lanzamiento de RViz, MoveIt y la HMI, de modo que toda la práctica pudiera reproducirse a partir del mismo workspace.

Esta etapa dejó listos los paquetes de control, simulación y la estructura del repositorio sobre la cual se construyó el resto de la práctica.

### Implementación en ROS 2 y MoveIt

Sobre el workspace `phantom_ws/src` se desarrollaron y ajustaron los paquetes encargados de la simulación y planificación de movimientos:

1. **Descripción del robot y RViz**  
   - Se configuró el modelo del Phantom X Pincher mediante archivos `URDF/XACRO` y mallas 3D, ubicados en los paquetes de descripción del workspace.
   - Se creó un archivo de lanzamiento para RViz2 que carga el modelo del robot, la configuración de visualización y la fuente de `joint_states`, permitiendo ver el manipulador en 3D desde el inicio.

2. **Configuración de MoveIt 2**  
   - Se añadió la configuración de MoveIt 2 para el manipulador, definiendo el grupo de planificación, las articulaciones y el *end effector*.
   - Se configuró la escena de planificación en RViz2 (grupo de planificación, límites articulares y escenas de colisión) para probar poses y trayectorias antes de ejecutarlas en el robot real.

3. **Nodos de control en ROS 2**  
   En los paquetes de control alojados en `phantom_ws/src` se implementó un nodo (o conjunto de nodos) en Python/ROS 2 que:
   - Inicializa la comunicación con los servomotores Dynamixel del Phantom X Pincher.
   - Publica comandos de posición para cada articulación (`waist`, `shoulder`, `elbow`, `wrist` y `gripper`) a través de los tópicos de control.
   - Actualiza el estado de las juntas en `/joint_states`, garantizando la sincronización entre el robot real, RViz2 y MoveIt 2.

4. **Secuencias de movimiento**  
   - Se programó una rutina que ejecuta el movimiento entre una postura de *home* y diferentes posturas objetivo.
   - El movimiento se realiza de forma secuencial, iniciando en la base y avanzando hacia las articulaciones distales, con pequeñas pausas entre cada junta para facilitar la observación y reducir movimientos bruscos.
   - Desde la interfaz de MoveIt 2 se probaron trayectorias planificadas hacia las poses de prueba, validando la cinemática y evitando colisiones.

Con esta implementación, el mismo conjunto de valores articulares se reutilizó en el controlador del robot, en las trayectorias de MoveIt 2 y en la visualización de RViz2, todo gestionado desde el workspace `phantom_ws`.

### Conexión con Python

Además de los nodos de control estándar, se desarrollaron scripts específicos en Python —ubicados también dentro de `phantom_ws/src`— para interactuar directamente con los tópicos y servicios de ROS 2:

- Un script publica en los tópicos de comando de cada controlador articular a partir de vectores de ángulos en grados. Antes de publicar, se validan los límites de cada junta; valores fuera del rango se saturan o se descartan, evitando comandos inválidos sobre los Dynamixel.
- Un segundo script se suscribe a los tópicos de estado de los controladores y/o a `/joint_states`, transforma las posiciones a grados y entrega la configuración articular de 5 ángulos. Esta información se aprovechó para:
  - Depurar el comportamiento de los controladores.
  - Alimentar la HMI con la lectura en tiempo real de las juntas.
  - Comparar los valores medidos en el robot real frente a los valores usados en simulación (RViz2/MoveIt).

Ambos scripts se integraron al árbol de paquetes del workspace, de forma que pueden ejecutarse mediante `ros2 run` desde el propio repositorio del proyecto final.

### Python + ROS + Toolbox

Se añadió un módulo en Python que conecta ROS 2 con un toolbox de robótica (entorno de cálculo) para representar el manipulador a partir de la tabla DH:

1. Se utilizó la tabla DH obtenida en la sección de análisis para construir el modelo cinemático directo del Phantom X Pincher.
2. El script recibe como entrada un vector \([q_1, q_2, q_3, q_4, q_5]\), en grados o radianes, y lo adapta a la convención del toolbox (offsets y signos).
3. A partir de este vector, el modelo calcula la pose cartesiana del TCP (posición y orientación) y genera una gráfica 3D de la configuración del robot.
4. La representación en el toolbox se sincronizó con los valores articulares que llegan desde ROS 2, permitiendo comparar:
   - La pose digital en el toolbox.
   - La pose mostrada en RViz2/MoveIt.
   - La pose físicamente alcanzada por el Phantom X Pincher.

Este módulo se integró al repositorio como parte del flujo de verificación de la solución.

### Poses de prueba

Durante la práctica se ensayaron múltiples configuraciones articulares para validar tanto el modelo como la interfaz de control y la configuración de MoveIt 2. En particular, se comprobaron las siguientes poses generadas a partir de los valores \((q_1, q_2, q_3, q_4, q_5)\) en grados:

1. \(0, 0, 0, 0, 0\)
2. \(25, 25, 20, -20, 0\)
3. \(-35, 35, -30, 30, 0\)
4. \(85, -20, 55, 25, 0\)
5. \(80, -35, 55, -45, 0\)

Para cada caso se verificó que los ángulos se mantuvieran dentro de los límites articulares definidos por los servomotores, que las trayectorias propuestas por MoveIt 2 fueran libres de colisión y que el movimiento no generara interferencias con la mesa de trabajo ni con otros elementos del entorno.

### Interfaz de Usuario (HMI)

Como parte del proyecto final se desarrolló una interfaz gráfica (HMI) en Python, incluida dentro del workspace `phantom_ws/src`, que centraliza las principales funciones de operación del manipulador, la visualización y la interacción con MoveIt 2:

1. **Identificación del grupo**  
   Se preparó un panel con los nombres, logos y datos de contacto de los integrantes del grupo, visible al iniciar la aplicación.
2. **Visualización de la última posición enviada**  
   La HMI muestra una imagen o captura asociada a la última configuración enviada al manipulador (tanto de la simulación como del robot real), facilitando la documentación de resultados.
3. **Selección de poses predefinidas**  
   Se incorporaron botones para seleccionar cualquiera de las cinco poses de prueba y enviarlas al robot con un solo clic, reutilizando los mismos vectores articulares empleados en los scripts de ROS 2 y en MoveIt 2.
4. **Lectura de ángulos articulares**  
   Se despliega en tiempo real el valor actual de cada ángulo articular, a partir de las lecturas de los tópicos de estado y/o `/joint_states`.
5. **Visualización de la posición actual**  
   Se presenta una segunda imagen o panel asociado a la pose actual del manipulador, permitiendo comparar instantáneamente la referencia enviada con la posición realmente alcanzada.

### Funcionalidades de la interfaz gráfica

La interfaz se organizó en varias pestañas, cada una enfocada en un modo de operación específico:

- **Pestaña de control en espacio articular**  
  Incluye deslizadores para cada articulación, configurados con los límites mínimos y máximos permitidos. Al modificar un slider, la HMI:
  1. Actualiza el valor numérico correspondiente.
  2. Publica el comando articular hacia el nodo de control.
  3. Fuerza la actualización de la visualización del robot en RViz2/MoveIt y en la vista de la HMI.

- **Pestaña de ingreso numérico articular**  
  Permite al operador introducir directamente los valores de \(q_1\) a \(q_5\) en grados mediante campos de texto. Antes de enviar el comando:
  1. Se verifican los rangos de cada junta.
  2. En caso de error, se notifica al usuario o se ajusta el valor al límite más cercano.
  3. Se actualizan de forma coherente la visualización del robot y los valores numéricos mostrados.

- **Pestaña de control en el espacio de la tarea**  
  Ofrece controles para manipular el TCP del robot en coordenadas \(X, Y, Z\) y orientación RPY. La HMI:
  1. Calcula la cinemática inversa para obtener una solución articular.
  2. Comprueba la alcanzabilidad y el cumplimiento de límites.
  3. Publica la nueva configuración articular en ROS 2 y actualiza la simulación.

- **Pestaña de visualización en RViz/MoveIt**  
  Desde esta pestaña se lanzan o detienen RViz2 y la escena de MoveIt utilizando los archivos de lanzamiento del workspace. El modelo del Phantom X Pincher se actualiza con los valores publicados en `/joint_states`, de modo que el movimiento del robot físico se refleja inmediatamente en la escena 3D.

- **Pestaña de visualización numérica de la pose cartesiana**  
  Presenta en tiempo real la posición \(X, Y, Z\) y la orientación en términos de Roll–Pitch–Yaw del TCP del robot. Estos valores se obtienen a partir del modelo cinemático y de la configuración actual de las articulaciones, permitiendo una validación cuantitativa de la pose lograda tanto en la simulación como en el robot real.



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



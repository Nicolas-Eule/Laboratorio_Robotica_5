<!-- ✦✦✦ FUTURE IS AUTOMATED ✦✦✦ -->
<!-- Banner superior "neón" -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=140&color=0:04041A,50:14213D,100:0A4D68&text=Laboratorio%205%20-%20Pincher%20Phantom%20X100%20-%20ROS%20Humble%20-%20RVIZ&fontColor=E0FBFC&fontAlign=50&fontAlignY=30&desc=Control%20y%20Conexi%C3%B3n%20con%20Python&descAlign=50&descAlignY=60" alt="header" style="width: 100%; height: auto; max-width: 100%; display: block;" />
</p>

<h1 align="center">🤖 LABORATORIO 5 – PINCHER PHANTOM X100 - ROS HUMBLE - RVIZ</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Ros%202-Humble-blue?style=for-the-badge" alt="ROS 2 Humble" style="display: inline-block; margin: 5px;" />
  <img src="https://img.shields.io/badge/Dynamixel%20AX-12-green?style=for-the-badge" alt="Dynamixel AX-12" style="display: inline-block; margin: 5px;" />
  <img src="https://img.shields.io/badge/Phantom%20X-100-red?style=for-the-badge" alt="Phantom X-100" style="display: inline-block; margin: 5px;" />
</p>

<!-- Línea de texto mecanografiado (animado) -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&pause=1200&duration=3500&color=00E5FF&center=true&vCenter=true&lines=Pincher+Phantom+X100+%E2%80%A2+ROS+2+Humble+%E2%80%A2+RVIZ;Control+de+Articulaciones+%E2%80%A2+Servicios+%E2%80%A2+Conexi%C3%B3n+con+Python" alt="typing" style="width: 100%; max-width: 800px; height: auto; display: block; margin: 0 auto;" />
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
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=800&size=22&duration=2000&pause=800&color=00E5FF&center=true&vCenter=true&width=1000&repeat=true&v=1&lines=Integrantes%3A" alt="Integrantes" style="width: 100%; max-width: 1000px; height: auto; display: block; margin: 10px auto;" />
</p>

<!-- Nombre 1 -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=20&duration=2400&pause=600&color=7F5AF0&center=true&vCenter=true&width=1000&repeat=true&v=1&lines=Nombre%20Integrante%201%20-%20correo%40unal.edu.co" alt="Integrante 1" style="width: 100%; max-width: 1000px; height: auto; display: block; margin: 5px auto;" />
</p>

<!-- Nombre 2 -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=20&duration=2400&pause=600&color=7F5AF0&center=true&vCenter=true&width=1000&repeat=true&v=1&lines=Nombre%20Integrante%202%20-%20correo%40unal.edu.co" alt="Integrante 2" style="width: 100%; max-width: 1000px; height: auto; display: block; margin: 5px auto;" />
</p>

<!-- Nombre 3 -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=20&duration=2400&pause=600&color=7F5AF0&center=true&vCenter=true&width=1000&repeat=true&v=1&lines=Nombre%20Integrante%203%20-%20correo%40unal.edu.co" alt="Integrante 3" style="width: 100%; max-width: 1000px; height: auto; display: block; margin: 5px auto;" />
</p>

<!-- Encabezado: Docentes -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=800&size=22&duration=2000&pause=800&color=00E5FF&center=true&vCenter=true&width=1000&repeat=true&v=1&lines=Docentes%3A" alt="Docentes" style="width: 100%; max-width: 1000px; height: auto; display: block; margin: 10px auto;" />
</p>

<!-- Docente 1 -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=20&duration=2400&pause=600&color=39D353&center=true&vCenter=true&width=1000&repeat=true&v=1&lines=Nombre%20Docente%201%20-%20correo%40unal.edu.co" alt="Docente 1" style="width: 100%; max-width: 1000px; height: auto; display: block; margin: 5px auto;" />
</p>

<!-- Docente 2 -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=20&duration=2400&pause=600&color=39D353&center=true&vCenter=true&width=1000&repeat=true&v=1&lines=Nombre%20Docente%202%20-%20correo%40unal.edu.co" alt="Docente 2" style="width: 100%; max-width: 1000px; height: auto; display: block; margin: 5px auto;" />
</p>

<!-- ===== FIN BLOQUE ANIMACIONES EQUIPO ===== -->


# Laboratorio 5 - Pincher Phantom X100 - ROS Humble - RVIZ

## Objetivos
1. **Crear todos los Joint Controllers** con ROS para manipular servomotores Dynamixel AX-12 del robot Phantom X Pincher.
2. **Manipular los tópicos de estado y comando** para todos los Joint Controllers del robot Phantom X Pincher.
3. **Manipular los servicios** para todos los Joint Controllers del robot Phantom X Pincher.
4. **Conectar el robot Phantom X Pincher con Python usando ROS 2**.

## Requisitos
- Ubuntu versión 22.xx preferible 22.04 LTS con ROS Humble.
- Espacio de trabajo para `colcon build` correctamente configurado.
- Paquetes de Dynamixel Workbench: [Dynamixel Workbench GitHub](https://github.com/labsir-un/ROB_Intro_ROS2_Humble_Phantom_Pincher_X100.git)
- Paquete del robot Phantom X: [Phantom X GitHub](https://github.com/labsir-un/ROB_Intro_ROS2_Humble_Phantom_Pincher_X100_RVIZ.git)
- Python.
- Un (1) manipulador Phantom X Pincher con su entorno de trabajo.

## Ejercicio en el laboratorio
Cada grupo tendrá a cargo un robot Phantom X Pincher. Siga las indicaciones del laboratorista y profesores para hacer buen uso de los robots del laboratorio.

### Mediciones
Establezca las longitudes de eslabón para cada articulación del robot Phantom X Pincher usando un calibrador. Genere un diagrama con los datos medidos, como el ejemplo presentado en la figura 2 de la guía.

### Análisis
Con las dimensiones medidas, obtenga los parámetros DH del robot Phantom X Pincher. Genere un diagrama del robot con las tablas de parámetros articulares utilizando software de ilustración.

### ROS 2
Cree un script en ROS 2 que publique a los tópicos y llame a los servicios correspondientes para realizar el movimiento de cada una de las articulaciones del manipulador (waist, shoulder, elbow, wrist). La lógica del script debe ser la siguiente:
1. Realice el movimiento entre dos posiciones angulares características: una de home y otra objetivo.
2. El movimiento de las articulaciones debe realizarse de forma secuencial, comenzando por la articulación de la base. Agregue una pequeña espera entre cada movimiento.

### Conexión con Python
Cree un script en Python que publique en cada tópico de controlador de articulación y valide los límites articulares de cada junta. También, cree un script para suscribirse a los tópicos de controlador de articulación y retornar la configuración de 5 ángulos en grados.

### Python + ROS + Toolbox
Cree un código en Python que envíe la posición en ángulos deseada a cada articulación del robot utilizando ROS + Dynamixel. El programa debe graficar la configuración del robot usando las herramientas del toolbox, y esta configuración debe coincidir con la obtenida en el robot real.

### Pruebe las siguientes poses generadas a partir de los valores articulares de q1, q2, q3, q4, q5:
1. 0, 0, 0, 0, 0.
2. 25, 25, 20, -20, 0.
3. -35, 35, -30, 30, 0.
4. 85, -20, 55, 25, 0.
5. 80, -35, 55, -45, 0.

Asegúrese de que las poses no interfieran con los límites articulares ni con algún objeto en el espacio de trabajo.

### Interfaz de Usuario (HMI)
Desarrolle una interfaz gráfica (HMI) que muestre:
1. Nombres, logos y datos de los integrantes del grupo.
2. Imagen de la perspectiva de la posición actual del manipulador con la última posición enviada.
3. Opción para seleccionar una de las 5 poses y enviarlas al manipulador.
4. Valores reales de los ángulos articulares de cada motor.
5. Imagen de la perspectiva de la posición actual del manipulador con los valores articulares.

### Funcionalidades de la interfaz gráfica
- **Pestaña de control en espacio articular**: Use deslizadores para mover el robot en el espacio articular.
- **Pestaña de ingreso numérico articular**: Permita mover cada articulación a un valor determinado por el operador, respetando los límites articulares.
- **Pestaña de control en el espacio de la tarea**: Permita mover el robot en el espacio de la tarea, controlando el TCP del robot a lo largo de los ejes X, Y, Z y rotarlo.
- **Pestaña de visualización en RViz**: Visualice el modelo del robot en RViz y sincronice los movimientos en tiempo real con el manipulador real.
- **Pestaña de visualización numérica de la pose cartesiana**: Muestre la posición en X, Y, Z y la orientación en Roll-Pitch-Yaw (RPY) del TCP del robot en tiempo real.

## Entregables
1. Descripción detallada de la solución planteada.
2. Diagrama de flujo de acciones del robot utilizando la herramienta Mermaid.
3. Plano de planta de la ubicación de cada uno de los elementos.
4. Descripción de las funciones utilizadas.
5. Código del script utilizado para el desarrollo de la práctica.
6. Video del brazo alcanzando cada posición solicitada.
7. Video demostración de uso de la interfaz de usuario.
8. Gráfica digital de las poses comparándola con la fotografía del brazo real en la misma configuración.

## Fecha de entrega
Consultar la actividad en Moodle.

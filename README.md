<!-- ✦✦✦ FUTURE IS AUTOMATED ✦✦✦ -->
<!-- Banner superior “neón” -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=200&width=1200&color=0:04041A,50:14213D,100:0A4D68&text=Laboratorio%205%20-%20Pincher%20Phantom%20X100%20-%20ROS%20Humble%20-%20RVIZ&fontColor=E0FBFC&fontAlign=50&fontAlignY=30&desc=Laboratorio%205%20-%20Pincher%20Phantom%20X100%20-%20ROS%20Humble%20-%20RVIZ&descAlign=50&descAlignY=60" alt="header" />
</p>

<h1 align="center">🤖 LABORATORIO 5 – PINCHER PHANTOM X100 - ROS HUMBLE - RVIZ</h1>

<p align="center">
  <img src="https://img.shields.io/badge/ROS2-Humble-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Phantom%20X%20Pincher-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/RobotStudio-2025-blue?style=for-the-badge" />
</p>

<!-- Línea de texto mecanografiado (animado) -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&pause=1200&duration=3500&color=00E5FF&center=true&vCenter=true&lines=Pincher%20Phantom%20X100%20ROS%202%20Control;%20Dynamixel%20AX-12%20Servomotors;%20RobotStudio%20-%20RViz%20Visualization" alt="typing">
</p>

---

### 🛰️ Descripción general

Este repositorio implementa el **Laboratorio No. 5** de *Robótica Industrial 2025-II*: automatización del **robot Phantom X Pincher** utilizando **ROS Humble** y **RViz** para visualización.  
Incluye la creación de **Joint Controllers** para los servomotores **Dynamixel AX-12**, manipulación de **tópicos** y **servicios** de ROS, y conexión con Python.

---

## 🧑‍🚀 Objetivos
1. **Crear todos los Joint Controllers** con ROS para manipular servomotores Dynamixel AX-12 del robot Phantom X Pincher.
2. **Manipular los tópicos de estado y comando** para todos los Joint Controllers del robot Phantom X Pincher.
3. **Manipular los servicios** para todos los Joint Controllers del robot Phantom X Pincher.
4. **Conectar el robot Phantom X Pincher con Python usando ROS 2**.

---

## 🧑‍🔧 Requisitos
- Ubuntu versión 22.xx preferible 22.04 LTS con ROS Humble.
- Espacio de trabajo para `colcon build` correctamente configurado.
- Paquetes de Dynamixel Workbench: [Dynamixel Workbench GitHub](https://github.com/labsir-un/ROB_Intro_ROS2_Humble_Phantom_Pincher_X100.git)
- Paquete del robot Phantom X: [Phantom X GitHub](https://github.com/labsir-un/ROB_Intro_ROS2_Humble_Phantom_Pincher_X100_RVIZ.git)
- Python.
- Un (1) manipulador Phantom X Pincher con su entorno de trabajo.

---

## 🛠️ Ejercicio en el laboratorio

### Mediciones
Establezca las longitudes de eslabón para cada articulación del robot Phantom X Pincher usando un calibrador. Genere un diagrama con los datos medidos, como el ejemplo presentado en la figura 2 de la guía.

### Análisis
Con las dimensiones medidas, obtenga los parámetros DH del robot Phantom X Pincher. Genere un diagrama del robot con las tablas de parámetros articulares utilizando software de ilustración.

---

## 🤖 ROS 2
Cree un script en **ROS 2** que publique a los tópicos y llame a los servicios correspondientes para realizar el movimiento de cada una de las articulaciones del manipulador (waist, shoulder, elbow, wrist). La lógica del script debe ser la siguiente:
1. Realice el movimiento entre dos posiciones angulares características: una de home y otra objetivo.
2. El movimiento de las articulaciones debe realizarse de forma secuencial, comenzando por la articulación de la base. Agregue una pequeña espera entre cada movimiento.

---

## Python + ROS + Toolbox
Cree un código en Python que envíe la posición en ángulos deseada a cada articulación del robot utilizando **ROS** + **Dynamixel**. El programa debe graficar la configuración del robot usando las herramientas del toolbox, y esta configuración debe coincidir con la obtenida en el robot real.

---

## 🧑‍💻 Funcionalidades de la interfaz gráfica

Desarrollar una **interfaz gráfica (HMI)** que permita:
1. Nombres, logos y datos de los integrantes del grupo.
2. Imagen de la perspectiva de la posición actual del manipulador con la última posición enviada.
3. Opción para seleccionar una de las 5 poses y enviarlas al manipulador.
4. Valores reales de los ángulos articulares de cada motor.
5. Imagen de la perspectiva de la posición actual del manipulador con los valores articulares.

---

### 🎮 Funcionalidades de control

- **Pestaña de control en espacio articular**: Usa deslizadores para mover el robot en el espacio articular.
- **Pestaña de ingreso numérico articular**: Permite mover cada articulación a un valor determinado por el operador, respetando los límites articulares.
- **Pestaña de control en el espacio de la tarea**: Permite mover el robot en el espacio de la tarea, controlando el TCP del robot a lo largo de los ejes X, Y, Z y rotarlo.
- **Pestaña de visualización en RViz**: Visualiza el modelo del robot en RViz y sincroniza los movimientos en tiempo real con el manipulador real.
- **Pestaña de visualización numérica de la pose cartesiana**: Muestra la posición en X, Y, Z y la orientación en Roll-Pitch-Yaw (RPY) del TCP del robot en tiempo real.

---

## 📝 Entregables

1. Descripción detallada de la solución planteada.
2. Diagrama de flujo de acciones del robot utilizando la herramienta **Mermaid**.
3. Plano de planta de la ubicación de cada uno de los elementos.
4. Descripción de las funciones utilizadas.
5. Código del script utilizado para el desarrollo de la práctica.
6. Video del brazo alcanzando cada posición solicitada.
7. Video demostración de uso de la interfaz de usuario.
8. Gráfica digital de las poses comparándola con la fotografía del brazo real en la misma configuración.

---

## 📅 Fecha de entrega
Consultar la actividad en **Moodle**.

---

<!-- ===== INICIO BLOQUE ANIMACIONES EQUIPO ===== -->

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

<!-- ===== FIN BLOQUE ANIMACIONES EQUIPO ===== -->

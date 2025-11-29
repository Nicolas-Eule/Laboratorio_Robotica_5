## Lab 05 – Tareas pendientes para finalizar

Este documento resume **qué falta por implementar** para completar el Lab 05 con el PhantomX Pincher X100, tomando como base el análisis de los paquetes y nodos ya disponibles.

---

## 1. Modelo geométrico y DH

- [ ] **Construir la tabla DH completa del brazo**
  - A partir del URDF/Xacro (`phantomx_pincher_arm.xacro`) o de mediciones físicas.
  - Incluir \(a_i\), \(\alpha_i\), \(d_i\), \(\theta_i\) para cada articulación activa.
- [ ] **Elaborar un diagrama del robot con los frames DH**
  - Mostrar claramente el sistema de referencia base y el frame del efector final (TCP).

---

## 2. Scripts ROS 2 en espacio articular

- [ ] **Script 1 – Movimiento secuencial HOME → pose objetivo**
  - Nodo ROS 2 en Python.
  - Realizar el movimiento desde HOME hasta una configuración objetivo **por articulación**, en el orden:
    - base → shoulder → elbow → wrist (y gripper si aplica).
  - Incluir pequeñas esperas entre movimientos de cada articulación para que se vea el movimiento escalonado.

- [ ] **Script 2 – Publicación de comandos articulares en grados**
  - Publicar comandos articulares en **grados**, convirtiendo internamente a radianes/ticks según corresponda.
  - **Validar límites articulares** (según Xacro/URDF) antes de enviar los comandos.
  - Integrarse con:
    - `pincher_control/control_servo.py`, o
    - `pincher_control/follow_joint_trajectory_node.py`, o
    - el nodo/tema de control articular que se use en el laboratorio.

- [ ] **Script 3 – Lectura de ángulos articulares en grados**
  - Suscribirse a `/joint_states` (o al nodo que publique el estado articular).
  - Calcular y mostrar/imprimir los **5 ángulos en grados respecto a HOME**.
  - Dejar claro en la salida cuál es el orden de las articulaciones.

---

## 3. Integración Python + ROS 2 + Toolbox (cinemática directa)

- [ ] **Script de cinemática directa con Toolbox**
  - Usar los parámetros DH definidos en la sección 1 en una toolbox de robótica (Matlab, Python Robotics Toolbox u otra).
  - Recibir una configuración articular (por ejemplo, las 5 poses propuestas en la guía).
  - Enviar esa configuración al robot (vía ROS 2).
  - Calcular la **cinemática directa** para obtener la pose cartesiana del TCP.
- [ ] **Comparación con RViz / robot real**
  - Graficar el modelo en la toolbox y comparar visualmente con:
    - La pose mostrada en RViz.
    - La pose física del robot (si se dispone de hardware).
  - Verificar coherencia (al menos cualitativa) entre ambas representaciones.

---

## 4. Extensiones de la interfaz gráfica (HMI)

- [ ] **Personalización de la GUI**
  - Añadir información del **grupo** (nombres de integrantes, logos, etc.) en la ventana principal o en una pestaña “Acerca de”.

- [ ] **Botones para poses predefinidas**
  - Definir al menos **5 poses** relevantes (por ejemplo, HOME y 4 poses de trabajo).
  - Añadir botones a la GUI para:
    - Enviar cada una de esas poses al robot en espacio articular.
    - Mostrar el nombre o descripción de cada pose.

- [ ] **Pestaña de control en espacio de la tarea**
  - Crear una nueva pestaña con sliders o campos numéricos para:
    - **X, Y, Z** (m).
    - **Roll, Pitch, Yaw** (rad o grados, pero documentado claramente).
  - Conectar esta pestaña al tópico `pose_command` (`phantomx_pincher_interfaces/PoseCommand`) o a un nodo equivalente.
  - Permitir elegir si se quiere:
    - Movimiento directo a la pose (planificación en espacio de configuración).
    - Trayectoria cartesiana (usando `cartesian_path = true`).

- [ ] **Pestaña de visualización numérica de la pose cartesiana**
  - Mostrar en tiempo real la pose cartesiana del TCP:
    - **X, Y, Z** (m).
    - **Roll, Pitch, Yaw** (rad o grados).
  - Obtener estos datos ya sea de:
    - La cinemática directa implementada con la Toolbox, o
    - La información de MoveIt (por ejemplo, pose actual del `end_effector_link`).

---

## 5. Entregables sugeridos

- [ ] **Documento o sección de informe**
  - Explicar brevemente:
    - Cómo se obtuvo la tabla DH.
    - Cómo se validó la cinemática directa.
    - Cómo se integró ROS 2 + Toolbox + GUI.
- [ ] **Evidencias**
  - Capturas de pantalla de:
    - RViz con el modelo del robot.
    - La GUI con las nuevas pestañas y botones.
    - La toolbox mostrando el modelo y la pose.
  - Video corto (si es posible) mostrando:
    - El movimiento secuencial HOME → pose objetivo.
    - El uso del control en espacio de la tarea desde la GUI.



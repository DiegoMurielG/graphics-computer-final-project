# 🕹 **MANUAL DE USUARIO – Controles y Funciones del Proyecto 3D**

Este manual explica **todas las teclas y acciones** disponibles dentro de la aplicación 3D desarrollada con GLFW + OpenGL.
Incluye movimiento, cámaras, animaciones, interacción, visualización, sonido y funciones auxiliares.

---

# ⭐ 1. **Controles del Personaje (Movimiento)**

### **W**

Avanzar.

### **S**

Retroceder.

### **A**

Mover a la izquierda (strafe).

### **D**

Mover a la derecha (strafe).

### **Shift Izquierdo**

Correr / aumentar velocidad de movimiento.

### **Ctrl Izquierdo**

Movimiento lento / caminar.

### **Espacio**

Saltar (si está implementado en `HandleMovementKeys`).

---

# ⭐ 2. **Control de Cámara – Primera y Tercera Persona**

### **C**

Alternar entre:

* **1ra persona**
* **3ra persona orbital**

### **Mouse (1ra persona)**

* Girar la cámara libremente (yaw y pitch).

### **Mouse (3ra persona)**

La cámara orbita alrededor del personaje.

* Movimiento horizontal → gira alrededor del personaje.
* Movimiento vertical → cambia la altura del ángulo.
* Con inversión activada:

  * X invertido
  * Y invertido

### **Rueda del Mouse**

Acerca o aleja la cámara (zoom).

---

# ⭐ 3. **Interacción**

### **E**

Interactuar con objetos del entorno.

Usos visibles en código:

* Activar puertas automáticas.
* Mostrar overlays (“Presione E”).
* Iniciar o detener animaciones o keyframes.

---

# ⭐ 4. **Animaciones y Keyframes**

### **O**

Guardar un keyframe en el índice actual.

### **P**

Reproducir los keyframes grabados.

### **L**

Limpiar / resetear los keyframes.

*(Todas estas teclas afectan las variables `KeyFrame`, `play`, `FrameIndex`, etc.)*

---

# ⭐ 5. **Control de Sofi (personaje animado secundario)**

El script indica movimiento y animaciones en `UpdateSofi()`.

### **Flechas ← ↑ ↓ →**

Mover la posición objetivo de Sofi (OrbitTarget).

### **H**

Reiniciar posición de Sofi.

*(Basado en `OrbitTarget.movable` y funciones de movimiento).*

---

# ⭐ 6. **Abrir / Cerrar Puertas**

Se activa automática o manualmente.

### **E**

* Si estás cerca → abre o cierra la puerta.
* También activa el overlay “Presione E”.

La puerta también se abre si **te acercas** (proximidad automática).

---

# ⭐ 7. **Visualización – Modo Malla / Aristas / Puntos**

El renderizador permite cambiar cómo se dibujan los objetos:

### **N**

Modo *malla* (`GL_LINE`).

### **M**

Modo *aristas* (wireframe reforzado).

### **B**

Modo *puntos* (`GL_POINT`).

Además:

### **, (coma)**

Disminuir grosor de líneas.

### **. (punto)**

Aumentar grosor de líneas.

### **; (punto y coma)**

Disminuir tamaño de puntos.

### **' (comilla)**

Aumentar tamaño de puntos.

---

# ⭐ 8. **Audio**

### **V**

Mutear o desmutear todo el audio.

### **G**

Reducir volumen maestro.

### **H**

Aumentar volumen maestro.

### **BARRA ESPACIADORA (si está cerca del suelo y en movimiento)**

Activa sonidos de paso automáticos (system interno).

*(Los pasos dependen de velocidad y deltaTime).*

---

# ⭐ 9. **Sistema de Guardado / Captura**

### **F2**

Guardar un frame (captura) con `saveFrame()`.

*(El archivo se guarda en el directorio del proyecto.)*

### **F1**

Restaurar elementos a su estado inicial (`resetElements()`).

---

# ⭐ 10. **Orbit Targets (Cambio de objetivo de cámara orbital)**

Si hay varios objetivos de cámara:

### **Tab**

Cambiar entre objetivos preconfigurados en `gTargets`.

---

# ⭐ 11. **Controles Globales y de Ventana**

### **ESC**

Cerrar la aplicación.

### **Alt + Enter**

(Depende del comportamiento de la ventana) Cambiar a fullscreen en algunos sistemas.

---

# ⭐ 12. **Debug / Desarrollo (si está habilitado)**

### **K**

Interpolación para keyframes (`interpolation()`).

### **F3**

Mostrar información de resolución / debug.

### **1, 2, 3...**

Cambiar shaders o materiales (si se conectaron a `HandleActionKeys`).

---

# ⭐ **RESUMEN RÁPIDO DE CONTROLES**

### **Movimiento**

W, A, S, D – mover
Shift – correr
Ctrl – caminar
Espacio – saltar

### **Cámara**

C – cambiar cámara
Mouse – rotar
Scroll – zoom

### **Interacción**

E – interactuar

### **Modo de dibujo**

N/M/B – mesh / wireframe / puntos

### **Audio**

V – mute
G/H – volumen − / +

### **Keyframes**

O – guardar
P – reproducir
L – limpiar

### **Otros**

ESC – salir
F2 – captura

---

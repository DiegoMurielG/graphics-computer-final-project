# 🕹 MANUAL DE USUARIO – Controles y funciones del proyecto 3D[1]

Este manual reúne todas las teclas y acciones disponibles en la aplicación 3D con GLFW + OpenGL: movimiento, cámaras, interacción, visualización, audio y utilidades de cámara/objetivos.[1]

***

# ⭐ 1. Controles del personaje (movimiento)[1]

### W[1]
Avanzar cuando está activa la cámara libre de 1ra persona o el objetivo movible en 3ra persona.[1]

### S[1]
Retroceder cuando está activa la cámara libre de 1ra persona o el objetivo movible en 3ra persona.[1]

### A[1]
Mover a la izquierda (strafe) en 1ra persona o desplazar el objetivo hacia su izquierda en 3ra persona.[1]

### D[1]
Mover a la derecha (strafe) en 1ra persona o desplazar el objetivo hacia su derecha en 3ra persona.[1]

### Shift (izq/der)[1]
Aumenta temporalmente la velocidad de movimiento (aprox. 3x) mientras se mantiene presionada.[1]

### Ctrl (izq/der)[1]
Reduce temporalmente la velocidad de movimiento (caminar lento) mientras se mantiene presionada.[1]

***

# ⭐ 2. Control de cámara – primera y tercera persona[1]

### F1[1]
Activar cámara de 3ra persona orbital (la cámara orbita al objetivo actual y el ratón controla la órbita).[1]

### F2[1]
Activar cámara libre de 1ra persona (el ratón controla yaw/pitch de la vista en primera persona).[1]

### Mouse (1ra persona)[1]
Girar libremente la cámara (yaw y pitch) mientras te desplazas con WASD y límites de altura aplicados.[1]

### Mouse (3ra persona)[1]
Orbitado alrededor del objetivo activo: horizontal para giro alrededor del objetivo y vertical para altura del ángulo.[1]

### Rueda del mouse[1]
Zoom de la cámara ajustando el FOV a través del scroll del ratón.[1]

***

# ⭐ 3. Interacción[1]

### E[1]
Interactuar con objetos cercanos del entorno (por ejemplo, abrir/cerrar la puerta manual si la apertura automática está desactivada).[1]

### T[1]
Alternar apertura automática de la puerta por proximidad (cuando está activa, la puerta reacciona a la distancia).[1]

***

# ⭐ 4. Animaciones y keyframes (si está habilitado)[1]

### P[1]
Reproducir la secuencia de keyframes grabados cuando exista una animación configurada.[1]

### L[1]
Guardar un keyframe o limpiar el estado según la implementación disponible en tu build actual.[1]

Nota: Este proyecto prioriza animaciones procedurales (puerta, multinstancia de personajes y UpdateSofi); la disponibilidad de edición de keyframes depende de la configuración activa.[1]

***

# ⭐ 5. Control de Sofi (personaje animado)[1]

### Flechas ← ↑ ↓ →[1]
Mover la posición del objetivo Sofi cuando está seleccionado como objetivo activo en 3ra persona (usa su yaw actual para adelante/derecha).[1]

### Ratón (3ra persona)[1]
El giro horizontal del ratón ajusta el yaw de Sofi cuando Sofi es el objetivo activo, manteniendo alineados vista y movimiento.[1]

***

# ⭐ 6. Abrir / cerrar puertas[1]

### E (manual)[1]
Si estás cerca, abre o cierra la puerta manualmente cuando la apertura automática esté desactivada.[1]

### T (automática)[1]
Activa o desactiva la apertura automática por proximidad para la puerta del museo.[1]

***

# ⭐ 7. Visualización – sólido / líneas / puntos[1]

### N[1]
Modo sólido (relleno) para el render normal de la escena.[1]

### M[1]
Modo líneas (wireframe) para depurar superficies y topología.[1]

### B[1]
Modo puntos para visualizar vértices de las mallas.[1]

***

# ⭐ 8. Audio[1]

- Sonidos de pasos: Se reproducen automáticamente a intervalos al detectar movimiento continuo del objetivo/cámara según el temporizador interno.[1]
- Variación: Cada paso elige aleatoriamente uno de tres archivos para evitar repetición perceptible.[1]
- Silencio global: El audio maestro puede silenciarse o reactivarse según el control de volumen global configurado en el proyecto.[1]

***

# ⭐ 9. Orbit targets (cambio de objetivo de cámara orbital)[1]

### 9 / 0[1]
Cambiar entre objetivos preconfigurados (por ejemplo, Sofi, puerta, ventilador) y actualizar de inmediato la órbita de la cámara.[1]

Nota: Los objetivos marcados como movibles pueden desplazarse con las flechas; los no movibles sirven solo para enfocar/visitar con la cámara.[1]

***

# ⭐ 10. Controles globales y de ventana[1]

### ESC[1]
Cerrar la aplicación de forma segura.[1]

Límite de altura: La cámara nunca bajará de y = 2 en 1ra y 3ra persona gracias a un clamp aplicado tras cada actualización de posición.[1]

***

# ⭐ 11. Debug / desarrollo[1]

- Cambios de modo de dibujo (N/M/B) permiten inspección rápida de la escena sin recompilar.[1]
- La selección de objetivos (9/0) ayuda a validar colisiones locales, iluminación y alineación de instancias en áreas específicas.[1]

***

# ⭐ Resumen rápido de controles[1]

- Movimiento: W, A, S, D; Shift acelera; Ctrl desacelera.[1]
- Cámara: F1 3ra persona, F2 1ra persona; mouse para rotar; scroll para zoom.[1]
- Interacción: E abrir/cerrar; T auto-puerta por proximidad.[1]
- Dibujo: N sólido; M líneas; B puntos.[1]
- Objetivos: 9/0 cambiar objetivo orbital; flechas mueven el objetivo activo si es movible.[1]
- Audio: pasos automáticos al moverte; volumen maestro conmutado según configuración global.[1]

[1](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/4522242/c4307585-d3ab-43d4-88eb-9162ae201b36/ProyectoFinal.txt)

# Apuntes-de-clase-Unidad-1

## Unidad I. Introducción a la graficación por computadora.

En este trabajo se presenta una investigación documental sobre los fundamentos de la graficación por computadora, abordando su origen, evolución tecnológica y las bases teóricas que permiten la creación y manipulación de imágenes digitales. El estudio inicia con un recorrido histórico que explica cómo surgieron los primeros sistemas gráficos, desde los dispositivos vectoriales y el proyecto Sketchpad, hasta la consolidación de los métodos de renderización y los avances modernos en animación, simulación y visualización 3D.

A lo largo del desarrollo se analizan las principales áreas de aplicación de la graficación —como el cine, los videojuegos, la medicina, la ingeniería y la arquitectura— destacando su importancia en la representación visual de información y en la creación de entornos virtuales. También se revisaron los aspectos matemáticos esenciales, incluyendo vectores, matrices, transformaciones geométricas y técnicas fundamentales para el trazo de líneas y polígonos, los cuales constituyen la base de cualquier motor gráfico.

Asimismo, se estudiaron los modelos de color más utilizados (RGB, CMY, HSV y HSL), comprendiendo cómo cada uno describe y estructura la información cromática según su propósito, ya sea para pantallas, impresión o manipulación artística del color. Como complemento práctico, se integró un pequeño tutorial utilizando Blender, donde se explica cómo iluminar un cubo y aplicar colores a sus caras para observar de forma directa el comportamiento de la luz y los materiales.

En conjunto, esta investigación permite entender cómo se originan las imágenes generadas por computadora, qué fundamentos matemáticos y perceptuales intervienen en su elaboración y de qué manera estas tecnologías se aplican en diferentes campos profesionales, sentando las bases para estudios posteriores en gráficos avanzados, animación y modelado 3D.

# 1.1 Historia y evolución de la graficación por computadora

La graficación por computadora es una disciplina que combina matemáticas, computación y arte para crear imágenes de forma digital. Desde sus inicios ha evolucionado a la par de los avances tecnológicos en hardware y software.

## Primeros pasos (1950–1960)
- En 1950 se realizaron los primeros experimentos con osciloscopios creando formas geométricas simples.
- En 1963, Ivan Sutherland creó **Sketchpad**, considerado el primer programa de gráficos interactivos.
- Año clave: introducción de las primeras pantallas de vector.

## Evolución en los 70's
- Aparición de **modelado 3D básico**.
- Uso de gráficos en simuladores militares.
- Popularización de algoritmos como *pintor*, *Bresenham* y representaciones en mallas.

## Década de 1980
- Se integra graficación en computadoras personales.
- Aparecen estaciones Silicon Graphics (SGI).
- Nacen las primeras películas con gráficos 3D (TRON, 1982).

## 1990–2000
- Explosión del 3D realista.
- Aparición de **rendereadores avanzados**.
- Videojuegos en 3D.

## Actualidad
- Cinemática hiperrealista (Pixar, Unreal Engine).
- Computación gráfica en realidad virtual, arquitectura, medicina y más.

# 1.2 Áreas de aplicación

La graficación por computadora se ha extendido a una gran variedad de disciplinas:

##  1. Videojuegos
Los motores gráficos procesan miles de polígonos por segundo para simular mundos virtuales.

##  2. Cine y animación
Películas animadas, CGI, efectos especiales y composición digital.

##  3. Ingeniería y simulación
Modelos en CAD, simulaciones de fluido, estructuras y dinámica.

##  4. Medicina
- Reconstrucción 3D de órganos
- Imágenes tomográficas
- Cirugía asistida

##  5. Ciencia y visualización de datos
Visualización de grandes conjuntos de datos astronómicos, meteorológicos o estadísticos.

##  6. Arquitectura
Render y modelado de espacios interiores y exteriores.

##  7. Diseño gráfico y publicidad
Carteles, ilustraciones, gráficos vectoriales, animación 2D/3D.

## 8. Realidad virtual y aumentada
Experiencias inmersivas en educación, ocio, medicina y entrenamiento.

# 1.3 Aspectos matemáticos de la graficación

Los gráficos por computadora dependen fuertemente de las matemáticas, especialmente las siguientes áreas:

## Álgebra lineal
Base fundamental para manipular posiciones y transformaciones.

- Vectores
- Matrices de transformación (traslación, rotación, escala)
- Matriz de proyección
- Producto punto y cruz

## Geometría analítica
Para representar lineas, polígonos y curvas:

- Rectas paramétricas
- Planos
- Intersecciones y colisiones

## Cálculo
Útil para animación y simulaciones físicas:

- Derivadas para velocidad/aceleración
- Integrales en simulación de movimiento

## Matemáticas del color
- Espacios de color
- Transformaciones entre modelos RGB ↔ HSV
- Gamma y corrección de brillo

## Algoritmos numéricos
- Interpolación lineal (LERP)
- Normalización de vectores
- Métodos para rasterizar líneas y polígonos

# 1.4 Modelos del color: RGB, CMY, HSV y HSL

Los modelos de color son formas de representar colores numéricamente.

---

# 🎨 Modelo RGB (Red, Green, Blue)
Es un modelo **aditivo** utilizado en pantallas.

- (255, 0, 0) → rojo
- (0, 255, 0) → verde
- (0, 0, 255) → azul

La combinación máxima → blanco.

---

# 🖨 Modelo CMY/CMYK
Modelo **sustractivo**, utilizado en impresión.

- Cian
- Magenta
- Amarillo
- (K = Negro) para mayor contraste

Funciona absorbiendo luz en lugar de emitirla.

---

# 🎛 Modelo HSV (Hue, Saturation, Value)
Representa colores según percepción humana:

- **Hue:** tono (0–360°)
- **Saturation:** intensidad
- **Value:** brillo

---

# 🎛 Modelo HSL (Hue, Saturation, Lightness)
Similar al HSV, pero Lightness define claridad.

---

# TUTORIAL: Cómo iluminar un cubo y sus caras en Blender

## PASO 1 — Crear un cubo
1. Abre Blender
<img width="1362" height="724" alt="image" src="https://github.com/user-attachments/assets/5c0f290b-722e-4255-9a7f-88a32d515d91" />

3. Presiona **A** → Suprimir objetos  
4. Agrega un cubo: **Shift + A → Mesh → Cube**
<img width="396" height="276" alt="{03F55CEA-FD16-4BC0-92E9-8207988BD619}" src="https://github.com/user-attachments/assets/fc19cfe2-9805-4fff-b499-f4bee8ef88fd" />

## PASO 2 — Activar vista renderizada
En la esquina superior derecha:  
**Viewport Shading → Rendered**
<img width="354" height="111" alt="{C3699362-18E5-4FC6-8352-0B4F2A08042C}" src="https://github.com/user-attachments/assets/83be044d-cd66-4355-9071-4e46bf9ca7c4" />

## PASO 3 — Agregar una luz
1. **Shift + A → Light → Point Light**
  <img width="469" height="103" alt="{11C992E7-814D-42A8-AB13-ED1B4C6C4166}" src="https://github.com/user-attachments/assets/e7ae17f8-6930-4540-9895-8d6077a26a93" />

3. Mueve la luz con:
   - **G** para mover
<img width="290" height="239" alt="{8C8D2536-5BAD-4BCE-A041-C5EA43ADB28F}" src="https://github.com/user-attachments/assets/065dd89f-2d4b-4352-bfae-85647f45355b" />

## PASO 4 — Material para cada cara
1. Selecciona el cubo  
2. En modo edición: **Tab**  
3. Selecciona una cara  
4. Ve a **Material Properties**
<img width="245" height="495" alt="image" src="https://github.com/user-attachments/assets/06b692ab-aa2c-4bba-b8fa-5a73734b6b69" />

6. Crea un material nuevo  
7. Asigna color con modelo **HSV** o **RGB**  
8. Presiona **Assign**

Repite para cada cara.
<img width="949" height="624" alt="image" src="https://github.com/user-attachments/assets/11e47b75-a13e-4d5d-bb38-b98bf48fd4ec" />

## Resultado
El cubo tendrá:
- Caras iluminadas con color

<img width="295" height="258" alt="image" src="https://github.com/user-attachments/assets/2941eefd-e595-4ff1-8ec4-5977d6d8b374" />



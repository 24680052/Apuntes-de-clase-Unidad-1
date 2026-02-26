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

# 1.5 Representación y trazo de líneas y polígonos

La representación digital de líneas y polígonos es esencial en gráficos por computadora, ya que constituyen las primitivas básicas para formar figuras y modelos más complejos.

## - Representación de líneas

Las líneas deben aproximarse a una malla de píxeles. Los algoritmos más importantes son:

### Algoritmo DDA (Digital Differential Analyzer)
- Calcula los puntos intermedios mediante incrementos fraccionales.
- Sencillo pero menos eficiente por el uso de números decimales.

### Algoritmo de Bresenham
- Solo utiliza operaciones enteras.
- Muy eficiente para rasterizar líneas.
- Es el más usado en sistemas gráficos y videojuegos.

---

## - Representación de polígonos

Los polígonos son superficies definidas por líneas conectadas. Son la base del modelado 2D y 3D.

### Tipos de polígonos
- **Convexos:** más fáciles de rasterizar.
- **Cóncavos:** requieren dividirse en polígonos convexos.

### Métodos de relleno
- **Scanline:** recorre la imagen horizontalmente para llenar áreas.
- **Flood Fill:** rellena desde un punto interior.
- **Boundary Fill:** depende de un color delimitador.

Estos métodos permiten construir superficies visibles en modelos 3D y renderizados.

# 1.5.1 Formatos de imagen

Un formato de imagen define cómo se almacena la información visual. Se dividen en raster (mapas de bits) y vectoriales.

---

## Formatos raster

Los más comunes:

### JPG/JPEG
- Compresión con pérdida.
- Ideal para fotografías.

### PNG
- Compresión sin pérdida.
- Soporta transparencia (canal alfa).

### GIF
- Paleta de 256 colores.
- Permite animación simple.

### BMP
- Sin compresión.
- Archivos pesados.

### TIFF
- Muy usado en escaneo e impresión profesional.

---

## ✏ Formatos vectoriales

### SVG
- Basado en XML.
- Escalable sin perder calidad.

### EPS
- Gráficos para impresión.

### PDF
- Puede contener gráficos vectoriales y raster.
  
# Poligono (Ejercicio practico)
# Generador de poligono 2D en Blender

## Explicacion 

Este proyecto consiste en el desarrollo de un poligono 2D usando **Python** dentro de BLender mediante la API bpy.
El script genera una malla personalizada calculando los vertices mediante trigonometria y conectandolos a traves de aristas para formar una figura cerrada. 

---

# Objetivo del proyecto

- Comprender el uso de la API bpy en Blender.
- Aplicar conversion de coordenadas polares a cartesianas.
- Generar mallas manualmente mediante Python.
- Automatiar la creacion de geometria dentro de Blender.

---

# Explicacion tecnica del codigo

## Importacion de modulos 

Python

import bpy
import math 

·bpy: permite interactuar con BLender a nivel interno 
·math: se utiliza para realizar calculos matematicos como seno, coseno y pi

# Creacion de la malla y objeto 

`malla = bpy.data.meshes.new(nombre)
objeto = bpy.data.objects.new(nombre, malla)
bpy.context.collection.objects.link(objeto)`

Aquí se:

· Crea una nueva estructura de malla. 
· Se crea un objeto que usa esa malla.
· Se vincula el objeto a la colección activa de la escena.

# Calculo de vertices

`for i in range(lados):
    angulo = 2 * math.pi * i / lados
    x = radio * math.cos(angulo)
    y = radio * math.sin(angulo)
    vertices.append((x, y, 0))1. Abrir Blender
`

Se realiza:

· División del círculo completo (2π radianes) entre el número de lados.
· Conversión de coordenadas polares a cartesianas.
· Se fija Z = 0 para mantener la figura en el plano 2D.

# Creación de aristas

`
for i in range(lados):
    aristas.append((i, (i + 1) % lados))
`
Cada vértice se conecta con el siguiente.
El operador módulo (%) permite que el último vértice se conecte nuevamente con el primero, cerrando la figura.

# Carga de datos en la malla

`malla.from_pydata(vertices, aristas, [])
malla.update()
`
Se cargan:
Lista de vértices
Lista de aristas
Lista de caras (vacía en este caso)

# Limpieza de la escena

`bpy.ops.object.select_all(action='SELECT')
bpy.ops.object.delete()
`
Se eliminan todos los objetos antes de crear el nuevo polígono para evitar superposición.

# Llamada final. 

`crear_poligono_2d("Poligono2D", lados=6, radio=5)
`
Se genera un hexágono con radio 5 unidades.

---

## Cómo ejecutar el script.

1. Abrir Blender.
2. Ir a la pestaña **Scripting**.

<img width="1023" height="51" alt="image" src="https://github.com/user-attachments/assets/6adb7ec3-621f-496a-943a-d510599e4c0f" />

4. Abrir el archivo `poligono.py`.
5. Presionar **Run Script** o Alt + P.`

---

# Parametros configurales
En la ultima linea del codigo se puede modificar
python

crear_poligono_2d("oligno", lados=6, radio=5)

·lados -> Numero de lados del poligono. 
·radio -> Tamaño del poligono.

---

# Codigo completo 

<img width="596" height="607" alt="image" src="https://github.com/user-attachments/assets/e7e28087-dd02-4f12-8dfd-6d54548d26d7" />

```
import bpy
import math

def crear_poligono_2d(nombre, lados, radio):
malla = bpy.data.meshes.new(nombre)
objeto = bpy.data.objects.new(nombre, malla)

bpy.context.collection.objects.link(objeto)  
  
vertices = []  
aristas = []  
  
for i in range(lados):  
    angulo = 2 * math.pi * i / lados  
    x = radio * math.cos(angulo)  
    y = radio *math.sin(angulo)  
    vertices.append((x, y, 0)) # Z = 0 para mantenerlo en 2D  
      
for i in range (lados):  
        aristas.append((i, (i + 1) % lados))  
          
malla.from_pydata(vertices, aristas, [])  
malla.update()

bpy.ops.object.select_all(action='SELECT')
bpy.ops.object.delete()

crear_poligono_2d("Poligono2D", lados=6, radio=5)
```
---


## Resultado 

<img width="506" height="621" alt="image" src="https://github.com/user-attachments/assets/c593e366-b7ec-49e2-8999-96307840e8e0" />

El ejemplo actual genera un **hexagono** de radio 5 unidades.

# Flor de vida (Ejercicio practico)



# 1.6 Procesamiento de mapas de bits

El procesamiento de mapas de bits consiste en modificar imágenes pixel por pixel, lo cual es esencial en edición digital y motores gráficos.

---

## - Operaciones básicas

### Brillo
Incrementa o reduce los valores RGB.

### Contraste
Amplifica la diferencia entre tonos claros y oscuros.

### Saturación y tono
Ajuste del modelo HSV/HSL.

### Escala de grises
Convierte la imagen mediante luminancia.

### Negativo
Invierte los colores.

---

## - Transformaciones geométricas
- Traslación  
- Rotación  
- Escalado  
- Reflexión  

Estas operaciones modifican la estructura espacial de los píxeles.

---

## - Filtrado por convolución

Los kernels permiten aplicar efectos:
- Suavizado (blur)  
- Enfoque  
- Detección de bordes (Sobel, Prewitt)  
- Emboss  

Se aplican mediante multiplicación matricial con la vecindad de cada píxel.

---

## - Aplicaciones en 3D y videojuegos

Los mapas de bits permiten:
- Crear texturas
- Normal maps
- Height maps
- HDRI
- Interfaces gráficas (HUD)

Son fundamentales en motores como Unity, Unreal Engine y Blender.


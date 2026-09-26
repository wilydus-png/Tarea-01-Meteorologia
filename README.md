# Tarea 01 - Análisis de Datos Meteorológicos

## Maestría en Ciencia de Datos

---

# 1. Descripción del proyecto

Este proyecto tiene como objetivo desarrollar un flujo completo de análisis de datos meteorológicos mediante la adquisición de información desde una API pública, procesamiento de datos utilizando Python y generación de visualizaciones para interpretar el comportamiento de diferentes variables climáticas.

Para el desarrollo del trabajo se utilizó la API gratuita **Open-Meteo**, obteniendo información meteorológica horaria correspondiente a la ciudad de **Cuenca, Ecuador** durante un período de siete días.

El análisis contempla las siguientes etapas:

- Adquisición de datos mediante una API.
- Procesamiento y transformación de información.
- Almacenamiento de datos en formato CSV.
- Visualización mediante gráficos.
- Análisis de resultados mediante preguntas planteadas.

---

# 2. Objetivos

## Objetivo general

Realizar la adquisición y análisis de datos meteorológicos utilizando una API pública, aplicando herramientas de programación en Python para procesar, visualizar e interpretar la información obtenida.

## Objetivos específicos

- Obtener datos meteorológicos mediante la API Open-Meteo.
- Procesar la información utilizando estructuras de análisis de datos.
- Generar visualizaciones utilizando Matplotlib.
- Identificar patrones de comportamiento entre variables meteorológicas.
- Responder preguntas de análisis basadas en los datos obtenidos.

---

# 3. Fuente de datos

Los datos fueron obtenidos mediante la API gratuita:

**Open-Meteo**

https://open-meteo.com/

La ubicación seleccionada para el análisis fue:

**Ciudad:** Cuenca, Ecuador

**Coordenadas utilizadas:**

- Latitud: -2.8953
- Longitud: -78.9963

Los datos fueron consultados con una frecuencia horaria.

---

# 4. Variables analizadas

Para el desarrollo del análisis se utilizaron las siguientes variables meteorológicas:

| Variable | Descripción | Unidad |
|---|---|---|
| temperature_2m | Temperatura a 2 metros | °C |
| relative_humidity_2m | Humedad relativa a 2 metros | % |
| wind_speed_10m | Velocidad del viento a 10 metros | km/h |
| precipitation | Precipitación acumulada | mm |

---

# 5. Preguntas de análisis

Para orientar el estudio de los datos se plantearon las siguientes preguntas:

### Pregunta 1

¿Cómo varía la temperatura en Cuenca durante los siete días analizados y cuáles son las temperaturas máxima y mínima?

### Pregunta 2

¿Cómo se comporta la precipitación durante el período analizado y cuál es la precipitación acumulada?

### Pregunta 3

¿Qué relación existe entre la temperatura y la humedad relativa durante el período analizado?

---

# 6. Metodología aplicada

El flujo desarrollado para el análisis fue:

API Open-Meteo
        ↓
Adquisición de datos mediante Python
        ↓
Procesamiento con Pandas
        ↓
Construcción del DataFrame
        ↓
Almacenamiento en archivo CSV
        ↓
Visualización mediante Matplotlib
        ↓
Análisis e interpretación de resultados


El proceso desarrollado permitió transformar datos meteorológicos obtenidos desde una fuente externa en información estructurada para su posterior análisis.

Las etapas principales del trabajo fueron:

**1. Adquisición de datos**

Se realizó la conexión con la API de Open-Meteo mediante Python para obtener información meteorológica horaria de Cuenca, Ecuador.

**2. Procesamiento de datos**

Los datos obtenidos fueron organizados utilizando Pandas, permitiendo construir un DataFrame para facilitar su análisis.

**3. Almacenamiento de datos**

La información procesada fue almacenada en un archivo CSV para conservar los datos utilizados en el análisis.

**4. Visualización de datos**

Se generaron gráficos mediante Matplotlib para analizar el comportamiento de las variables meteorológicas.

**5. Análisis de resultados**

Finalmente, se interpretaron los datos obtenidos y se respondieron las preguntas planteadas mediante los resultados estadísticos y visualizaciones generadas.

# 7. Adquisición y procesamiento de datos

La adquisición de datos fue realizada mediante Python utilizando la librería:

- `openmeteo_requests`

Posteriormente, los datos fueron procesados utilizando:

- `Pandas`

El conjunto de datos obtenido contiene:

- **168 registros horarios**
- Correspondientes a **7 días de información meteorológica**

Los datos procesados fueron almacenados localmente en:

Este archivo contiene la información utilizada posteriormente para el análisis y generación de gráficos.

---

# 8. Visualización de datos

Para analizar el comportamiento de las variables meteorológicas se generaron cinco visualizaciones utilizando la librería:

- `Matplotlib`

Las visualizaciones desarrolladas fueron:

1. Temperatura horaria.
2. Humedad relativa horaria.
3. Precipitación horaria.
4. Velocidad del viento horaria.
5. Relación entre temperatura y humedad relativa.

---

# 9. Visualizaciones generadas

Para analizar el comportamiento de las variables meteorológicas se generaron cinco visualizaciones utilizando Matplotlib. Estas gráficas permiten identificar tendencias, variaciones y posibles relaciones entre las variables analizadas.

---

## 9.1 Temperatura horaria

La gráfica muestra la variación de la temperatura durante el período analizado. Permite identificar los momentos del día con mayores y menores valores térmicos, evidenciando los cambios de temperatura entre horas.

![Temperatura](graficas/01_temperatura.png)

---

## 9.2 Humedad relativa horaria

Esta visualización representa el comportamiento de la humedad relativa a lo largo del tiempo. Permite observar cómo la humedad presenta variaciones durante el día y su comportamiento respecto a los cambios de temperatura.

![Humedad](graficas/02_humedad.png)

---

## 9.3 Precipitación horaria

La gráfica permite identificar los períodos donde se registraron precipitaciones y observar la distribución de la lluvia durante los siete días analizados. Los valores más altos representan los momentos con mayor acumulación de precipitación.

![Precipitación](graficas/03_precipitacion.png)

---

## 9.4 Velocidad del viento horaria

Esta gráfica muestra la variación de la velocidad del viento durante el período de estudio. Permite analizar los cambios en la intensidad del viento a diferentes horas.

![Velocidad del viento](graficas/04_viento.png)

---

## 9.5 Relación entre temperatura y humedad relativa

Mediante un gráfico de dispersión se analiza la relación entre la temperatura y la humedad relativa. La distribución de los puntos permite identificar el comportamiento conjunto de ambas variables y evaluar la existencia de una relación entre ellas.

![Relación temperatura humedad](graficas/05_temperatura_humedad.png)

# 10. Resultados obtenidos

## Pregunta 1: Variación de temperatura

Durante el período analizado se obtuvieron los siguientes resultados:

- Temperatura máxima registrada: **23,00 °C**
- Temperatura mínima registrada: **8,70 °C**

La diferencia entre ambos valores representa una amplitud térmica de:

**14,30 °C**

Estos resultados muestran la variación existente entre las temperaturas más bajas y más altas durante el período analizado.

---

## Pregunta 2: Comportamiento de la precipitación

Durante los siete días analizados se obtuvo:

- Precipitación acumulada: **33,70 mm**
- Mayor precipitación registrada en una hora: **4,70 mm**

La precipitación presentó variaciones durante el período, concentrándose en determinadas horas con mayores acumulaciones.

---

## Pregunta 3: Relación entre temperatura y humedad

Para analizar la relación entre ambas variables se calculó el coeficiente de correlación:

**Coeficiente de correlación: -0,951**

Este resultado representa una relación lineal negativa fuerte entre temperatura y humedad relativa.

Durante el período analizado se observa que:

- Cuando aumenta la temperatura, la humedad relativa tiende a disminuir.
- Cuando disminuye la temperatura, la humedad relativa tiende a aumentar.

---

# 11. Conclusiones

El desarrollo del proyecto permitió aplicar un proceso completo de análisis de datos, iniciando desde la adquisición de información mediante una API pública hasta la generación de resultados mediante técnicas de visualización.

El uso de Python permitió automatizar la extracción, transformación y análisis de los datos meteorológicos obtenidos desde Open-Meteo.

Las visualizaciones generadas facilitaron la identificación de patrones en variables como temperatura, humedad, precipitación y velocidad del viento.

Finalmente, el análisis de correlación permitió identificar una relación inversa entre temperatura y humedad relativa durante el período estudiado.

---

# 12. Herramientas utilizadas

Las herramientas utilizadas fueron:

- Python
- Pandas
- Matplotlib
- Open-Meteo API
- Google Colab
- GitHub

---

# 13. Estructura del proyecto

---

# 14. Repositorio

El proyecto completo se encuentra disponible en GitHub, incluyendo:

- Código fuente.
- Datos utilizados.
- Visualizaciones.
- Documentación del análisis.

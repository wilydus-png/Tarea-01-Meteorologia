# Tarea 01 - Análisis de Datos Meteorológicos

## Maestría en Ciencia de Datos

## 1. Descripción del proyecto

Este proyecto tiene como finalidad realizar un flujo completo de análisis de datos meteorológicos mediante la adquisición de información desde una API pública, procesamiento de datos utilizando Python y generación de visualizaciones para interpretar patrones climáticos.

Para el desarrollo del trabajo se utilizó la API de **Open-Meteo**, obteniendo información meteorológica horaria de la ciudad de **Cuenca, Ecuador**, durante un período de siete días.

El análisis contempla la extracción, transformación, almacenamiento y visualización de datos, aplicando herramientas utilizadas habitualmente en procesos de análisis de datos.

---

# 2. Objetivos

## Objetivo general

Obtener y analizar datos meteorológicos mediante una API, aplicando técnicas de procesamiento y visualización de datos con Python.

## Objetivos específicos

- Consumir información meteorológica desde una API pública.
- Transformar los datos obtenidos en una estructura adecuada para análisis.
- Almacenar los datos en un archivo local.
- Generar visualizaciones utilizando Matplotlib.
- Analizar relaciones entre variables meteorológicas y responder preguntas basadas en los datos.

---

# 3. Fuente de datos

Los datos utilizados fueron obtenidos mediante la API gratuita:

Open-Meteo  
https://open-meteo.com/

La ubicación seleccionada para el análisis fue:

**Ciudad:** Cuenca, Ecuador  
**Latitud:** -2.8953  
**Longitud:** -78.9963

La consulta fue realizada utilizando información meteorológica horaria.

---

# 4. Variables analizadas

Las variables seleccionadas para el estudio fueron:

| Variable | Descripción | Unidad |
|---|---|---|
| temperature_2m | Temperatura a 2 metros | °C |
| relative_humidity_2m | Humedad relativa a 2 metros | % |
| wind_speed_10m | Velocidad del viento a 10 metros | km/h |
| precipitation | Precipitación acumulada | mm |

---

# 5. Preguntas de análisis

Para orientar el análisis se plantearon las siguientes preguntas:

### Pregunta 1
¿Cómo varía la temperatura en Cuenca durante los siete días analizados y cuáles son las temperaturas máxima y mínima?

### Pregunta 2
¿Cómo se comporta la precipitación durante el período analizado y cuál es la precipitación acumulada?

### Pregunta 3
¿Qué relación existe entre la temperatura y la humedad relativa durante el período analizado?

---

# 6. Metodología aplicada

El flujo desarrollado fue:

---

# 7. Adquisición y procesamiento de datos

La extracción de información fue realizada mediante Python utilizando la librería:

- `openmeteo_requests`

Posteriormente los datos fueron procesados utilizando:

- `Pandas`

El conjunto obtenido contiene:

- **168 registros horarios**
- Correspondientes a **7 días de información meteorológica**

Los datos procesados fueron almacenados localmente en:

---

# 8. Visualización de datos

Para analizar el comportamiento de las variables meteorológicas se generaron cinco visualizaciones utilizando la librería:

- `Matplotlib`

Las gráficas desarrolladas fueron:

1. Temperatura horaria.
2. Humedad relativa horaria.
3. Precipitación horaria.
4. Velocidad del viento horaria.
5. Relación entre temperatura y humedad relativa.

---

# 9. Resultados obtenidos

## 9.1 Análisis de temperatura

Durante el período analizado:

- Temperatura máxima registrada: **23,00 °C**
- Temperatura mínima registrada: **8,70 °C**

La diferencia entre ambos valores representa una amplitud térmica de:

**14,30 °C**

### Visualización

![Temperatura](graficas/01_temperatura.png)


---

## 9.2 Análisis de humedad relativa

La humedad relativa permitió observar el comportamiento de la humedad durante las diferentes horas del período analizado.

### Visualización

![Humedad](graficas/02_humedad.png)


---

## 9.3 Análisis de precipitación

Durante los siete días analizados:

- Precipitación acumulada: **33,70 mm**
- Mayor precipitación horaria registrada: **4,70 mm**

La precipitación presentó variaciones durante el período, concentrándose en determinadas horas.

### Visualización

![Precipitación](graficas/03_precipitacion.png)


---

## 9.4 Análisis de velocidad del viento

La velocidad del viento fue analizada para identificar sus variaciones horarias durante el período estudiado.

### Visualización

![Viento](graficas/04_viento.png)


---

## 9.5 Relación entre temperatura y humedad

Para analizar la relación entre variables se calculó el coeficiente de correlación:

**Correlación = -0,951**

Este resultado indica una relación lineal negativa fuerte entre temperatura y humedad relativa.

Durante el período analizado:

- Cuando aumenta la temperatura, la humedad relativa tiende a disminuir.
- Cuando disminuye la temperatura, la humedad relativa tiende a aumentar.

### Visualización

![Relación temperatura humedad](graficas/05_temperatura_humedad.png)

---

# 10. Conclusiones

El desarrollo del proyecto permitió implementar un flujo completo de análisis de datos meteorológicos, iniciando desde la adquisición mediante una API hasta la interpretación de resultados mediante técnicas de visualización.

El uso de Python facilitó la automatización del proceso de extracción, transformación y análisis de información, mientras que las visualizaciones permitieron identificar patrones en las variables meteorológicas estudiadas.

Finalmente, la correlación encontrada entre temperatura y humedad permitió evidenciar una relación inversa entre ambas variables durante el período analizado.

---

# 11. Herramientas utilizadas

- Python
- Pandas
- Matplotlib
- Open-Meteo API
- Google Colab
- GitHub

---

# 12. Estructura del proyecto

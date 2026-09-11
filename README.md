# Análisis de uso de servicios móviles - ConnectaTel

## Descripción del proyecto

Este proyecto analiza el comportamiento de los clientes de **ConnectaTel**, una empresa de telecomunicaciones con operaciones en México y Colombia.

El análisis busca comprender cómo los usuarios utilizan los servicios móviles, principalmente llamadas y mensajes, identificar comportamientos atípicos y detectar segmentos de clientes con diferentes necesidades.

##  Objetivo

Analizar los patrones de uso de los clientes de ConnectaTel para:

- Identificar diferencias en el comportamiento de los usuarios.
- Comparar el uso de los servicios entre los distintos planes.
- Detectar valores atípicos o usuarios con consumos inusuales.
- Identificar segmentos de clientes según sus características y nivel de uso.
- Generar recomendaciones que puedan ayudar a mejorar la oferta comercial.

##  Datasets utilizados

El proyecto utiliza tres archivos CSV:

- `plans.csv`: información de los planes disponibles, como precio, minutos y GB incluidos y costos adicionales.
- `users_latam.csv`: información de los clientes, incluyendo edad, ciudad, fecha de registro y plan contratado.
- `usage.csv`: registros del uso de los servicios, incluyendo llamadas, duración de llamadas y mensajes.

##  Etapas del análisis

El proyecto se desarrolló en las siguientes etapas:

1. Carga y exploración inicial de los datos.
2. Identificación y tratamiento de problemas de calidad de los datos.
3. Integración de las diferentes fuentes de información.
4. Análisis exploratorio de datos (EDA).
5. Visualización de distribuciones mediante histogramas.
6. Comparación del comportamiento según el tipo de plan.
7. Identificación de valores atípicos mediante boxplots.
8. Análisis de outliers utilizando el método IQR.
9. Segmentación de clientes según edad y nivel de consumo.
10. Elaboración de conclusiones y recomendaciones para ConnectaTel.

##  Cómo ejecutar el proyecto

El análisis se encuentra desarrollado en un **Jupyter Notebook (`.ipynb`)**.

Una forma sencilla de ejecutarlo es utilizando **Google Colab**:

1. Descargar el archivo `.ipynb` de este repositorio.
2. Ingresar a Google Colab.
3. Seleccionar **Archivo → Subir notebook**.
4. Cargar el archivo `.ipynb`.
5. Subir los archivos CSV utilizados en el proyecto.
6. Ejecutar las celdas en orden desde el inicio.

##  Guía de reproducción

Para reproducir correctamente el análisis:

1. Tener disponibles `plans.csv`, `users_latam.csv` y `usage.csv`.
2. Abrir el notebook en Google Colab o Jupyter Notebook.
3. Verificar que las rutas de los archivos CSV correspondan con su ubicación.
4. Ejecutar las celdas en el orden establecido.
5. Revisar las visualizaciones, resultados y conclusiones generadas.

##  Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab

##  Principales hallazgos

El análisis permitió observar que el **nivel de consumo es un factor más útil que la edad para diferenciar a los clientes**.

También se identificaron usuarios con niveles de consumo considerablemente superiores al comportamiento habitual, especialmente en los minutos de llamada. Estos valores atípicos pueden representar clientes de alto consumo y posibles oportunidades para desarrollar ofertas o planes adaptados a sus necesidades.

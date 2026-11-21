# sprint7-final-project
Sprint 7 - Final Project

# Análisis de uso de clientes - ConnectaTel

## 🎯 Objetivo del proyecto
Analizar el comportamiento de uso de los clientes de ConnectaTel (llamadas y mensajes) para identificar patrones de consumo, detectar comportamientos atípicos y segmentar a los usuarios según edad y nivel de uso, con el fin de apoyar decisiones comerciales sobre los planes ofrecidos.

## 📂 Datasets utilizados
- `plans.csv`: catálogo de planes (precio, minutos incluidos, GB incluidos, costo por extra).
- `users_latam.csv`: información de los clientes (edad, ciudad, fecha de registro, plan contratado).
- `usage.csv`: detalle de uso real (duración de llamadas, longitud de mensajes).

## 🔍 Etapas del análisis
1. Exploración inicial de los tres datasets (estructura, tipos de datos, valores nulos).
2. Limpieza de datos: tratamiento de valores faltantes ("?"), fechas inválidas y valores atípicos (-999) en `age`.
3. Verificación del patrón de nulos en `usage` (MAR) en las columnas `duration` y `length`.
4. Agregación de datos de uso por cliente (`usage_agg`) y unión con `users` para crear `user_profile`.
5. Estadística descriptiva de las variables numéricas (media, mediana).
6. Visualización con histogramas y boxplots para detectar distribución y outliers.
7. Segmentación de clientes por nivel de uso (`grupo_uso`) y por edad (`grupo_edad`).
8. Visualización de los segmentos con gráficos de conteo.
9. Conclusiones y recomendaciones de negocio.

## ▶️ Cómo ejecutar el notebook
1. Abrir el archivo `.ipynb` en Google Colab o Jupyter Notebook.
2. Asegurarse de tener instaladas las librerías: `pandas`, `numpy`, `seaborn`, `matplotlib`.
3. Cargar los archivos `plans.csv`, `users_latam.csv` y `usage.csv` en el mismo entorno (o ajustar las rutas de carga).
4. Ejecutar las celdas en orden, de arriba hacia abajo.

## 🔁 Guía de reproducción
- Clonar o descargar este repositorio.  
- Verificar que los tres archivos CSV estén en la misma carpeta que el notebook.
- Ejecutar `pip install pandas numpy seaborn matplotlib` si falta alguna librería.
- Correr todas las celdas del notebook para reproducir el análisis completo.

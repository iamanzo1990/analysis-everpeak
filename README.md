# analysis-everpeak
Análisis ConnectaTel

##Objetivo del proyecto##

Evaluar el comportamiento de los clientes de una empresa de telecomunicaciones en Latinoamérica, ConnectaTel. El objetivo de la empresa es identificar patrones de uso, detectar comportamientos atípicos y comprender qué segmentos de clientes muestran necesidades diferenciadas, con el fin de optimizar la oferta comercial y mejorar la experiencia del usuario.

##Datasets empleados##

- plans.csv: los planes actuales (precio, minutos incluidos, GB incluidos, costo por extra).
- users_latam.csv: información de clientes: edad, ciudad, fecha de registro, plan contratado.
- usage.csv: el detalle de uso real: llamadas (duración) y mensajes (longitud).

##Etapas del análisis realizado##

1.- Exploración de la estructura de los datasets
2.- Identificación de problemas de calidad de datos (valores nulos, inválidos y sentinels)
3.- Estandarización de fechas
4.- Limpieza básica de datos (sentinels y fechas imposibles)
5.- Agrupación por comportamiento de uso
6.- Resumen estadístico por usuario durante el 2024
7.- Visualización de Distribuciones
8.- Identificación de Outliers
9.- Segmentación de Clientes por uso y edades
10.- Visualización de la Segmentación de Clientes
11.- Insight Ejecutivo para Stakeholders

##Ejecución del notebook##

### Requisitos previos

- Python 3.9 o superior
- Jupyter Notebook, JupyterLab o Google Colab
- Librerías utilizadas:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`

##Breve guía de reproducción##

1. **Carga de datos:** se importan `plans.csv`, `users_latam.csv` y `usage.csv`, y se revisa su estructura (dimensiones, tipos de datos, columnas).
2. **Calidad de datos:** se detectan valores nulos, inválidos y sentinels (valores placeholder que no representan datos reales).
3. **Estandarización y limpieza:** se unifica el formato de fechas, se tratan los sentinels y se eliminan o corrigen las fechas imposibles.
4. **Agrupación y resumen por usuario:** se agrega el uso (llamadas y mensajes) por cliente y se calculan estadísticas descriptivas para el año 2024.
5. **Exploración visual:** se generan las distribuciones de las variables de uso y se identifican outliers.
6. **Segmentación:** se clasifica a los clientes según su nivel de uso y edad, y se visualizan los segmentos resultantes.
7. **Conclusiones:** se redacta el insight ejecutivo con hallazgos y recomendaciones para los stakeholders.


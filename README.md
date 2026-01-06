# Analisis-de-la-calidad-del-aire-y-la-movilidad-urbana-en-la-ciudad-de-Lima
Análisis de la relación entre calidad del aire (SENAMHI) y ciclovías (MML) en Lima Metropolitana
## Proyecto: Movilidad Sostenible y Calidad del Aire en Lima Metropolitana. 
### Resumen del Proyecto
Este proyecto analiza la relación entre la infraestructura ciclista actual y los niveles de contaminación atmosférica en distritos clave de Lima. El objetivo es identificar si la red de movilidad activa está ubicada en zonas de bajo riesgo ambiental o si existe una "doble vulnerabilidad" en distritos con alta contaminación y baja inversión en ciclovías.
### El Problema
Lima enfrenta retos críticos de salud pública debido a la antigüedad de su parque automotor y una distribución desigual de vías seguras para el transporte no motorizado. Se planteó la pregunta: ¿Existe una correlación entre la densidad de ciclovías y la reducción de gases contaminantes como el Dióxido de Nitrógeno (NO2)?.
### Metodología (Pipeline de Datos)
Siguiendo una lógica de ingeniería de datos, el flujo de trabajo fue el siguiente:
Recolección: Extracción de microdatos desde la Plataforma Nacional de Datos Abiertos, utilizando datasets del SENAMHI (Monitoreo de Aire) y la Municipalidad Metropolitana de Lima (Inventario de Ciclovías).
Limpieza y Procesamiento (Python): Normalización de nombres de distritos mediante el manejo de cadenas y eliminación de tildes para asegurar un cruce de datos (Merge) preciso.
  Tratamiento de valores nulos en sensores de monitoreo, preservando la integridad de las mediciones de PM10, PM2.5 y NO2.
  Uso de la librería Pandas para la agregación estadística de promedios anuales y sumatorias de infraestructura por distrito.
Visualización y Storytelling: Creación de gráficos comparativos multivariables mediante Matplotlib, permitiendo observar la disparidad entre la carga contaminante y la oferta de movilidad.
### Hallazgos Principales
Zona Crítica de Tráfico: San Juan de Lurigancho registró el promedio más alto de NO2 ($31.4 \mu g/m^3$), evidenciando una alta congestión vehicular que no es compensada proporcionalmente por su red de ciclovías ($11.7 km$).
Contaminación por Partículas: Villa María del Triunfo presenta niveles críticos de PM10 ($97.4 \mu g/m^3$), siendo el distrito con menor infraestructura ciclista registrada ($0.29 km$) en el análisis.
Liderazgo en Infraestructura: San Borja destaca con la mayor red de ciclovías ($28.4 km$), aunque sus niveles de NO2 ($21.0 \mu g/m^3$) indican que aún existe un impacto significativo del tráfico circundante.
### Conclusiones y Propuesta Social
El análisis demuestra que la expansión de ciclovías no siempre coincide con las áreas de mayor necesidad ambiental. Se recomienda priorizar la inversión en distritos del "Anillo Vial Exterior" (como SJL y VMT) para reducir la exposición de los ciudadanos a contaminantes de largo plazo, alineando el desarrollo urbano con los indicadores de salud ambiental de SENAMHI.

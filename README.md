# Analisis de Accidentes
## Objetivo
Analizar los accidentes de tránsito en zonas urbanas y suburbanas en México, utilizando los datos abiertos del Gobierno Federal. Se aplicarán técnicas de análisis descriptivo para obtener insights sobre tendencias, distribución y características de los accidentes.

## Instrucciones 
1. Preparación y Carga de Datos 
- ~~Descargue el dataset ATUS desde datos.gob.mx. ~~
- ~~Divida el archivo CSV en partes de máximo 20MB para facilitar su manejo en GitHub. Puede hacerlo con pandas o - herramientas como split en Linux/macOS.~~
- ~~Suba el dataset a su repositorio en GitHub.~~
- ~~Enlace su repositorio con Kaggle o Google Colaboratory.~~
- ~~Invite al profesor al repositorio.~~
- Solo trabajaremos con los datos de los últimos 3 años.
2. Exploración de Datos
- Lea y analice el diccionario de datos para comprender el significado de cada variable.
- Revise los catálogos de datos y verifique los valores únicos de las variables categóricas.
- Cargue en un DataFrame los datos de los últimos 3 años.
- Transformaciones iniciales:
  - Cree una nueva columna fecha_hora combinando las columnas Año, Mes, Día, Hora y Minuto en formato de fecha.
  - Cree una columna Zona con los valores "Urbana" o "Suburbana", según corresponda.
  - Cree una columna Area con el área específica donde ocurrió el accidente.
  - Elimine las columnas URBANA y SUBURBANA, ya que ahora están representadas en Zona.
3. Estadística Descriptiva
Realice un análisis estadístico de las siguientes variables para entender su distribución:

   1. Número de accidentes por municipio:
       - Media, mediana, moda.
       - Rango y desviación estándar.
        > ¿Existen municipios con valores atípicos?
   2. Número de víctimas (muertos y lesionados):

        - Media y mediana por estado.
        - ¿Qué estados tienen una mayor variabilidad en el número de víctimas?
   3. Distribución por hora del día:
       - Calcule la hora del día con mayor número de accidentes.
       - ¿Hay patrones en la ocurrencia de accidentes según la hora?
   4. Comparación entre zonas urbanas y suburbanas:
       - Media de accidentes en cada zona.
       - ¿En qué zona hay mayor dispersión de accidentes?

> Pregunta reflexiva: ¿Qué diferencias existen entre la media y la mediana en estos casos? ¿La presencia de valores extremos afecta la interpretación de los datos?

4. Análisis Descriptivo
   1. Municipios sin accidentes: Identifique el municipio de cada estado que tuvo más dias sin accidentes. ¿Por qué podrían no registrarse accidentes en algunos municipios?
   2. Distribución de tipos de accidentes:
     - Resuma los accidentes del último año por tipo.
     - Calcule el porcentaje que representa cada tipo sobre el total.
     - ¿Qué tipo de accidente es el más frecuente? ¿Existen diferencias entre zonas urbanas y suburbanas?
   3. Víctimas:
      - Obtenga la cantidad total de muertos y lesionados en los últimos 3 años.
      - ¿Ha aumentado o disminuido la severidad de los accidentes con el tiempo?
   4. Tendencia de accidentes por año:
   - Compare el número de accidentes de cada año con el anterior.
   - ¿Cuál fue el porcentaje de cambio año con año?
   - ¿Se observa una tendencia creciente o decreciente?
5. Visualización de Datos
Seleccione una o dos variables y genere las siguientes gráficas para interpretar los datos:

   - Histograma: Distribución de los accidentes por hora del día.
   - Gráfica de dispersión: Relación entre número de lesionados y el tipo de accidente.
   - Gráfica de líneas: Evolución mensual del número de accidentes en los últimos 3 años.
6. Entrega
   - Subir el análisis en un Notebook (.ipynb) con comentarios explicativos.
   - Generar un PDF con las visualizaciones clave y un breve resumen de los hallazgos.

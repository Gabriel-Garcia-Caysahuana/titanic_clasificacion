# Proyecto: Análisis y Predicción de Supervivencia en el Titanic

Este proyecto aplica técnicas de análisis de datos y aprendizaje automático para predecir la supervivencia de los pasajeros del Titanic. La base de datos utilizada proviene de [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data).

## Descripción del Proyecto

El análisis incluye el preprocesamiento de datos, exploración de variables, transformación de datos y modelado predictivo. Las principales etapas del proyecto son:

1. **Preprocesamiento de datos:**
   - Limpieza y transformación de variables.
   - Manejo de valores nulos y codificación de variables categóricas.
2. **Análisis exploratorio:**
   - Estadísticos descriptivos y gráficos univariados y bivariados.
3. **Transformación de datos:**
   - Creación de variables derivadas.
   - Transformación de Box-Cox para normalización.
4. **Modelado predictivo:**
   - Entrenamiento de un modelo de regresión logística.
   - Evaluación de métricas y visualización de resultados.

## Variables en el Dataset

- **survived:** Booleano que indica si el pasajero sobrevivió (0 = No, 1 = Sí).
- **pclass:** Clase del ticket (1 = 1ra clase, 2 = 2da clase, 3 = 3ra clase).
- **name:** Nombre del pasajero.
- **sex:** Sexo del pasajero (male o female).
- **age:** Edad del pasajero.
- **sibsp:** Número de hermanos/esposo/a a bordo.
- **parch:** Número de padres/hijos a bordo.
- **fare:** Tarifa del ticket.
- **cabin:** Identificador de la cabina.
- **embarked:** Puerto de embarque (C = Cherbourg, Q = Queenstown, S = Southampton).
- **adult_male:** Booleano (True si es hombre adulto, False en caso contrario).

## Dependencias

Las siguientes librerías son necesarias para ejecutar el proyecto:

- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `statsmodels`
- `tabulate`
- `numpy`

## Estructura del Proyecto

### 1. Preprocesamiento de datos

- Limpieza de inconsistencias y valores nulos.
- Codificación de variables categóricas (dummies).
- Creación de variables derivadas, como:
  - `alone`: Indica si el pasajero viajaba solo.
  - `title`: Extracto del título del nombre (Mr, Miss, etc.).
  - Segmentación de edad y tarifa (`fare_q`).

### 2. Análisis exploratorio

#### Estadísticos descriptivos
- Resumen estadístico de variables categóricas y numéricas.

#### Visualizaciones
- Gráficos univariados: histogramas y diagramas de sectores.
- Gráficos bivariados: distribución de variables categóricas según supervivencia.

### 3. Transformaciones

- Normalización mediante transformación de Box-Cox.
- Conversión de variables categóricas en indicadores binarios.

### 4. Modelado predictivo

- Entrenamiento de un modelo de regresión logística.
- Evaluación mediante:
  - Matriz de confusión.
  - Métricas de precisión, recall y F1-score.
  - Curva ROC y AUC.

## Resultados

### Evaluación del Modelo

- **Precisión Global:** 87%
- **AUC:** 0.92

### Insights Clave

1. Las mujeres y los pasajeros en 1ra clase tienen mayor probabilidad de supervivencia.
2. Los niños tienen una mayor tasa de supervivencia en comparación con adultos jóvenes y mayores.
3. Los pasajeros que pagaron tarifas más altas tienen una mayor probabilidad de supervivencia.

## Ejecución

1. Descargar los datos desde [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data).
2. Cargar los datos y ejecutar el análisis en un entorno compatible con Python (e.g., Jupyter Notebook).
3. Seguir el flujo de trabajo descrito en la estructura del proyecto.

## Contribuciones

Se aceptan propuestas de mejora al análisis o la implementación del modelo predictivo. Siéntase libre de hacer un pull request o reportar problemas.

---

Este proyecto ofrece un enfoque práctico y detallado para analizar y modelar datos históricos, con aplicaciones en aprendizaje automático y análisis exploratorio de datos.

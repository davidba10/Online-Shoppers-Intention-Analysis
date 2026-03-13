# Online Shoppers Intention Analysis

Proyecto de análisis de datos y machine learning aplicado al dataset **Online Shoppers Intention**, cuyo objetivo es analizar el comportamiento de los usuarios en una tienda online y predecir si un visitante terminará realizando una compra.

El proyecto combina **exploración de datos, análisis estadístico y modelos de clasificación** para entender qué factores influyen en la intención de compra.

---

# Contenido del repositorio

- `shopping_intention_analisis.ipynb` → notebook principal con todo el análisis
- `online_shoppers_intention.csv` → dataset utilizado
- `README.md` → descripción del proyecto

---

# Dataset

El dataset **Online Shoppers Intention** contiene información sobre sesiones de navegación de usuarios en un ecommerce.

Cada fila representa **una sesión de usuario**, incluyendo información como:

- comportamiento de navegación
- duración de las páginas visitadas
- tipo de visitante
- mes de la visita
- métricas analíticas del sitio web

La variable objetivo es:

```
Revenue
```

donde:

- `1` → el usuario realizó una compra
- `0` → el usuario no compró

---

# Variables principales

El dataset incluye variables de distintos tipos.

### Variables de comportamiento

- `Administrative`
- `Administrative_Duration`
- `Informational`
- `Informational_Duration`
- `ProductRelated`
- `ProductRelated_Duration`

Estas variables describen **cómo interactúa el usuario con el sitio web**.

---

### Variables analíticas

- `BounceRates`
- `ExitRates`
- `PageValues`
- `SpecialDay`

Estas métricas describen el **rendimiento de las páginas y la probabilidad de abandono**.

---

### Variables contextuales

- `Month`
- `OperatingSystems`
- `Browser`
- `Region`
- `TrafficType`
- `VisitorType`
- `Weekend`

Estas variables describen el **contexto técnico y temporal de la visita**.

---

# Pipeline del proyecto

El análisis sigue una estructura típica de ciencia de datos:

```
Carga del dataset
↓
Exploración de datos (EDA)
↓
Análisis de variables
↓
Preprocesamiento
↓
Construcción del modelo
↓
Evaluación del modelo
↓
Interpretación de resultados
```

---

# Exploratory Data Analysis (EDA)

En el notebook se realiza un análisis exploratorio para entender:

- distribución de variables
- correlaciones
- diferencias entre usuarios que compran y los que no

Se estudian aspectos como:

- qué variables están más asociadas con la compra
- qué características diferencian a los compradores
- cómo influyen métricas como `PageValues` o `ExitRates`

---

# Modelado

El problema se formula como un **problema de clasificación binaria**:

```
X → variables de navegación
y → Revenue (compra o no compra)
```

El objetivo del modelo es estimar la probabilidad de que una sesión termine en compra.

Los modelos de clasificación permiten:

- detectar patrones de comportamiento
- estimar intención de compra
- identificar variables relevantes

---

# Evaluación

Para evaluar el modelo se utilizan métricas típicas de clasificación:

- accuracy
- precision
- recall
- matriz de confusión

Estas métricas permiten analizar cómo de bien el modelo distingue entre:

- usuarios que compran
- usuarios que abandonan la web

---

# Qué demuestra este proyecto

Este proyecto demuestra habilidades en:

- exploración y análisis de datos
- preprocesamiento de datasets reales
- modelado predictivo
- interpretación de resultados
- análisis de comportamiento de usuarios
- uso de notebooks para análisis reproducible

También ilustra cómo los datos de navegación pueden utilizarse para **modelar la intención de compra en ecommerce**.

---

# Posibles mejoras

Algunas mejoras que podrían implementarse en futuras versiones:

- probar distintos modelos de clasificación
- optimización de hiperparámetros
- análisis de importancia de variables
- validación cruzada
- técnicas de balanceo de clases
- visualización más avanzada de patrones de compra

---

# Conclusión

El análisis del dataset **Online Shoppers Intention** permite observar cómo ciertas variables de comportamiento de navegación están relacionadas con la probabilidad de compra.

El uso de modelos de clasificación permite identificar patrones relevantes en las sesiones de los usuarios y construir sistemas capaces de predecir la intención de compra en tiempo real.

Este tipo de análisis es clave en ecommerce, donde entender el comportamiento del usuario puede mejorar estrategias de marketing, personalización y optimización de conversiones.

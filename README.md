# 📊 Análisis y Predicción de Evasión de Clientes (Churn) - TelecomX LATAM ✅ COMPLETADO

## 🎯 Descripción del Proyecto

Este proyecto presenta un análisis exhaustivo y la construcción de un modelo predictivo para la evasión de clientes (churn) en la empresa TelecomX. El objetivo se divide en dos fases:
1.  **Análisis Exploratorio (Completado):** Identificar patrones, factores de riesgo y perfiles de clientes propensos a cancelar.
2.  **Modelado Predictivo (Completado):** Desarrollar un pipeline de Machine Learning para predecir qué clientes tienen mayor probabilidad de cancelar sus servicios.

**🏆 Estado: PROYECTO COMPLETADO** - Incluye análisis exploratorio, desarrollo de modelos predictivos y recomendaciones estratégicas.

## 📁 Estructura del Proyecto

```
challenge2-data-science-LATAM/
├── TelecomX_Data.json          # Dataset principal con datos de clientes
├── TelecomX_diccionario.md     # Diccionario de datos con descripción de variables
├── TelecomX.ipynb             # Notebook principal con análisis y modelado completo
└── README.md                   # Documentación del proyecto
```

## 🔍 Dataset

- **Fuente**: API de TelecomX en formato JSON
- **Tamaño**: 7,043 registros limpios (de 7,267 iniciales)
- **Variables**: 21 características incluyendo datos demográficos, servicios contratados y estado de churn
- **Variable objetivo**: Churn (Yes/No) - indica si el cliente canceló el servicio

### Variables Principales:
- **Demográficas**: género, edad senior, pareja, dependientes
- **Servicios**: teléfono, internet, servicios adicionales
- **Contractuales**: tipo de contrato, método de pago, facturación
- **Financieras**: cargos mensuales, cargos totales, antigüedad

## 🛠️ Tecnologías Utilizadas

- **Python 3.x**
- **Pandas** & **NumPy** - Manipulación y análisis de datos
- **Matplotlib** & **Seaborn** - Visualización de datos
- **Scikit-learn** - Modelado de Machine Learning
- **Jupyter Notebook** - Entorno de desarrollo interactivo

## 📋 Metodología Completada

### Parte 1: Análisis Exploratorio ✅
- **Extracción y Transformación**: Carga, limpieza, normalización y codificación de datos.
- **Análisis Exploratorio (EDA)**: Identificación de patrones, correlaciones y perfiles de riesgo mediante visualizaciones.

### Parte 2: Modelado Predictivo de Churn ✅
- **Preparación de Datos**: División en conjuntos de entrenamiento/prueba y escalado de características.
- **Entrenamiento de Modelos**: Se entrenaron dos modelos de clasificación:
    1.  `Regresión Logística` (como línea de base).
    2.  `Random Forest Classifier` (modelo avanzado).
- **Evaluación de Modelos**: Comparación usando métricas como Accuracy, Precision, Recall, F1-Score y ROC AUC.
- **Interpretación**: Análisis de la importancia de las variables para entender los predictores clave del churn.

## 🔍 Principales Hallazgos

### Hallazgos del Análisis Exploratorio
- **Tasa de Churn Global**: 26.5% (1,869 de 7,043 clientes).
- **Período Crítico**: Los primeros 12 meses de antigüedad son los de mayor riesgo.
- **Factores Contractuales**: Contratos anuales o de dos años reducen el churn drásticamente.

### Resultados del Modelo Predictivo
- **Mejor Modelo**: El **Random Forest Classifier** superó a la Regresión Logística con un **ROC AUC de 0.84**, demostrando una capacidad robusta para identificar clientes en riesgo.
- **Principales Predictores de Churn**:
    1.  **Permanencia (`tenure`)**: El factor más importante. A menor antigüedad, mayor probabilidad de churn.
    2.  **Tipo de Contrato (`Contract_Month-to-month`)**: El predictor más fuerte después de la permanencia.
    3.  **Cargos Mensuales (`Charges.Monthly`)**: Cargos más altos se asocian con más cancelaciones.
    4.  **Servicio de Internet (`InternetService_Fiber optic`)**: Clientes con fibra óptica tienden a cancelar más, sugiriendo posibles problemas de precio o calidad.

## 🚀 Recomendaciones Estratégicas Implementadas

### 🎯 Retención Inmediata (Prioridad Alta)
- **Programa de onboarding extendido** para nuevos clientes (0-6 meses).
- **Sistema de alerta temprana** utilizando el modelo predictivo para identificar clientes con alto score de churn.
- **Incentivos contractuales** para migrar clientes de contratos mes a mes a compromisos de largo plazo.
- **Revisar la oferta de Fibra Óptica** para entender y mitigar las causas de la alta tasa de cancelación en este segmento.

### 📊 Segmentación y Mejoras
- **Estrategia "Bundle Inteligente"** con paquetes personalizados.
- **Capacidades analíticas avanzadas** con el pipeline de ML implementado.

## 🚦 Cómo Ejecutar el Proyecto

### Prerrequisitos
```bash
pip install pandas numpy matplotlib seaborn jupyter scikit-learn
```

### Ejecución
```bash
# Clonar el repositorio
git clone [repository-url]

# Navegar al directorio
cd challenge2-data-science-LATAM

# Abrir Jupyter Notebook
jupyter notebook TelecomX.ipynb
```

### Estructura del Notebook
1. **📌 Extracción y Limpieza**: Carga y preparación de datos.
2. **📊 Análisis Exploratorio**: Visualización detallada de patrones.
3. **🤖 Modelado y Predicción**: Pipeline de Machine Learning.
4. **📋 Informe Final**: Conclusiones, insights y recomendaciones.

---

## 👨‍🎓 Nota del Estudiante

Este proyecto representa un ciclo completo de ciencia de datos, desde el análisis inicial hasta la implementación de un modelo predictivo. Cada recomendación está respaldada por datos y por los resultados del modelo, demostrando cómo la ciencia de datos puede generar insights valiosos y herramientas proactivas para la toma de decisiones empresariales.

**Proyecto desarrollado como parte del desafío de Ciencia de Datos de Alura - LATAM**

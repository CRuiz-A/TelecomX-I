# 📊 Análisis de Evasión de Clientes (Churn) - TelecomX LATAM

## 🎯 Descripción del Proyecto

Este proyecto presenta un análisis exhaustivo de la evasión de clientes (churn) para la empresa TelecomX utilizando técnicas de ciencia de datos. El objetivo principal es identificar patrones, factores de riesgo y desarrollar estrategias de retención efectivas basadas en datos.

## 📁 Estructura del Proyecto

```
challenge2-data-science-LATAM/
├── TelecomX_Data.json          # Dataset principal con datos de clientes
├── TelecomX_diccionario.md     # Diccionario de datos con descripción de variables
├── TelecomX_LATAM.ipynb        # Notebook principal con análisis completo
└── README.md                   # Documentación del proyecto
```

## 🔍 Dataset

- **Fuente**: API de TelecomX en formato JSON
- **Tamaño**: +7,000 registros de clientes
- **Variables**: 21 características incluyendo datos demográficos, servicios contratados y estado de churn
- **Variable objetivo**: Churn (Yes/No) - indica si el cliente canceló el servicio

### Variables Principales:
- **Demográficas**: género, edad senior, pareja, dependientes
- **Servicios**: teléfono, internet, servicios adicionales
- **Contractuales**: tipo de contrato, método de pago, facturación
- **Financieras**: cargos mensuales, cargos totales, antigüedad

## 🛠️ Tecnologías Utilizadas

- **Python 3.x**
- **Pandas** - Manipulación y análisis de datos
- **NumPy** - Computación numérica
- **Matplotlib** - Visualización de datos
- **Seaborn** - Visualización estadística avanzada
- **Jupyter Notebook** - Entorno de desarrollo interactivo

## 📋 Metodología

### 1. 📌 Extracción
- Carga de datos desde archivo JSON
- Exploración inicial de la estructura del dataset

### 2. 🔧 Transformación
- **Detección de inconsistencias**: Identificación de problemas en los datos
- **Limpieza**: Corrección de tipos de datos, valores faltantes y duplicados
- **Estandarización**: Normalización de valores categóricos
- **Feature Engineering**: Creación de variable "Cuentas_Diarias"
- **Encoding**: Transformación de variables categóricas a numéricas

### 3. 📊 Análisis Exploratorio
- Análisis descriptivo de variables numéricas y categóricas
- Visualización de distribuciones y patrones
- Análisis de correlaciones
- Identificación de factores de riesgo

### 4. 📄 Informe Final
- Síntesis de hallazgos principales
- Recomendaciones estratégicas basadas en datos
- Propuesta de próximos pasos

## 🔍 Principales Hallazgos

### 📈 Métricas Clave
- **Tasa de Churn Global**: ~26.5%
- **Factor de Mayor Impacto**: Tipo de contrato
- **Período Crítico**: Primeros 12 meses de antigüedad

### 🎯 Perfil de Cliente en Riesgo
1. **Contractual**: Contrato mes a mes
2. **Financiero**: Cargos mensuales altos, baja antigüedad
3. **Método de Pago**: Cheque electrónico
4. **Servicios**: Fibra óptica sin servicios adicionales
5. **Demográfico**: Sin pareja ni dependientes

### 🛡️ Factores Protectores
- Contratos de 1-2 años
- Antigüedad > 24 meses
- Métodos de pago automáticos
- Múltiples servicios contratados

## 🚀 Recomendaciones Estratégicas

### 🎯 Retención Inmediata
- **Onboarding extendido** para nuevos clientes
- **Incentivos contractuales** para compromisos largos
- **Automatización de pagos** con beneficios

### 📊 Segmentación
- **Alto Riesgo**: Intervención proactiva
- **Riesgo Medio**: Programas de lealtad
- **Bajo Riesgo**: Expansión de servicios

### 🔧 Mejoras Operacionales
- Mejora de calidad en fibra óptica
- Simplificación de facturación
- Implementación de ML predictivo

## 📊 Impacto Esperado

- **Reducción del churn**: 15-20%
- **Aumento CLV**: 25-30%
- **Mejora NPS**: Medible a 6 meses

## 🚦 Cómo Ejecutar el Proyecto

### Prerrequisitos
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Ejecución
```bash
# Clonar el repositorio
git clone [repository-url]

# Navegar al directorio
cd challenge2-data-science-LATAM

# Abrir Jupyter Notebook
jupyter notebook TelecomX_LATAM.ipynb
```

### Estructura del Notebook
1. **Extracción**: Carga y exploración inicial
2. **Transformación**: Limpieza y preparación de datos
3. **Análisis**: Exploración y visualización
4. **Informe**: Conclusiones y recomendaciones

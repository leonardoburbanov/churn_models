# 📊 Modelos de Detección de Abandono de Clientes - Netflix

Este proyecto implementa modelos de machine learning para predecir el abandono de clientes (churn) utilizando datos de Netflix. El objetivo es desarrollar y evaluar diferentes algoritmos de clasificación para identificar patrones que indiquen la probabilidad de que un cliente abandone el servicio.

## 🎯 Características

- **Análisis exploratorio de datos** con visualizaciones interactivas
- **Múltiples algoritmos de clasificación** (Random Forest, Logistic Regression, SVM, etc.)
- **Evaluación de modelos** con métricas de rendimiento
- **Explicabilidad de modelos** usando SHAP values
- **Optimización de hiperparámetros** con GridSearchCV
- **Jupyter Notebook** para experimentación interactiva

## 🛠️ Tecnologías Utilizadas

- **Python 3.13+**
- **Pandas** - Manipulación y análisis de datos
- **Scikit-learn** - Algoritmos de machine learning
- **Matplotlib & Seaborn** - Visualizaciones
- **XGBoost** - Algoritmos de boosting
- **Jupyter** - Notebooks interactivos
- **uv** - Gestión de dependencias

## 📋 Requisitos Previos

Antes de comenzar, asegúrate de tener instalado:

- **Python 3.13** o superior
- **uv** (gestor de paquetes de Python)

### Instalación de uv (si no lo tienes)

```bash
# Windows (PowerShell)
pip install uv

# macOS/Linux
curl -LsSf https://astral.sh/uv/install.sh | sh
```

## 🚀 Instalación y Configuración

1. **Clona el repositorio**
   ```bash
   git clone <url-del-repositorio>
   cd churn_models
   ```

2. **Instala las dependencias**
   ```bash
   uv sync
   ```

3. **Activa el entorno virtual**
   ```bash
   uv shell
   ```

## 📖 Uso

### Opción 1: Jupyter Notebook (Recomendado)

1. **Inicia Jupyter Notebook**
   ```bash
   uv run jupyter notebook
   ```

2. **Abre el notebook**
   - Navega a `netflix_churn_prediction.ipynb`
   - Ejecuta las celdas en orden para seguir el análisis completo

### Opción 2: Ejecutar desde línea de comandos

```bash
uv run jupyter nbconvert --to notebook --execute netflix_churn_prediction.ipynb
```

## 📊 Datos

El proyecto utiliza el dataset `netflix_customer_churn.csv` que contiene:

### Variables del Dataset:
- **customer_id**: Identificador único del cliente
- **age**: Edad del cliente
- **gender**: Género del cliente
- **subscription_type**: Tipo de suscripción
- **watch_hours**: Horas de visualización
- **last_login_days**: Días desde el último login
- **region**: Región del cliente
- **device**: Dispositivo utilizado
- **monthly_fee**: Tarifa mensual
- **payment_method**: Método de pago
- **number_of_profiles**: Número de perfiles
- **avg_watch_time_per_day**: Tiempo promedio de visualización por día
- **favorite_genre**: Género favorito
- **churned**: Variable objetivo (1 = Abandona, 0 = No abandona)

**Fuente de datos**: [Netflix Customer Churn Dataset](https://www.kaggle.com/datasets/abdulwadood11220/netflix-customer-churn-dataset) en Kaggle

## 📁 Estructura del Proyecto

```
churn_models/
├── input/
│   └── netflix_customer_churn.csv    # Dataset principal (5000 registros)
├── netflix_churn_prediction.ipynb    # Notebook de análisis completo
├── pyproject.toml                    # Configuración del proyecto
├── uv.lock                          # Lock file de dependencias
├── .python-version                  # Versión de Python
├── .gitignore                       # Archivos ignorados por Git
├── LICENSE                          # Licencia del proyecto
└── README.md                        # Este archivo
```

## 🔬 Análisis Incluido

### 1. **Exploración de Datos**
   - Estadísticas descriptivas del dataset
   - Análisis de correlaciones entre variables
   - Visualizaciones de distribución de datos
   - Identificación de patrones en el abandono

### 2. **Preprocesamiento**
   - Limpieza de datos y manejo de valores faltantes
   - Codificación de variables categóricas (LabelEncoder)
   - Escalado de features (StandardScaler)
   - División train/test (80%/20%)

### 3. **Modelado**
   - **Regresión Logística**: Modelo lineal para clasificación
   - **Random Forest**: Ensemble de árboles de decisión
   - Evaluación con métricas de rendimiento
   - Análisis de importancia de features

### 4. **Evaluación de Modelos**
   - Matriz de confusión
   - Métricas de clasificación (Accuracy, Precision, Recall, F1)
   - Comparación de rendimiento entre modelos

## 📈 Modelos Implementados

### 1. **Regresión Logística**
- **Descripción**: Modelo lineal que utiliza la función sigmoidea
- **Ventajas**: Interpretable, rápido, bueno para relaciones lineales
- **Uso**: Clasificación binaria del abandono

### 2. **Random Forest**
- **Descripción**: Ensemble de múltiples árboles de decisión
- **Ventajas**: Maneja bien datos no lineales, robusto a overfitting
- **Uso**: Clasificación con mayor precisión

### 3. **XGBoost** (Incluido en dependencias)
- **Descripción**: Algoritmo de boosting con gradient descent
- **Ventajas**: Alto rendimiento, manejo de datos faltantes
- **Uso**: Optimización de rendimiento

## 📊 Métricas de Evaluación

Los modelos son evaluados usando:
- **Accuracy**: Precisión general del modelo
- **Precision**: Proporción de predicciones positivas correctas
- **Recall**: Proporción de casos positivos reales identificados
- **F1-Score**: Media armónica de precision y recall
- **Matriz de Confusión**: Visualización de predicciones vs valores reales

## 🔍 Análisis de Importancia de Features

El proyecto incluye análisis de importancia de variables para:
- Identificar qué factores más influyen en el abandono
- Optimizar estrategias de retención de clientes
- Entender patrones de comportamiento

## 🚀 Próximas Mejoras

- [ ] Implementación de modelos adicionales (SVM, Neural Networks)
- [ ] Optimización de hiperparámetros con GridSearchCV
- [ ] Análisis de SHAP values para explicabilidad
- [ ] API REST para predicciones en tiempo real
- [ ] Dashboard interactivo con Streamlit
- [ ] Pipeline de ML con MLflow

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📝 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## 👨‍💻 Autor

**Leonardo Burbano**

- 🔗 Web: [https://leonardoburbano.com]
- 🔗 LinkedIn: [https://www.linkedin.com/in/leoburbano/]
- 🐙 GitHub: [https://github.com/leonardoburbanov]

---

⭐ Si este proyecto te resulta útil, ¡no olvides darle una estrella!
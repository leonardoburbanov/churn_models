# 📊 Modelos de Detección de Abandono de Clientes

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
- **Matplotlib** - Visualizaciones
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



## 📊 Datos

El proyecto utiliza el dataset `netflix_customer_churn.csv` que contiene:

- **Información demográfica** de los clientes
- **Datos de uso** del servicio
- **Métricas de facturación**
- **Variable objetivo**: Estado de abandono (Churn)

**Fuente de datos**: [Netflix Customer Churn Dataset](https://www.kaggle.com/datasets/abdulwadood11220/netflix-customer-churn-dataset) en Kaggle

## 📁 Estructura del Proyecto

```
churn_models/
├── input/
│   └── netflix_customer_churn.csv    # Dataset principal
├── netflix_churn_prediction.ipynb    # Notebook de análisis
├── pyproject.toml                    # Configuración del proyecto
├── uv.lock                          # Lock file de dependencias
└── README.md                        # Este archivo
```

## 🔬 Análisis Incluido

1. **Exploración de Datos**
   - Estadísticas descriptivas
   - Análisis de correlaciones
   - Visualizaciones de distribución

2. **Preprocesamiento**
   - Limpieza de datos
   - Codificación de variables categóricas
   - Escalado de features

3. **Modelado**
   - División train/test
   - Entrenamiento de múltiples algoritmos
   - Evaluación con métricas (Accuracy, Precision, Recall, F1)

4. **Optimización**
   - Ajuste de hiperparámetros
   - Selección del mejor modelo
   - Análisis de importancia de features

## 📈 Resultados

Los modelos implementados incluyen:
- **Random Forest**
- **Logistic Regression**
- **Support Vector Machine (SVM)**
- **Gradient Boosting**

Cada modelo es evaluado usando:
- Matriz de confusión
- Curva ROC
- Métricas de clasificación

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
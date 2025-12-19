# 🏦 Bank Customer Analytics & Prediction

Este proyecto realiza un análisis integral de datos para una entidad financiera ("Banco Monopoly"), abarcando desde la segmentación de clientes hasta la predicción de cupos de crédito y propensión digital.

### 🎯 Objetivo del Proyecto
Transformar más de **320 variables de comportamiento transaccional** en inteligencia de negocio accionable, permitiendo al banco personalizar sus estrategias de fidelización y riesgo.

### 🛠️ Tech Stack
- **Lenguaje:** Python 🐍
- **Análisis de Datos:** Pandas, NumPy
- **Machine Learning:** Scikit-learn (PCA, K-Means, DBSCAN, SVM, Random Forest, Regresión Ridge)
- **Visualización:** Matplotlib, Seaborn

---

### 📊 Metodología y Resultados

#### 1. Segmentación de Clientes (Clustering)
Se aplicaron técnicas de reducción de dimensionalidad y clustering para perfilar la cartera de clientes.
- **Técnica:** K-Means (k=5) validado contra DBSCAN y Clustering Jerárquico.
- **Hallazgo Clave:** Se identificaron **5 arquetipos de clientes**, desde el "Usuario de Crédito Integral" (alto valor) hasta el "Inactivo" (riesgo de fuga). Se descubrió que el comportamiento financiero es un continuo y no grupos aislados por densidad.

#### 2. Predicción de Cupo de Crédito (Regresión)
Desarrollo de modelos para estimar el cupo nacional (`CUPO_L1`).
- **Modelos:** Regresión Lineal Múltiple y Ridge.
- **Resultados:** El modelo explicó el **44% de la variabilidad** del cupo (R²=0.44).
- **Insight:** El cupo internacional (`CUPO_MX`) demostró ser el predictor más fuerte, superando a variables demográficas como la renta.

#### 3. Clasificación de Clientes Digitales (Internautas)
Predicción de si un cliente es usuario de banca digital (Internauta vs No Internauta).
- **Modelos:** Regresión Logística, SVM, Random Forest y Árboles de Decisión.
- **Resultados:** El modelo **SVM** alcanzó un Recall del **93%**, siendo ideal para detectar clientes digitales.
- **Insight:** La edad y la frecuencia de uso de cajeros automáticos (`FacDebAtm`) son los factores determinantes para la digitalización.

---

### 🚀 Cómo ejecutar este proyecto
1. Clonar el repositorio.
2. Instalar dependencias: `pip install -r requirements.txt`
3. Ejecutar el notebook en Jupyter o Google Colab.

---
*Proyecto desarrollado para la asignatura de Ciencia de Datos I.*

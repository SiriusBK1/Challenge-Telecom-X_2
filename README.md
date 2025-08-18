"""
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~ .oooooo..o  o8o            o8o                          oooooooooo.  oooo       ~
~d8P'    `Y8  `"'            `"'                          `888'   `Y8b `888       ~
~Y88bo.      oooo  oooo d8b oooo  oooo  oooo   .oooo.o     888     888  888  oooo ~
~ `"Y8888o.  `888  `888""8P `888  `888  `888  d88(  "8     888oooo888'  888 .8P'  ~
~     `"Y88b  888   888      888   888   888  `"Y88b.      888    `88b  888888.   ~
~oo     .d8P  888   888      888   888   888  o.  )88b     888    .88P  888 `88b. ~
~8""88888P'  o888o d888b    o888o  `V88V"V8P' 8""888P'    o888bood8P'  o888o o888o~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
"""

# Challenge-Telecom-X_2
Modelo predictivo capaz de prever qué clientes tengan mayor probabilidad de cancelar sus servicios.


> Proyecto de análisis de cancelación de clientes (churn) en una empresa de telecomunicaciones, utilizando técnicas de balanceo, escalado, y modelos predictivos como regresión logística y Random Forest.  
> Desarrollado por **Adrian** | Branding: **SiriusBk**

---

## Objetivo

Identificar patrones y variables clave que explican la cancelación de clientes en Telecom X, y construir modelos predictivos que permitan anticipar el churn con alta precisión. El análisis busca generar insights accionables para mejorar la retención de clientes.

---

## Metodología

1. **Carga y limpieza de datos**
   - Renombrado de columnas
   - Conversión de tipos
   - One-hot encoding para variables categóricas

2. **Preprocesamiento**
   - Separación de variables (`X`, `y`)
   - División en entrenamiento y prueba (`train_test_split`)
   - Balanceo de clases con **SMOTE**
   - Escalado de variables numéricas con `StandardScaler`

3. **Modelado**
   - Regresión Logística con `GridSearchCV` para optimización de hiperparámetros
   - Random Forest para análisis de importancia de variables

4. **Evaluación**
   - Métricas: Accuracy, Precision, Recall, F1-score, ROC-AUC
   - Visualizaciones: Matriz de confusión, curva ROC, curva Precision-Recall

5. **Interpretación**
   - Coeficientes de regresión logística
   - Importancia de características en Random Forest

---

## 📈 Resultados

| Modelo                        | Accuracy | F1-score | ROC-AUC |
|------------------------------|----------|----------|---------|
| Regresión Logística (Optim.) | 0.XX     | 0.XX     | 0.XX    |
| Random Forest                | 0.XX     | 0.XX     | 0.XX    |

> Las variables más influyentes incluyen `MonthlyCharges`, `Tenure`, y ciertos servicios contratados como `OnlineSecurity` y `TechSupport`.

---

## Recomendaciones

- **Segmentar clientes con alto riesgo de churn** según las variables más influyentes.
- **Ofrecer incentivos personalizados** para clientes con baja permanencia (`Tenure`) y altos cargos mensuales.
- **Mejorar servicios clave** como soporte técnico y seguridad online, que muestran fuerte correlación con retención.

---

## Tecnologías utilizadas

- Python (pandas, numpy, scikit-learn, imbalanced-learn)
- Visualización: matplotlib, seaborn
- Jupyter Notebook / Google Colab

---

## Cómo reproducir
1. Clona el repositorio:
   ```bash
   git clone https://github.com/SiriusBk/telecom-churn-analysis.git
   cd telecom-churn-analysis
2. 	Instala dependencias:
    pip install -r requirements.txt

3. 	Ejecuta el notebook:
   jupyter notebook Telecom_X_2.ipynb


Autor
Adrián — Estudiante de Data Science
🔗 GitHub: SiriusBk
📬 Contacto: aacevedovergara@gmail.com

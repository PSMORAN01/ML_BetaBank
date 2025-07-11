# Predicción de abandono de clientes en Beta Bank 🏦

Este proyecto busca predecir si un cliente abandonará el banco, basándonos en sus características y comportamiento anterior. Se utilizó aprendizaje supervisado para entrenar distintos modelos de clasificación.

---

## 📊 Descripción general

El problema viene de un banco llamado Beta Bank que quiere reducir la fuga de clientes (churn). Ya que atraer nuevos clientes es más caro que mantener los actuales, se necesita un modelo que prediga si un cliente va a irse o no.

Se usó un dataset realista con variables como edad, saldo, productos contratados, tarjeta de crédito, etc. La variable objetivo es `Exited`, que indica si el cliente se fue (`1`) o no (`0`).

---

## ⚙️ Tecnologías usadas

- Python 3
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Imbalanced-learn (SMOTE, RandomOverSampler)

---

## 🧪 Modelos utilizados

Probé varios modelos de clasificación:

1. **Regresión logística**
2. **Árbol de decisión**
3. **Random Forest**
4. **Pipelines con escalado + oversampling (SMOTE)**

Además, utilicé validación cruzada y optimización de hiperparámetros con `GridSearchCV`.

---

## 📈 Métricas

- Se optimizó la métrica **F1-score**, ya que el dataset está algo desbalanceado.
- También se midió **AUC-ROC** para comparar el rendimiento de los modelos.
- El modelo final logró un F1-score superior a 0.59, lo cual era el objetivo mínimo del proyecto.

---

## 🧼 Proceso general

1. Carga y revisión del dataset (`Churn.csv`)
2. Limpieza de datos e imputación de valores nulos (por ejemplo, `Tenure = 0`)
3. Análisis exploratorio con gráficas de distribución y correlaciones
4. Ingeniería básica de características
5. División en conjuntos de entrenamiento y prueba
6. Entrenamiento de varios modelos y comparación de métricas
7. Ajustes finales con oversampling y escalado

---

## 📌 Notas personales

Este proyecto me ayudó a entender mejor la diferencia entre accuracy y F1-score, especialmente en problemas con clases desbalanceadas. También aprendí a usar SMOTE para mejorar los resultados y a implementar pipelines más estructurados con `make_pipeline`.

---

## 👨‍💻 Autor

**Pablo Sebastián Morán**  
📧 psmoran01@gmail.com  
🔗 [GitHub](https://github.com/PSMORAN01)  
🔗 [LinkedIn](https://www.linkedin.com/in/tu-usuario) ← recuerda cambiarlo por el correcto

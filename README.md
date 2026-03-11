# 📡 Telecom X — Predicción de Cancelación de Clientes (Churn)

Proyecto de Machine Learning desarrollado como parte del programa **Oracle Next Education (ONE) — Alura LATAM**.

---

## 🎯 Objetivo

Construir modelos predictivos capaces de identificar qué clientes tienen mayor probabilidad de cancelar el servicio en Telecom X, a partir de un dataset de más de 7.000 registros.

La empresa busca anticiparse al problema de cancelación para tomar acciones de retención antes de que ocurra.

---

## 🗂️ Estructura del proyecto

```
telecomx-churn/
│
├── TelecomX_LATAM_.ipynb         # Parte 1 — Análisis exploratorio (ETL)
├── TelecomX_LATAM_Parte2.ipynb   # Parte 2 — Modelado predictivo (ML)
└── README.md
```

---

## 🧩 Metodología

### Parte 1 — Análisis Exploratorio
- Extracción de datos desde API en formato JSON
- Limpieza y transformación (ETL)
- Análisis de distribuciones y correlaciones
- Identificación de variables asociadas a la cancelación

### Parte 2 — Modelado Predictivo
1. **Preparación**: encoding, normalización y verificación del balance de clases
2. **Correlación**: matriz de correlación y análisis dirigido por variable
3. **Modelado**: entrenamiento de dos modelos de clasificación
4. **Evaluación**: métricas, matrices de confusión y análisis de overfitting
5. **Conclusiones**: importancia de variables e informe estratégico

---

## 🤖 Modelos utilizados

| Modelo | Requiere normalización | Características |
|---|---|---|
| Regresión Logística | Sí | Lineal, interpretable, buen Recall |
| Random Forest | No | Basado en árboles, robusto ante variables correlacionadas |

---

## 📊 Métricas de evaluación

- **Accuracy**: porcentaje de predicciones correctas en total
- **Precisión**: de los predichos como cancelación, cuántos realmente cancelaron
- **Recall**: de los que realmente cancelaron, cuántos detectó el modelo ← métrica principal
- **F1-score**: media armónica entre precisión y recall
- **Matriz de confusión**: visualización de errores por tipo

---

## 💡 Principales hallazgos

- El **tipo de contrato** es el factor con mayor impacto: los clientes con contrato mensual cancelan a una tasa significativamente mayor que los de contratos anuales o bianuales.
- La **antigüedad del cliente** es el factor protector más fuerte: a más meses de permanencia, menor probabilidad de cancelar. Los primeros 12 meses son el período crítico.
- El **método de pago** con cheque electrónico está fuertemente asociado a la cancelación.
- Los clientes con **fibra óptica** presentan una tasa de cancelación elevada a pesar de ser el servicio de mayor costo.
- La ausencia de **soporte técnico** incrementa significativamente la probabilidad de cancelación.

---

## 📋 Recomendaciones estratégicas

- Priorizar acciones de retención en los primeros 12 meses de contrato
- Incentivar la migración de contratos mensuales a anuales o bianuales
- Promover métodos de pago automáticos sobre el cheque electrónico
- Revisar la propuesta de valor del servicio de fibra óptica
- Incluir soporte técnico en más planes de servicio

---

## 🛠️ Tecnologías utilizadas

- Python 3
- Pandas / NumPy
- Matplotlib / Seaborn
- Scikit-learn
- Jupyter Notebook / Google Colab

---

## ▶️ Cómo ejecutar

1. Abrí el archivo `TelecomX_LATAM_Parte2.ipynb` en Google Colab o Jupyter Notebook
2. Ejecutá las celdas en orden de arriba hacia abajo
3. Los datos se cargan automáticamente desde la fuente original — no se necesita ningún archivo externo

---

## 👤 Autor

**maxhero3**
🔗 [github.com/maxhero3](https://github.com/maxhero3)

Proyecto desarrollado en el marco del programa Oracle Next Education (ONE) — Alura LATAM.

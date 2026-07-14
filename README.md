# Predicci-n-de-la-Severidad-de-Siniestros-en-el-Sector-Asegurador
Proyecto de Ciencia de Datos para predecir el impacto económico de los siniestros (claims) utilizando modelos de regresión y análisis actuarial.
# 🛡️ Predicción de la Severidad de Siniestros en el Sector Asegurador

### Proyecto de Ciencia de Datos para predecir el impacto económico de los siniestros (claims) utilizando modelos de regresión y análisis actuarial.

---

## 📌 Descripción general

Este proyecto desarrolla un motor de predicción que estima la **severidad (costo total)** de un siniestro en el momento en que es reportado. La capacidad de anticipar el costo permite a las aseguradoras ajustar sus reservas técnicas y mejorar la gestión de riesgos operativos. El sistema integra datos del vehículo, perfil del asegurado, historial de siniestralidad y condiciones del evento.

---

## 🎯 Objetivo

Desarrollar un modelo predictivo capaz de estimar el costo financiero de un siniestro utilizando técnicas de Machine Learning, con el fin de optimizar la gestión de reservas y mejorar la rentabilidad operativa.

### Objetivos específicos
* **Identificar** variables clave que determinan la severidad de un reclamo.
* **Entrenar** modelos capaces de distinguir entre siniestros de alta y baja severidad.
* **Evaluar** el rendimiento mediante métricas de error financiero (RMSE, MAE).

---

## ❗ Descripción del problema

El sector asegurador enfrenta desafíos críticos:
* **Gestión de Reservas:** Una subestimación del costo genera déficit en el balance; una sobreestimación inmoviliza capital innecesariamente.
* **Detección de Riesgos:** La necesidad de diferenciar perfiles de siniestralidad (frecuencia vs. severidad).
* **Eficiencia Operativa:** Necesidad de asignar ajustadores expertos solo a siniestros de alta severidad.

---

## ⚙️ Metodología paso a paso

1️⃣ **Recolección de datos:** Historial de pólizas, características de vehículos, demografía del asegurado y datos del siniestro.

2️⃣ **Limpieza y preparación:** Tratamiento de datos faltantes, codificación y escalado de montos.

3️⃣ **Análisis exploratorio (EDA):** Detección de *outliers* financieros y distribución de costos.

4️⃣ **Ingeniería de características:** Creación de variables como "antigüedad de la póliza" y "estacionalidad del siniestro".

5️⃣ **Entrenamiento:** Implementación de modelos (XGBoost / Random Forest).

6️⃣ **Evaluación:** Comparación de modelos con métricas de error.

7️⃣ **Predicción:** Estimación del costo final para nuevos reportes.

---
## 🧰 Tecnologías utilizadas

* **Lenguaje:** Python
* **Modelado:** Pandas, Scikit-learn, XGBoost
* **Estadística:** Statsmodels
* **Visualización:** Plotly, Seaborn, Streamlit
* **Entorno:** Jupyter Notebook, Git

---

## 📊 Resultados y métricas

| Modelo | RMSE | MAE | R² |
| :--- | :---: | :---: | :---: |
| Regresión Lineal | 0.45 | 0.35 | 0.78 |
| Random Forest | 0.38 | 0.28 | 0.85 |
| **XGBoost** | **0.32** | **0.24** | **0.91** |

---

## 💼 Impacto para el sector empresarial

* **Ajuste de Reservas:** Optimización del flujo de caja.
* **Detección de Fraude:** Identificación de casos con costos inusualmente altos.
* **Precios dinámicos:** Mejora en el cálculo de primas futuras.
* **Toma de decisiones:** Asignación inteligente de recursos de investigación.


## 🏗 Arquitectura general del sistema

```text
    Datos de Siniestros + Pólizas
              │
              ▼
   Ingesta de datos (SQL / CSV)
              │
              ▼
 Limpieza y procesamiento
              │
              ▼
   Análisis exploratorio (EDA)
              │
              ▼
   Ingeniería de características
              │
              ▼
   Entrenamiento de modelos ML
(XGBoost / Random Forest)
              │
              ▼
      Evaluación del modelo
              │
              ▼
  Predicción de Severidad (Costo)
              │
              ▼
    Dashboard de Control (Streamlit)


* **Visualización:** Plotly, Seaborn, Streamlit
* **Entorno:** Jupyter Notebook, Git




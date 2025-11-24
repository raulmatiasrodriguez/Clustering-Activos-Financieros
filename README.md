# 📊 Análisis Financiero y Modelado de Series Temporales con ARIMA

## Descripción del Proyecto
Este proyecto realiza un **análisis de activos financieros argentinos** (acciones cotizadas en Bolsa y tipo de cambio) desde 2023 hasta 2025, con el objetivo de:

- Evaluar la evolución histórica de los precios de cierre en USD.
- Calcular métricas financieras clave: retorno diario, volatilidad y momentum.
- Detectar y tratar **outliers** mediante z-score e IQR.
- Agrupar acciones en **clusters** para identificar perfiles de riesgo y potencial de crecimiento.
- Seleccionar acciones candidatas para análisis de series temporales y aplicar **modelos ARIMA** para predicción de precios.

El proyecto está desarrollado íntegramente en **Python**, utilizando librerías como `pandas`, `numpy`, `yfinance`, `matplotlib`, `seaborn` y `statsmodels`.

---

## Estructura del Repositorio

---


---

## Tecnologías y Librerías

- **Python 3.9+**
- `yfinance` → Descarga de datos financieros históricos.
- `pandas` & `numpy` → Manejo y transformación de datos.
- `matplotlib` & `seaborn` → Visualización de datos.
- `statsmodels` → Modelado de series temporales (ARIMA).
- `scikit-learn` → Normalización de datos y clustering (KMeans).

---

## Funcionalidades

### 1️⃣ Descarga y preparación de datos
- Descarga de precios de cierre de acciones y tipo de cambio ARS/USD.
- Conversión de precios a **dólares**.
- Limpieza de datos: eliminación de valores nulos y duplicados.

### 2️⃣ Cálculo de métricas financieras
- **Return**: Retorno diario porcentual.
- **Volatility**: Desviación estándar móvil (21 días).
- **Momentum**: Variación porcentual respecto a 21 días atrás.

### 3️⃣ Análisis exploratorio
- Histogramas, boxplots y matriz de correlación.
- Identificación y filtrado de outliers usando **z-score** e **IQR**.
- Comparación visual de datasets antes y después del tratamiento.

### 4️⃣ Clustering
- Normalización de métricas financieras.
- Agrupamiento con **K-Means**.
- Evaluación de número óptimo de clusters usando **Silhouette Score**.
- Visualización de centroides y perfiles de cada cluster.

### 5️⃣ Selección de acciones para ARIMA
- Priorización de acciones con menor volatilidad, mayor momentum y retorno positivo.
- Ejemplo: **PAMP_USD** seleccionada como acción candidata.

### 6️⃣ Modelado ARIMA
- Análisis de estacionariedad (ADF test) y diferenciación de series.
- Selección automática de parámetros ARIMA `(p,d,q)` basada en **AIC**.
- Ajuste del modelo y diagnóstico de residuos.
- Predicciones in-sample y out-of-sample.

---

## Visualizaciones
- Histogramas y boxplots de métricas financieras.
- Matrices de dispersión antes y después del tratamiento de outliers.
- Boxplots de métricas por cluster.
- Gráficos de centroides y cluster destacado.
- Series temporales reales vs predicciones ARIMA.

> Nota: Para no sobrecargar el repositorio, las imágenes generadas se incluyen en los **issues** del proyecto o se pueden generar directamente desde los notebooks.

---

## 

---

Autores






# 📊 Análisis y Perfilamiento de Acciones Argentinas con Clustering  

Este proyecto realiza un **análisis de activos financieros argentinos** (acciones cotizadas en Bolsa y tipo de cambio) desde 2023 hasta 2025, con el objetivo de:

- Evaluar la evolución histórica de los precios de cierre en USD.
- Calcular métricas financieras clave: retorno diario, volatilidad y momentum.
- Detectar y tratar **outliers** mediante z-score e IQR.
- Agrupar acciones en **clusters** para identificar perfiles de riesgo y potencial de crecimiento.
- Seleccionar acciones candidatas para análisis de series temporales y aplicar **modelos ARIMA** para predicción de precios.

El proyecto está desarrollado íntegramente en **Python**, utilizando librerías como `pandas`, `numpy`, `yfinance`, `matplotlib`, `seaborn` y `statsmodels`.

El análisis completo se encuentra en el notebook:

📄 `notebooks/tp_final_Grupo4.ipynb`

---
## 📁 Estructura del Repositorio

```text
Clustering-Activos-Financieros/  
│
├── notebooks/
│   └── tp_final_Grupo4.ipynb   # Notebook principal
│
└── README.md
```
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

<img width="637" height="528" alt="Matriz de Correlacion" src="https://github.com/user-attachments/assets/de00daac-05e2-4d1c-9115-441a8e746675" />        
    

<img width="986" height="1023" alt="Matriz de dispersión original" src="https://github.com/user-attachments/assets/c473b28d-201e-422c-810c-f6195afe973a" />  

<img width="985" height="1023" alt="Matriz de dispersión sin outliers" src="https://github.com/user-attachments/assets/b037f9a5-0c6b-4e04-a81a-7d779255b35c" />  


<img width="708" height="394" alt="Grafico de Silloute" src="https://github.com/user-attachments/assets/3f517b87-f098-4fbd-a28b-85c1ae836aef" />  

  
<img width="976" height="590" alt="Centroides de Clusters" src="https://github.com/user-attachments/assets/823153b7-b6d3-41dd-bba2-1ae17d0313d6" />  
  
 
<img width="1486" height="790" alt="Modelo ARIMA" src="https://github.com/user-attachments/assets/9b62dc03-c54e-48cd-b7ae-67d3670cae56" />  

> Nota: Para no sobrecargar el repositorio, las imágenes generadas se incluyen en los **issues** del proyecto o se pueden generar directamente desde los notebooks.

---

## 🎥 Video de demostración  

[![Ver video](https://img.youtube.com/vi/7tpNCkkmVM8/0.jpg)](https://youtu.be/7tpNCkkmVM8)  

> El video muestra la ejecución del proyecto y las visualizaciones generadas.  

---
## ✨ Autores

Este proyecto fue realizado en el marco de presentación de ultimo Trabajo Practico de la Materia Aprendizaje Autómatico de la Licenciatura en Ciencia de Datos.

- **Acevedo, David**  
- **Galeano, Mónica Inés**  
- **Rodriguez, Raúl Matías**

Año: 2025 — Universidad del Gran Rosario  






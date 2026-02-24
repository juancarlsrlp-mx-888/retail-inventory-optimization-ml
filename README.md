# 🚀 Optimización de Inventario y Predicción de Demanda con IA en Retail

## 📊 Resumen Ejecutivo
**El Desafío:** Las cadenas de *Fast Fashion* enfrentan altos costos por sobrestock y pérdida de ventas por quiebres de stock (*stockouts*). Los modelos tradicionales no capturan la volatilidad de la demanda moderna influenciada por el clima y tendencias.
**La Solución:** Un modelo predictivo end-to-end (XGBoost) que pronostica la demanda a nivel de tienda y SKU, acoplado a un sistema dinámico de alertas de inventario.
**El Impacto:** En una simulación de 7 días, el modelo identificó proactivamente 21,520 alertas de desabasto, previniendo un **riesgo de pérdida de ingresos de $44.3 Millones MXN**.

## 🛠 Stack Tecnológico
* **Lenguaje:** Python (Pandas, NumPy)
* **Machine Learning:** Scikit-Learn, XGBoost (Extreme Gradient Boosting)
* **Entorno:** Google Colab
* **Business Intelligence:** Looker Studio, Google Sheets

## ⚙️ Metodología del Proyecto
1. **Generación de Datos y Feature Engineering:** Procesamiento de +4.5 millones de registros. Se crearon variables de rezago (*lags*, *rolling windows*) y se integraron variables exógenas (clima, días festivos, tendencias virales).
2. **Modelado Predictivo:** Entrenamiento de un modelo `XGBRegressor` para capturar relaciones no lineales y elasticidad de precios.
3. **Lógica de Negocio:** Cálculo automatizado del *Punto de Reorden* basado en la volatilidad de la demanda y los tiempos de entrega (Lead Time) del proveedor.
4. **Despliegue Directivo:** Construcción de un dashboard operativo enfocado en la rentabilidad y acción inmediata.

## 📈 Visualización y Resultados

*(Nota: Aquí subes una captura de pantalla de tu dashboard en Looker Studio y la insertas en el README)*

## 📂 Estructura del Repositorio
* `01_Data_Generation.ipynb`: Script de generación de datos sintéticos hiperrealistas.
* `02_EDA_and_Feature_Engineering.ipynb`: Análisis exploratorio y creación de variables predictivas.
* `03_Demand_Forecasting_XGBoost.ipynb`: Entrenamiento del modelo y cálculo de impacto financiero.

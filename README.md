# 📊 Proyecto 8 | Validación de Hipótesis de Negocio con Pruebas Estadísticas (A/B Testing)

## 📌 Descripción

En este proyecto se analiza un **experimento A/B** realizado sobre la **landing page** de una empresa de e-commerce con el objetivo de determinar, mediante evidencia estadística, cuál versión de la página genera un mejor desempeño para el negocio.

El análisis se centra en responder preguntas relacionadas con:

* Incremento de la **tasa de conversión**.
* Diferencias en el **gasto promedio** de los usuarios convertidos.
* Influencia de la **fuente de tráfico** en la conversión.
* Influencia del **tipo de usuario** en la conversión.
* Generación de **insights ejecutivos** para apoyar la toma de decisiones.

---

# 🎯 Objetivos

* Validar la calidad del conjunto de datos.
* Aplicar pruebas estadísticas apropiadas para responder preguntas de negocio.
* Interpretar correctamente los resultados utilizando valores p.
* Identificar oportunidades de optimización para marketing y producto.
* Comunicar los resultados mediante visualizaciones e insights ejecutivos.

---

# 🗂 Dataset

El conjunto de datos contiene información de **40.000 usuarios** expuestos a un experimento A/B.

Cada registro representa un usuario que visualizó únicamente una versión de la página.

## Variables principales

| Variable         | Descripción                                          |
| ---------------- | ---------------------------------------------------- |
| `landing`        | Versión de la página (A o B)                         |
| `converted`      | Indica si el usuario realizó una compra              |
| `gasto`          | Valor gastado por el usuario (solo cuando convirtió) |
| `traffic_source` | Canal de adquisición                                 |
| `user_type`      | Usuario nuevo o recurrente                           |
| `region`         | Región geográfica                                    |
| `dispositivo`    | Desktop o Mobile                                     |

---

# 🛠 Herramientas utilizadas

* Python
* Pandas
* NumPy
* Matplotlib
* SciPy
* Statsmodels
* Jupyter Notebook

---

# 📈 Metodología

El proyecto se desarrolló siguiendo un flujo analítico orientado a negocio.

## 1️⃣ Exploración y validación de datos

* Revisión de estructura del dataset.
* Validación de tipos de datos.
* Identificación de valores faltantes.
* Estadísticos descriptivos.
* Identificación de valores atípicos mediante la regla del **IQR**.

---

## 2️⃣ Comparación del gasto promedio (Página A vs Página B)

Se comparó el gasto promedio de los usuarios convertidos utilizando una **prueba t para muestras independientes**.

**Hipótesis**

* H₀: El gasto promedio es igual entre las páginas A y B.
* H₁: El gasto promedio es diferente entre ambas páginas.

### Resultado

El análisis mostró una diferencia estadísticamente significativa (**p < 0.05**), indicando que una de las versiones genera un mayor valor económico por usuario convertido.

---

## 3️⃣ Comparación de la tasa de conversión

Se utilizó una **prueba Z para dos proporciones**.

**Hipótesis**

* H₀: Ambas páginas poseen la misma tasa de conversión.
* H₁: Las tasas de conversión son diferentes.

### Resultado

La página **B** presentó una tasa de conversión superior (**15.96%**) frente a la página **A** (**12.57%**), con una diferencia estadísticamente significativa.

---

## 4️⃣ Relación entre la fuente de tráfico y la conversión

Se aplicó una **prueba Chi-cuadrado de independencia**.

### Resultado

Se encontró una asociación estadísticamente significativa (**p = 0.034**) entre la fuente de tráfico y la conversión.

Las mayores tasas de conversión fueron:

* 📧 Email → **14.99%**
* 📢 Ads → **14.74%**
* 🤝 Referral → **13.88%**
* 🌱 Organic → **13.79%**

---

## 5️⃣ Relación entre el tipo de usuario y la conversión

Se aplicó nuevamente una prueba **Chi-cuadrado**.

### Resultado

No se encontró evidencia estadísticamente significativa (**p = 0.4736**) para afirmar que el tipo de usuario influya en la conversión.

Esto indica que las diferencias observadas entre usuarios nuevos y recurrentes pueden atribuirse al azar.

---

## 6️⃣ Visualización de resultados

Se construyeron gráficos para comparar:

* Conversión por fuente de tráfico.
* Conversión por tipo de usuario.
* Tasas de conversión.
* Distribución de usuarios convertidos.

Las visualizaciones respaldan los resultados obtenidos mediante las pruebas estadísticas.

---

# 📊 Principales hallazgos

✅ La **página B** genera una tasa de conversión significativamente mayor que la página A.

✅ Existe una diferencia significativa en el gasto promedio entre ambas versiones.

✅ **Email** y **Ads** son los canales con mejor desempeño en conversión.

✅ No existe evidencia suficiente para afirmar que el tipo de usuario influya en la conversión.

---

# 💼 Recomendaciones de negocio

* Implementar la **versión B** como landing principal.
* Priorizar campañas en **Email Marketing** y **Ads**.
* Continuar realizando pruebas A/B para optimizar la experiencia del usuario.
* No segmentar campañas únicamente por tipo de usuario, ya que no mostró un efecto estadísticamente significativo.

---

# 📚 Aprendizajes

Durante este proyecto reforcé conocimientos en:

* Estadística aplicada.
* Pruebas de hipótesis.
* A/B Testing.
* Interpretación de valores p.
* Visualización de datos.
* Storytelling con datos.
* Comunicación de resultados para stakeholders.

---

# 📁 Estructura del proyecto

```
Proyecto-8-A-B-Testing/
│
├── datasets/
│   └── landing_experiment.csv
│
├── notebooks/
│   └── Proyecto_8_AB_Testing.ipynb
│
├── images/
│
├── README.md
│
└── requirements.txt
```

---

# 🚀 Autor

**Jhon Fajardo**

Data Analyst | Python | SQL | Power BI | Estadística | Machine Learning

📧 [rofajhon@gmail.com](mailto:rofajhon@gmail.com)

🔗 LinkedIn: *(https://www.linkedin.com/in/jhon-fajardo-ingeniero-de-sistemas-data-analyst/)*

---

⭐ Si este proyecto fue útil o te gustó el análisis, no olvides darle una estrella al repositorio.

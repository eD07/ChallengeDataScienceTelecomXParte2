# 📊 Challenge Telecom X: análisis de evasión de clientes - Parte 2

## 📌 Descripción del Proyecto
Este proyecto tiene como objetivo predecir la cancelación de clientes (**churn**) en la empresa ficticia **TelecomX LATAM**, utilizando técnicas de Machine Learning aplicadas a un dataset realista del sector telecomunicaciones.

La problemática central es **identificar a los clientes con mayor probabilidad de cancelar su servicio**, con el fin de diseñar estrategias de retención efectivas.

---

## 🎯 Objetivos
- Analizar el comportamiento de los clientes para entender los factores de cancelación.
- Comparar distintos modelos de Machine Learning y evaluar su desempeño.
- Identificar las variables más influyentes en el churn.
- Proponer **estrategias de retención orientadas al negocio** basadas en los hallazgos.

---

## 🛠️ Metodología
El flujo de trabajo fue el siguiente:

1. **Análisis Exploratorio de Datos (EDA)**  
   - Estadísticas descriptivas.  
   - Visualización de variables categóricas y numéricas.  
   - Detección de outliers y valores nulos.  

2. **Preprocesamiento de Datos**  
   - Estandarización de variables numéricas.  
   - Codificación de variables categóricas.  
   - Balanceo de clases con técnicas de sobremuestreo.  

3. **Modelado Predictivo**  
   Se entrenaron y compararon los siguientes modelos:  
   - Regresión Logística  
   - K-Nearest Neighbors (KNN)  
   - Random Forest  
   - Support Vector Machine (SVM)  

4. **Evaluación de Modelos**  
   - Accuracy, Precision, Recall, F1-score.  
   - Matriz de confusión.  
   - Curva ROC-AUC.  

---

## 📈 Resultados y Hallazgos

### 🔑 Principales Factores de Cancelación
- Contratos de **corto plazo (Mes a Mes)**.  
- **Baja antigüedad** (clientes nuevos).  
- **Altos cargos mensuales** sin un valor agregado percibido.  
- **Métodos de pago inestables**, especialmente cheque electrónico.  
- Clientes con **pocos o demasiados servicios** contratados.  

### 📊 Importancia de Variables (por modelo)
- **Regresión Logística:** mostró que `Charges.Monthly` y `Cuentas_Diarias` aumentan el riesgo de cancelación, mientras que `Contract` a largo plazo reduce la probabilidad de churn.  
- **Random Forest:** identificó `Charges.Total`, `Charges.Monthly` y `tenure` como las variables más relevantes.  
- **KNN y SVM:** coincidieron en que el gasto mensual y la antigüedad son determinantes para la clasificación.  

---

## 💡 Conclusiones Orientadas al Negocio

- Los clientes con **contratos mes a mes** y **altos gastos mensuales** son los más propensos a cancelar.  
- Los clientes **nuevos** (tenure bajo) son especialmente vulnerables a churn en los primeros meses.  
- Los métodos de pago poco automatizados (ej: cheque electrónico) están asociados a una mayor inestabilidad.  

---

## 🚀 Estrategias de Retención Propuestas

1. **Incentivar Contratos a Largo Plazo**  
   - Ofrecer descuentos y beneficios exclusivos al migrar de mes a mes a contratos de 1 o 2 años.  
   - Programas de lealtad con recompensas por permanencia.  

2. **Mejorar la Experiencia de Clientes Nuevos**  
   - Programa de **onboarding proactivo** en los primeros 90 días.  
   - Atención técnica prioritaria para resolver problemas tempranos.  

3. **Optimizar Precios y Pagos**  
   - Diseñar **paquetes personalizados** que justifiquen cargos altos con valor agregado (streaming, datos extra).  
   - Incentivar métodos de pago automáticos (débito, tarjeta).  

---

## 📂 Estructura del Repositorio
```
├── telecomxparte2.py      # Script principal de análisis y modelos
├── data/                  # Dataset utilizado
├── notebooks/             # Notebooks de Colab
└── README.md              # Documentación del proyecto
```

---

## 👨‍💻 Autor
- Proyecto desarrollado como parte de la evaluación de **Estadísticas y Machine Learning**  
- Curso: Challenge Telecom X: análisis de evasión de clientes - Parte 2  
- Apoyo en bibliografía académica.  

**Autor:** *Edgardo Encina Pino*
- Repositorio base: https://github.com/eD07/ChallengeDataScienceTelecomXParte2
		    

---

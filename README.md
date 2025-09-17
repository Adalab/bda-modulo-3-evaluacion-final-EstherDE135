# ✈️ Proyecto de Análisis de Clientes de Aerolínea  

Este proyecto tiene como objetivo **explorar, limpiar y visualizar** datos provenientes de dos conjuntos principales relacionados con la actividad de clientes en una aerolínea:  

1. **Customer Flight Activity** → Información sobre vuelos reservados y realizados.  
2. **Customer Loyalty History** → Información sobre el historial de lealtad y membresías.  

Tras el preprocesamiento, ambos datasets se integran en un único DataFrame llamado **Clientes**, que nos permite realizar un análisis conjunto.  

---

## 📌 Objetivos del Proyecto  

- Identificar problemas en los datos (valores nulos, duplicados, outliers).  
- Limpiar y transformar columnas para facilitar el análisis (ej. meses de float → categorías con nombres).  
- Combinar la información de vuelos y lealtad en un solo dataset.  
- Realizar visualizaciones para responder preguntas de negocio como:  
  - ¿Cómo se distribuye la cantidad de vuelos reservados por mes durante el año?  
  - ¿Qué relación existe entre los años de inscripción y la actividad de vuelos?  
  - ¿Cuáles son los patrones de cancelación de clientes?  

---

## 🛠️ Tecnologías utilizadas  

- **Python 3.12.7**  
- **Pandas** para exploración y limpieza de datos  
- **NumPy** para manejo numérico  
- **Matplotlib** y **Seaborn** para visualización 
- **scipy.stats** para evaluación de la linealidad de las relaciones entre las variables y la distribución de las mismas
- **Jupyter Notebook** o **Visual Studio Code** para ejecución del análisis  

---

## 📂 Estructura del Proyecto  

├── Customer_Flight_Activity.csv
├── Customer_Loyalty_History.csv
├── Evaluacion_final_modulo_3.ipynb
├── README.md


---

## 🚀 Instrucciones de uso  

1. Clona este repositorio:  
   ```bash
   git clone https://github.com/Adalab/bda-modulo-3-evaluacion-final-EstherDE135.git
   cd bda-modulo-3-evaluacion-final-EstherDE135

2. Ejecuta el notebook principal en Jupyter o Visual Studio Code:
jupyter notebook notebooks/01_exploracion_inicial.ipynb

---
## 🔍 Flujo del análisis

1. Exploración inicial
- Uso de df.info(), df.describe(), df.isnull().sum() y visualizaciones básicas.
2. Limpieza de datos
- Conversión de columnas numéricas (Month, Enrollment_Month, Cancellation_Month) a categorías con nombres de meses.
- Sustitución de valores nulos (NaN → "Desconocido").
- Eliminación de duplicados en Loyalty_Number.
3. Unión de DataFrames
- Merge de Customer_Flight_Activity y Customer_Loyalty_History en Clientes mediante la columna Loyalty_Number.
4. Visualización y análisis
- Distribución de vuelos por mes.
- Patrones de cancelación.
- Relación entre variables de lealtad y actividad de vuelo.

## 📊 Ejemplo de visualización
import seaborn as sns
import matplotlib.pyplot as plt

sns.countplot(x="Month", data=Clientes, hue="Month", palette="viridis", legend=False)
plt.xticks(rotation=45)
plt.title("Distribución de vuelos reservados por mes")
plt.show()

## 👩‍💻 Autores
Esther Domínguez Escudero

## 📌 Estado del proyecto
🔧 En desarrollo: faltan fases adicionales de modelado y predicción, además de incorporar otras fuentes de datos externas.
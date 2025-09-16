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

- **Python 3.10+**  
- **Pandas** para exploración y limpieza de datos  
- **NumPy** para manejo numérico  
- **Matplotlib** y **Seaborn** para visualización  
- **Jupyter Notebook** o **Visual Studio Code** para ejecución del análisis  

---

## 📂 Estructura del Proyecto  

├── data/
│ ├── Customer_Flight_Activity.csv
│ ├── Customer_Loyalty_History.csv
│
├── notebooks/
│ ├── 01_exploracion_inicial.ipynb
│ ├── 02_limpieza_datos.ipynb
│ ├── 03_union_datasets.ipynb
│ ├── 04_visualizaciones.ipynb
│
├── src/
│ ├── utils.py # funciones auxiliares (ej. conversión de meses)
│
├── README.md


---

## 🚀 Instrucciones de uso  

1. Clona este repositorio:  
   ```bash
   git clone <url-del-repo>
   cd nombre-del-repo

2. Instala las dependencias necesarias: 
pip install -r requirements.txt

3. Ejecuta el notebook principal en Jupyter o Visual Studio Code:
jupyter notebook notebooks/01_exploracion_inicial.ipynb



# Trabajo Práctico - Asignatura 7
Modelado Predictivo con Machine Learning
Desarrollo de un modelo predictivo con base en wms_dataset_clean.xlsx

## Descripción
Este proyecto desarrolla un modelo de Machine Learning para predecir el estado operativo de activos en un sistema de gestión de inventario (WMS).

Las clases a predecir son:
- In Use
- In Storage
- Needs Repair

## Objetivo
-Construir un sistema de clasificación capaz de predecir el status operativo de los activos del
inventario (In Use, In Storage, Needs Repair) a partir de sus atributos descriptivos,
organizativos y logísticos, incorporando además un modelo ensemble y una segmentación no
supervisada para apoyar decisiones de gestión de almacén.

## Dataset
- Fuente: dataset interno del proyecto
- Registros utilizados: 797
- Variables: atributos logísticos, organizativos y descripción textual

## Metodología
- Preprocesamiento:
  - One-hot encoding
  - Escalado (StandardScaler)
  - TF-IDF en descripciones
- Modelos:
  - Dummy Classifier (baseline)
  - Regresión Logística
  - Random Forest
  - Support Vector Machine (modelo avanzado)
- Validación:
  - Train/test split (80/20)
  - Validación cruzada (5 folds)

## Resultados
El modelo Random Forest obtuvo el mejor desempeño:
- Accuracy: 0.94
- F1 macro: 0.93

## Análisis adicional
- Segmentación con K-means para identificar perfiles de inventario

## Cómo ejecutar

1. Ingresar o crear cuenta de google 
```bash
2.- Instalar google colaboratory 
3.-Abrir el notebook:
jupyter notebook
4.-copiar y cargar celdas del codigo en Asignatura7.ipynb dentro de google colaboratory
5.-copia ,pega y ejecuta cada una de las celdas
 
** Estructura del Proyecto**
data/: dataset utilizado
notebook/: desarrollo del modelo

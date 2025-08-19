- Análisis de la Tasa de Cancelación de Clientes (Churn Rate)

- Resumen ---------------------------------------------------------------------------------------------------------------

El proyecto trata del   análisis y la predicción de la tasa de cancelación (Churn Rate) de clientes. El objetivo principal fue desarrollar un modelo de Machine Learning capaz de identificar a los clientes que nos estan cancelando los pedidos. 
## Metodología

Como trabajamos este proyecto.

- 1 Preparación de Datos 

---División de Datos:-- El conjunto de datos se dividió en un 80% para entrenamiento y un 20% para prueba para una evaluación justa del rendimiento del modelo.
--Normalización:-- Se aplicó normalización a las variables numéricas para escalar los datos, un paso crucial para modelos sensibles a la escala como la Regresión Logística.

-- 2. Entrenamiento y Evaluación de Modelos

Se entrenaron y evaluaron dos modelos principales: --Regresión Logística-- y --Árbol de Decisión--.

--Regresión Logística:--
    --Rendimiento:-- En el ejercicio se  Logró una exactitud del 80%.
    --Justificación:-- Aca vemos que el modelo es  equilibrado, con una exactitud en entrenamiento (79%) y en prueba (80%) muy similar, lo que indica una buena capacidad de generalización y no presenta overfitting.

--Árbol de Decisión:
    --Rendimiento:-- Obtuvo una exactitud del 72% en los datos de prueba.
    --Justificación:-- El modelo mostró un claro **overfitting**, con una exactitud del 99% en entrenamiento pero una caída a 72% en prueba, lo que indica que memorizó los datos de entrenamiento y no generalizó bien. quizas debieramos seguir probando para verificar resultados

-- 3. Análisis de la Importancia de las Variables

Se analizaron las variables más influyentes en la cancelación para ambos modelos.

--Variables clave:** Tanto la Regresión Logística como el Árbol de Decisión coincidieron en que las variables relacionadas con el gasto del cliente (`Charges.Total`, `Charges.Monthly` y `Cuentas_Diarias`) y el tipo de contrato (`Contract`) son las más importantes para predecir el Churn.

-- 4. Conclusión y Estrategias Propuestas

El modelo final seleccionado fue la --Regresión Logística-- debido a su alto rendimiento y estabilidad.

Se propusieron estrategias de retención de clientes basadas en los hallazgos del modelo, tales como:
- Ofrecer valor agregado (ej. streaming o datos extra) a clientes con altos cargos mensuales para justificar el costo.
- Incentivar contratos a largo plazo, ya que están asociados con una menor probabilidad de cancelación.
- 



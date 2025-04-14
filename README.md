# trabajoFinal

•  Instalación de Dependencias: 
Al principio, se instalan las bibliotecas necesarias como gradio, seaborn, scikit-learn, y matplotlib para realizar visualizaciones y entrenar el modelo.
•  Carga y Preprocesamiento de los Datos: 
Se descarga un dataset sobre la esperanza de vida desde un repositorio de GitHub. Luego se limpian los nombres de las columnas para eliminar espacios innecesarios y se filtran las filas con valores nulos.
•  Modelo de Machine Learning - Random Forest:
Se define el modelo de Random Forest Regressor para predecir la esperanza de vida de un país, con las variables relevantes (como el Producto Interno Bruto (GDP), el nivel de escolaridad, el índice de masa corporal (BMI), etc.).
Se divide el dataset en un conjunto de entrenamiento y otro de prueba, y se realiza una búsqueda de los mejores hiperparámetros mediante GridSearchCV.
•  Evaluación del Modelo:
Se evalúa el modelo usando métricas como el MAE (Error Absoluto Medio), RMSE (Raíz del Error Cuadrático Medio) y R² para ver qué tan bien está funcionando el modelo de predicción.
•  Interfaz Gradio:
Se crea una interfaz de usuario interactiva usando Gradio para mostrar los gráficos generados.
Los usuarios pueden seleccionar un país y ver la predicción de la esperanza de vida usando el modelo, junto con un gráfico de la importancia de las características y una predicción futura para los próximos 25 años.
•  Gráficos de Comparativa Global:
Se generan gráficos que muestran los Top 10 países con mayor esperanza de vida y los Top 10 países con menor esperanza de vida usando seaborn.
•  Predicción por País:
Cuando un usuario selecciona un país, se realiza una predicción de la esperanza de vida para ese país usando el modelo ajustado. Además, se muestra un gráfico comparativo entre el valor real y el predicho, junto con la importancia de las características y la predicción futura.
•  Ejecutar la App Gradio: 
La app Gradio se lanza con la opción de compartirla públicamente, lo que permite interactuar con la visualización y las predicciones desde cualquier navegador.

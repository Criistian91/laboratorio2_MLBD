# laboratorio2_MLBD
Repositorio canciones Spotify
# DOCUMENTACIÓN CANCIONES SPOTIFY

## Introducción

Este código se ha desarrollado para abordar la evaluación y comparación de diversos modelos de clasificación en el contexto de nuestro proyecto de clasificación binaria. El objetivo principal es seleccionar un modelo óptimo que pueda predecir con precisión un resultado binario en nuestros datos. La selección del modelo adecuado es crucial para el éxito de nuestro proyecto.

##Estructura del Código
A continuación, describiremos las distintas secciones de código y explicaremos las razones detrás de nuestras elecciones:

A). Importación de Bibliotecas y Datos:
En esta sección, importamos las bibliotecas necesarias y cargamos nuestros datos. Las bibliotecas, como scikit-learn, xg boost, matplotlib y numpy, proporcionan herramientas esenciales para la evaluación y visualización de modelos. La elección de estas bibliotecas se basa en su amplia adopción y su capacidad para abordar tareas de aprendizaje automático de forma eficaz.

B). Preprocesamiento de Datos:
El preprocesamiento de datos es un paso crítico para garantizar la calidad de los resultados. En esta sección, dividimos nuestros datos en conjuntos de entrenamiento y prueba, normalizamos características y codificamos etiquetas. Estas técnicas son fundamentales para evitar el sobreajuste y garantizar que los modelos sean capaces de generalizar a nuevos datos.

C). Evaluación de Modelos Individuales:
Seleccionamos varios modelos de clasificación, como SVM con kernel RBF, Árbol de Decisión, Naive Bayes (MultinomialNB), Regresión Logística y XG Boost. La elección de estos modelos se basa en su idoneidad para problemas de clasificación y su capacidad para capturar patrones en los datos.
Cada modelo se entrena y evalúa en el conjunto de prueba, y se calculan métricas como la matriz de confusión, la curva ROC, la precisión, el recall y el F1-score. Estas métricas se seleccionaron porque proporcionan una visión completa del rendimiento de los modelos en el contexto de nuestro proyecto.

D). Búsqueda en Cuadrícula (Grid Search):
Aplicamos la búsqueda en cuadrícula para ajustar los hiper parámetros de ciertos modelos, como la Regresión Logística y XG Boost. La optimización de hiper parámetros es esencial para maximizar el rendimiento de los modelos. Elegimos estos modelos específicos debido a su flexibilidad y capacidad para mejorar el rendimiento mediante ajustes precisos.

E). Ensamble de Modelos:
Creamos un ensamble de modelos base, incluyendo SVM con kernel RBF, Árbol de Decisión y XG Boost, mediante el enfoque de votación de la mayoría. La relevancia de este paso radica en la mejora de la robustez y la precisión general al combinar múltiples modelos.

F). Visualización de Resultados:
Visualizamos los resultados utilizando mapas de calor para las matrices de confusión y curvas ROC. Esto permite una comprensión más fácil de las fortalezas y debilidades de los modelos. La elección de estas visualizaciones se basa en su capacidad para comunicar de manera efectiva la información de evaluación.

-----------------------------------------------------------------------------

Durante el desarrollo de este código, se enfrentaron algunos desafíos y consideraciones

Selección de modelos: Elegir los modelos adecuados para nuestro proyecto fue un desafío clave. Optamos por modelos ampliamente utilizados en problemas de clasificación debido a su robustez y flexibilidad.

Limpieza de datos: Durante el proceso, se optó por una limpieza de datos exhaustiva para optimizar los resultados. Esta decisión puede haber reducido ligeramente la precisión, pero aumentó la confiabilidad de los resultados. Antes de esta operación, la mayoría de los modelos arrojan resultados buenos o engañosamente altos, lo que podría haber sido el resultado de datos ruidosos o inconsistentes. La limpieza de datos garantizó que los modelos se entrenan y evaluaran en datos de alta calidad, lo que es fundamental para la confiabilidad y aplicabilidad de nuestro proyecto.
Ajuste de hiper parámetros: Ajustar los hiper parámetros de ciertos modelos puede ser complejo. La búsqueda en cuadrícula nos ayudó a abordar este desafío y encontrar los valores óptimos.
Evaluación de resultados: Interpretar las métricas y visualizaciones para tomar decisiones informadas requería tiempo y análisis cuidadoso.

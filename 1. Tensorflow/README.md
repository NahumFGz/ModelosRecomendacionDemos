# Tensorflow for recsys

- Tutoriales disponibles en https://www.tensorflow.org/recommenders/examples/basic_retrieval  

# Los sistemas de recomendación del mundo real a menudo se componen de dos etapas:
1. **La etapa de la recuperación**  
    - Es responsable de selecciona un conjunto inicial de cientos de candidatos entre todos los posibles candidatos.  
    - El objetivo principal de este modelo es eliminar de manera eficiente a todos los candidatos que no le interesen al usuario.  
    - Dado que el modelo de recuperación puede estar tratando con millondes de candidatos, tiene que ser computacionalmente eficiente.  
  
2. **La etapa de clasificación**  
    - Toma los resultados del modelo de recuperación y los ajusta para  seleccionar el mejor puñado de recomendaciones posibles.  
    - Su tarea es reducir el conjunto de elementos que le pueden interesar al usuario a una lista corta de posibles candidatos.  


## Los modelos de recuperación a menudo se componen de dos submodelos:
1. **Un modelo de consulta**
    - Calcula la representación de la consulta (normalmente un vector de incorporación de dimensionalidad fija) mediante funciones de consulta.  
  
2. **Un modelo candidato**
    - Que calcula la representación candidata (un vector de igual tamaño) utilizando las mismas caracteriticas candidatas.


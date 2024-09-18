# Laboratorio 2 - Agrupación - Clustering

[Objetivos](#objetivos)

[Herramientas](#herramientas)

[Enunciado](#enunciado)

[Entregables](#entregables)

[Rúbrica de clasificación](#rubrica)

[Sugerencias y aclaraciones](#sugerencias)

## <a name="objetivos"></a> Objetivos

- Aplicar el proceso de aprendizaje para resolver una tarea de agrupación, desde la preparación de los datos hasta la interpretación de los resultados. 
- Aplicar y comparar tres algoritmos de clústering (k-means y dos de libre elección) para resolver el objetivo de la organización. 
- Derivar y comunicar conclusiones a partir de los mejores grupos identificados, que sean útiles para la organización.


## <a name="herramientas"></a> Herramientas

Durante este laboratorio trabajaremos con las siguientes herramientas:

 - Python
	 - Distribución sugerida: [Anaconda](https://www.continuum.io/downloads) 
		 - La versión de Anaconda es 4.4
		 - La versión usada es la de python 2.7, usar python 3 no debería requerir muchos cambios.
	 - Ambiente de desarrollo
	   	 - JupyterLab
	   	 - Google Colab
	 - Librerías
	 	 - Pandas
		 - Scikit-learn
		 - Matplot
		 - Seaborn 

## <a name="enunciado"></a> Enunciado

### Descripción del problema

La técnica de agrupación, o clústering, es un método de aprendizaje no supervisado cuyo objetivo es organizar un conjunto de datos en grupos con base en la similitud de sus características. Esta técnica permite descubrir patrones y estructuras subyacentes en los datos sin necesidad de etiquetas predefinidas para cada instancia.  
MediAlpes, EPS cuyo objetivo de negocio es incorporar herramientas de Inteligencia Artificial para incrementar la eficiencia de la prestación de servicios a los usuarios en las diferentes IPS asociadas, considera que, en el contexto del triage, la agrupación puede ser útil para la toma de decisiones. Al analizar las características de los pacientes que llegan a Urgencias, es posible identificar y analizar tendencias en los tipos de emergencias más frecuentes. Esto facilita la optimización de los protocolos de atención y los tiempos de respuesta según los patrones detectados. Además, permite desarrollar programas de prevención y educación dirigidos a las características predominantes de los pacientes en cada grupo, así como mejorar la planificación de recursos y la asignación de personal para manejar los flujos de pacientes de manera más eficiente y reducir los tiempos de espera en urgencias.  
Dado el éxito de la primera etapa del proyecto relacionado con la mejora de los procesos de asignación de recursos para la atención a pacientes que ingresen por Urgencias, MediAlpes ha solicitado a su equipo de Científicos de Datos para que evalúe la factibilidad de aplicar técnicas de agrupación sobre la información de pacientes que se suministró, para identificar patrones y características comunes que pueden utilizarse para optimizar la toma de decisiones y mejorar la eficiencia en la atención médica.


* [Datos de entrenamiento](202420/Laboratorio 2 - Agrupación/202420_Laboratorio_2_-_Agrupación_data.csv)
* [Diccionario de datos](202420/Laboratorio 2 - Agrupación/202420_Laboratorio_2_-_Agrupación_diccionario_de_datos.xlsx)


### Instrucciones 

MediAlpes desea que usted los apoye en la construcción del modelo de agrupación previamente descrito utilizando algunas de las etapas de la metodología "ASUM-DM":

1. **Preparación de datos:** Realizar la preparación de los datos con base en las características de los algoritmos de agrupación a emplear. Aunque los datos que se utilizarán son los mismos de la primera etapa del proyecto (Laboratorio 1), es recomendable revisar el proceso de exploración y limpieza de los datos.

3. **Modelamiento:** Aplicar el algoritmo K-Means y otros dos algorimos para construir tres modelos de agrupación. Tengan en cuenta que, en ambientes profesionales, la elección y justificación del algoritmo y sus hiperparámetros hace parte de su tarea de consultoría.

4. **Validación cuantitativa:** Comparar los resultados de los tres algoritmos aplicados desde el punto de vista cuantitativo puede validarse utilizando diferentes métricas intrínsecas, como el coeficiente de silueta.
En caso de contar con datos anotados es posible también realizar una validación externa. Información adicional para complementar su interpretación puede encontrarla en este [enlace](https://towardsdatascience.com/k-means-clustering-algorithm-applications-evaluation-methods-and-drawbacks-aa03e644b48a). 
    
5. **Validación cualitativa:** Una vez realizada la validación cuantitativa, comparar la validación cualitativa de los tres algoritmos aplicados. Esto significa que debe hacer una descripción de los grupos obtenidos y relacionarlo con el objetivo que tiene la organización para determinar si es posible utilizar el resultado obtenido, o hay que seguir trabajando en alguna dirección específica para la comprensión por parte de la organización.

6. **Visualización:** El grupo debe proponer una visualización de los resultados obtenidos en un tablero de control, para que MediAlpes tenga la capacidad de entender estos resultados en su labor de consultoría.

## <a name="entregables"></a> Entregables
- Informe, que puede ser el mismo cuaderno, el cual debe incluir:
    - Descripción detallada de cada etapa según las instrucciones dadas previamente
    - Describir cada algoritmo aplicado e indicar el nombre del estudiante responsable de esta tarea.
    - Determinar y describir los hiperparámetros obtenidos para aplicar los algorimos.
    - Construir una tabla comparativa que muestre el rendimiento de los tres algoritmos de agrupación aplicados. 
    - Comunicar los hallazgos encontrados a la organización, explicando por qué tienen valor para el negocio. Esto aplica para el algoritmo que considere es el que mejor resultado desde el punto de vista cualitativo y cuantitativo. 
- Tablero de control construido.
- Presentación con los resultados. La presentación debe estar orientada a la organización, por lo que se recomienda evitar el uso de términos muy técnicos y utilizar un lenguaje que sea familiar en el contexto de aplicación. Se les sugiere centrarse en la interpretación de los resultados visualizados en el tablero de control construido.
- Cuaderno ejecutado.

    
Algunas preguntas que pueden guiar su desarrollo son: 

1. ¿Qué criterios son importantes para la selección del modelo? 

2. ¿Cómo medir la calidad del modelo construido? ¿Cómo saber que el modelo construido tiene una buena calidad?  

3. ¿Qué retos tienen estos modelos no supervisados, si se quisieran aplicar a nivel profesional?

4. ¿Cómo varía la calidad del modelo obtenido si se aplican diferentes algoritmos?

5. ¿Qué pasa en la ejecución de los algortimos si se incluyen variables categóricas nominales. ¿Qué tratamiento se les debe aplicar? 




## Instrucciones de Entrega
- El laboratorio se entrega en grupos de mínimo 2 y máximo 3 estudiantes. Estos estudiantes pueden ser de diferentes secciones.
- Recuerde hacer la entrega por la sección unificada en Bloque Neón, antes del sábado 21 de septiembre a las 20:00.   
  Ese será el único medio por el cual se reciben entregas. Verifique que la entrega realizada es la correcta.

## <a name="rubrica"></a> Rúbrica de Calificación

A continuación se encuentra la rúbrica de calificación.

**Nota:** Los siguientes porcentajes hacen referencia a la nota grupal, que corresponde a un 80% de la nota inidividual.  
El 20% restante se calcula según el puntaje obtenido en la implementación del algoritmo del cual el estudiante estuvo a cargo dentro del grupo.

| Concepto | Porcentaje |
|:---:|:---:|
| Descripción del proceso de preparación de datos realizado, el genérico y el relacionado con el algoritmo utilizado. Justitificar utilizando el entendimiento de los datos | 15% |
| Implementación de K-means, descripción de las decisiones más importantes asociadas a la implementación del algoritmo y los hiperparámetros configurados | 10% |
| Implementación de un segundo algoritmo de libre elección, descripción corta del algoritmo y de las decisiones más importantes asociadas a la implementación y los hiperparámetros configurados | 10% |
| Implementación de un tercer algoritmo de libre elección, descripción corta del algoritmo y de las decisiones más importantes asociadas a la implementación y los hiperparametros configurados | 10% |
| Análisis de los resultados obtenidos y justificación del modelo recomendado para el caso propuesto | 25% |
| Presentación para la organización con resultados, recomendaciones y visualización usando el tablero de control construido| 25% |
| Cuaderno asociado, ejecutado | 5% |

## <a name="sugerencias"></a> Sugerencias y aclaraciones

 - Nota 1: la interpretación de los grupos se debe hacer en términos de las variables que considere importantes (incluya las usadas para la construcción de los clusters
 pero también otras variables, que no hayan incluido)
 - Nota 2: Analizar si los valores de cada columna corresponden a valores adecuados para el negocio, en caso de que no lo sean, deben tratar dichos valores y justificar sus decisiones.

Los siguientes enlaces pueden serle de utilidad para la implementación en Python. 

* [Ejemplo de K-Means usando Sklearn](https://jakevdp.github.io/PythonDataScienceHandbook/05.11-k-means.html)

* [Artículo de Towards Data Science: K-means with Sklearn](https://towardsdatascience.com/k-means-clustering-with-scikit-learn-6b47a369a83c)

* [Artículo de Towards Data Science: Introducción al análisis de datos con Python](https://towardsdatascience.com/tips-and-tricks-for-fast-data-analysis-in-python-f108ad32fa90) 

* [Artículo de Towards Data Science: Best Practices for Visualizing Your Cluster Results](https://towardsdatascience.com/best-practices-for-visualizing-your-cluster-results-20a3baac7426) 

 - Cada integrante del grupo debe estar encargado de la implementación de un algoritmo distinto. Sin embargo, todos los integrantes del grupo
deben tener la capacidad de explicar lo realizado por los demás compañeros
 - El análisis de resultados y su justificación debe ser realizado en grupo.


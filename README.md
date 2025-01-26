# Taller de Algoritmos Genéticos

### Presentado por:
- **Ángel Rivera Amortegui**
- **Daniel Echeverry Jimenez**

---

## **Punto 1: Matriz de poder para repartir el poder usando AGs.**
Archivo: [AlgGen_poderPolitico.ipynb](./AlgGen_poderPolitico.ipynb)
[AlgGen_PyGad.ipynb](./AlgGen_PyGad.ipynb) 
Descripción: Este código implementa un algoritmo genético para resolver un problema de asignación de curules a partidos políticos basado en el peso político de diferentes entidades. El objetivo es asignar entidades a los partidos de manera que se respeten las restricciones de curules disponibles para cada partido, maximizando el puntaje obtenido de acuerdo al peso político de las entidades. A continuación se realizar una breve explicación del código.
- Generación de cromosomas: Se crean soluciones aleatorias donde cada bit indica la asignación de una entidad a un partido.
- Evaluación: Se calcula un puntaje de aptitud según si las asignaciones respetan las restricciones de curules y el peso político de las entidades.
- Selección de padres: Los cromosomas con mejores puntajes tienen más probabilidad de ser seleccionados para la siguiente generación.
- Cruce y mutación: Se combinan los cromosomas de los padres para generar nuevos, con algunas mutaciones aleatorias para evitar soluciones subóptimas.
- Iteración: El proceso se repite durante un número de iteraciones, imprimiendo los resultados al final. Con este enfoque busca encontrar la mejor asignación de entidades a partidos de manera eficiente, respetando las restricciones impuestas.

## **Punto 2: Usar un AGs en un despacho de energía para minimizar los costos de transporte y generación de energía**
Archivo: [3_2_Energía_eléctrica.ipynb](./3_2_Energía_eléctrica.ipynb)  
Descripción:Este código resuelve un problema de optimización lineal utilizando la librería pulp, donde se busca minimizar los costos de transporte y generación de energía entre varias plantas y ciudades. Define las cantidades disponibles de energía en cada planta, la demanda de energía en cada ciudad, y los costos asociados tanto al transporte como a la generación. Las variables de decisión representan la cantidad de energía transportada entre cada planta y ciudad. Luego, establece restricciones de oferta y demanda, y resuelve el problema. Finalmente, muestra una tabla con los resultados, detallando los costos de transporte, generación y el costo total del suministro.

## **Punto 3: Solución de un TSP (Traveling Salesman Problem), el problema de un viajero en Colombia:**
Archivo: [El_problema_del_viajero_en_ciudades_de_Colombia.ipynb](./El_problema_del_viajero_en_ciudades_de_Colombia.ipynb)  
Descripción: Este código implementa un algoritmo genético para resolver el problema del Viajante de Comercio (TSP) utilizando un conjunto de ciudades colombianas y sus coordenadas geográficas. El algoritmo comienza creando una población inicial de rutas aleatorias entre las ciudades. A continuación, evalúa el "fitness" de cada ruta, que se define como la distancia total recorrida, e implementa la selección por torneo para elegir a los mejores individuos. Posteriormente, se aplica el cruce para generar nuevas rutas (descendencia) y una mutación para introducir variabilidad. El proceso se repite durante un número determinado de generaciones para optimizar la ruta y encontrar la mejor solución posible en términos de distancia total recorrida. Finalmente, el código devuelve la mejor ruta encontrada y su distancia total.

## **Punto 4: Generación aleatoria para una población de 50 palabras **
Archivo: [3_4_50_palabras.ipynb](./3_4_50_palabras.ipynb)  
Descripción: Este código implementa un algoritmo genético para encontrar una palabra objetivo (en este caso, "GENETICA") mediante un proceso de evolución simulada. Inicia generando una población aleatoria de palabras y luego evalúa qué tan cerca están de la palabra objetivo usando una función de aptitud. La aptitud se mide por la cantidad de caracteres coincidentes entre una palabra de la población y la palabra objetivo. Posteriormente, los individuos más aptos se seleccionan para cruzarse y producir descendencia, aplicando mutaciones aleatorias a cada generación. El proceso continúa hasta encontrar la palabra objetivo o alcanzar el número máximo de generaciones.

## **Punto 5: Un AGs para una máquina despulpadora de café (Punto de investigación adicional)**
Archivo: -[AGS_máquina_despulpadora_de_café.ipynb](./AGS_máquina_despulpadora_de_café.ipynb)
Descripción: Este código implementa un algoritmo genético (AG) para optimizar la velocidad de una máquina en función de dos factores: la eficiencia y los defectos. La eficiencia sigue una curva tipo campana centrada en 200 RPM, mientras que los defectos aumentan linealmente con la velocidad. El AG evoluciona una población de posibles soluciones (velocidades) a lo largo de varias generaciones, seleccionando los mejores individuos, cruzándolos para generar nuevos, y aplicando mutaciones aleatorias para explorar soluciones adicionales. Al final, el algoritmo muestra la velocidad óptima encontrada para maximizar la eficiencia mientras minimiza los defectos, dentro de un rango de 50 a 300 RPM.


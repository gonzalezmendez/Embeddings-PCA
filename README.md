# Embeddings y PCA

### Conceptos:
Los embeddings son representaciones vectoriales de datos, como palabras o frases, en un espacio numérico de alta dimensión; permiten medir relaciones semánticas entre objetos, lo que significa que cosas similares se representan con vectores cercanos entre sí. Por ejemplo, "gato" y "perro" estarán cerca en el espacio vectorial, mientras que "gato" y "avión" estarán muy lejos. 

La PCA (Principal Component Analysis) es una técnica de análisis de datos que reduce la dimensionalidad de un conjunto de datos al transformar los datos en un espacio de dimensiones más bajas, manteniendo la mayor cantidad de variabilidad posible. Esto se logra al seleccionar las componentes principales que representan la mayor parte de la variabilidad en el conjunto de datos.

---
### Aplicados en la comparación de textos (Leyes de la fisica)

Los embeddings y la PCA son herramientas fundamentales en el procesamiento del lenguaje natural y la inteligencia artificial, permitiendo a los modelos de aprendizaje automático entender y procesar el lenguaje humano de manera más efectiva.

Este proyecto utiliza leyes fundamentales de la física como punto de partida para analizar cómo distintos niveles de abstracción influyen en los resultados de Machine Learning, específicamente en la generación y análisis de embeddings.

Las leyes físicas (por ejemplo, las leyes de Newton, la gravedad, la conservación de la energía o la termodinámica) se representan como descripciones textuales que, aunque pertenecen a un dominio altamente estructurado, presentan distintos grados de complejidad conceptual.

Estas descripciones se transforman en embeddings y posteriormente se analizan mediante Análisis de Componentes Principales (PCA) para observar cómo el modelo captura similitudes, relaciones y estructuras latentes.

## Saber que modelo de ML elegir.
| MODELO | IDIOMAS |  PRECISION | VELOCIDAD | USO TIPICO |
| :-- | :-- | :-- | :-- |:-- |
| all-MiniLM-L6-v2 | Principalmente inglés | Buena | Muy Rapido | Búsqueda semántica general |
| paraphrase-multilingual-MiniLM-L12-v2 | Multilenguaje | Alta | Lento | Similaridad semántica multilingüe|

## Modelo all-MiniLM-L6-v2
  * Tiende a la "homogeneización". Al forzar a todos a medir 1.0, reduce la jerarquía entre los conceptos.
  * Es útil para comparaciones rápidas de "a qué se parece esto", pero pierde el matiz de la importancia relativa.

[Codigo completo usando modelo all-MiniLM-L6-v2](https://github.com/gonzalezmendez/Embeddings-PCA/blob/img/L6.png)
![Texto alternativo](https://github.com/gonzalezmendez/Embeddings-PCA/blob/img/L6B.png)
---
## Modelo paraphrase-multilingual-MiniLM-L12-v2
  * Es más robusto. Al permitir que los vectores crezcan en magnitud, está capturando una dimensionalidad más rica del texto complejo.
  * Refleja mejor las distancias reales entre conceptos físicos distintos (no es lo mismo la inercia que la gravedad).

[Codigo completo usando el modelo paraphrase-multilingual-MiniLM-L12-v2](https://github.com/gonzalezmendez/Embeddings-PCA/blob/img/L12.png))
![Texto alternativo](https://github.com/gonzalezmendez/Embeddings-PCA/blob/img/L12B.png)

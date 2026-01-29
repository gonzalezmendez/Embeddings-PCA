# NLP – Natural Language Processing (procesamiento de lenguaje natural)
### _Generación de embeddings vectoriales de texto y aplicación de PCA para reducción de dimensionalidad y comparación semántica._

Los embeddings y la PCA son herramientas fundamentales en el procesamiento del lenguaje natural y la inteligencia artificial, permitiendo a los modelos de aprendizaje automático entender y procesar el lenguaje humano de manera más efectiva.

Este proyecto utiliza leyes fundamentales de la física como punto de partida para analizar cómo distintos niveles de abstracción influyen en los resultados de Machine Learning, específicamente en la generación y análisis de embeddings.

Las leyes físicas (por ejemplo, las leyes de Newton, la gravedad, la conservación de la energía o la termodinámica) se representan como descripciones textuales que, aunque pertenecen a un dominio altamente estructurado, presentan distintos grados de complejidad conceptual.

Estas descripciones se transforman en embeddings y posteriormente se analizan mediante Análisis de Componentes Principales (PCA) para observar cómo el modelo captura similitudes, relaciones y estructuras latentes.

### Librerias:
`pip install sentence-transformers`
`pip install scikit-learn`
`pip install pandas`
`pip install numpy`
`pip install plotly`

### Saber que modelo de ML elegir.
| MODELO | IDIOMAS |  PRECISION | VELOCIDAD | USO TIPICO |
| :-- | :-- | :-- | :-- |:-- |
| all-MiniLM-L6-v2 | Principalmente inglés | Buena | Muy Rapido | Búsqueda semántica general |
| paraphrase-multilingual-MiniLM-L12-v2 | Multilenguaje | Alta | Lento | Similaridad semántica multilingüe|

### Modelo all-MiniLM-L6-v2
  * Tiende a la "homogeneización". Al forzar a todos a medir 1.0, reduce la jerarquía entre los conceptos.
  * Es útil para comparaciones rápidas de "a qué se parece esto", pero pierde el matiz de la importancia relativa.

|[Codigo modelo all-MiniLM-L6-v2](https://github.com/gonzalezmendez/NLP/blob/txt/L6.txt)|[Imagen del codigo](https://github.com/gonzalezmendez/NLP/blob/img/L6.png)|
|:--|--:|

![L6](https://github.com/gonzalezmendez/NLP/blob/img/L6B.png)
---
### Modelo paraphrase-multilingual-MiniLM-L12-v2
  * Es más robusto. Al permitir que los vectores crezcan en magnitud, está capturando una dimensionalidad más rica del texto complejo.
  * Refleja mejor las distancias reales entre conceptos físicos distintos (no es lo mismo la inercia que la gravedad).

|[Codigo modelo paraphrase-multilingual-MiniLM-L12-v2](https://github.com/gonzalezmendez/NLP/blob/txt/L12.txt)|[Imagen del codigo](https://github.com/gonzalezmendez/NLP/blob/img/L12.png)|
|:--|--:|

![L12](https://github.com/gonzalezmendez/NLP/blob/img/L12B.png)

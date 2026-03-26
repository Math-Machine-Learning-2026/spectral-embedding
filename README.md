# Spectral embedding para la descripción de imágenes

## Integrantes del grupo
- Hannah Macadam
- Pablo Pérez
- Ane Redondo
- David Valenzuela

## Descripción del proyecto
En este trabajo estudiamos el algoritmo **spectral embedding** como técnica de reducción de la dimensionalidad no lineal sobre el dataset **Fashion MNIST**, con el objetivo de representar imágenes de prendas de ropa en una variedad de menor dimensión preservando, en la medida de lo posible, la estructura local de los datos.

Trabajamos con un subconjunto de 12.000 imágenes del dataset original. Éstas tienen un tamaño de 28×28 píxeles en escala de grises, y llevan asignadas una de las 10 etiquetas posibles según el tipo de prenda que representen (pantalones, abrigos, camisetas, etc). Una especificación más detallada de los datos se puede encontrar en el repositorio de Github oficial de [Fashion MNIST](https://github.com/zalandoresearch/fashion-mnist).

Los principales objetivos que abordamos son:
- la preparación y visualización de los datos,
- la construcción de grafos de vecindad sobre las imágenes,
- la elección de hiperparámetros relevantes,
- la comparación de distintas matrices de afinidad,
- el análisis e interpretación gráfica de los *embeddings* obtenidos,
- el estudio de la dimensión más adecuada para la representación,
- y la exploración de la relación entre **spectral embedding** y **spectral clustering** mediante la aplicación de **KMeans**.

Así, no solo presentamos el algoritmo, sino también una comparativa entre distintas decisiones de modelado y una discusión sobre los resultados obtenidos.

## Estructura del repositorio
- `src/Spectral_embedding.ipynb`: notebook que hemos utilizado para el desarrollo del proyecto. En él incluimos todo el código implementado y bastantes explicaciones relevantes.
- `docs/Spectral_embedding.pdf`: presentación del proyecto. Aquí explicamos la mayor parte del trabajo desarrollado en el notebook, así como la metodología llevada a cabo, la teoría detrás del algoritmo, los detalles del dataset y las referencias empleadas.

## Instrucciones de uso y ejecución
Puedes descargar el notebook desde [`src/Spectral_embedding.ipynb`](src/Spectral_embedding.ipynb) y abrirlo con Jupyter Notebook, JupyterLab o Google Colab.

De forma similar, puedes descargar la presentación desde [`docs/Spectral_embedding.pdf`](docs/Spectral_embedding.pdf) y abrirla con tu lector de PDFs favorito.

## Observaciones
- El notebook está planteado de forma secuencial, así que recomendamos no saltarse celdas en la ejecución del mismo.
- Algunas partes pueden requerir un tiempo de ejecución elevado, especialmente aquellas relacionadas con cálculo de vecinos, construcción de matrices de afinidad y clustering.
- Tanto la presentación como el notebook se complementan mutuamente, así que recomendamos consultar ambos para un mejor entendimiento del tema.
- Si tenéis cualquier duda o sugerencia de mejora, ¡no dudéis en contactarnos!

# image-recognition

En este proyecto se reentrenó la red neuronal convolucional Mobilente para identificar el proceso fotográfico a partir de una imagen digital del objeto original.

![Tipologías fotograficas](imagenes/tipologias.jpg)

Las redes neuronales convolucionales (RNC) son dispositivos para el análisis de información visual que han tenido un desarrollo muy acelerado en los últimos diez años.

La operación de convolución que da nombre a estas redes es aquella en la que el dígito que corresponden a cada pixel de la imagen se multiplica por un filtro o kernel, el resultado es una versión de la imagen en la que se destacan algunas de sus características y se simplifican otras. La convolución se repite en diferentes capas de la red, con lo cual progresivamente se va obteniendo una versión más reducida, pero a la vez más destilada de la imagen, llamada mapa de características, con ésta es posible alimentar la última capa conocida como clasificador y de esta manera la red identifica el contenido de una imagen en alguna de las categorías utilizadas para su entrenamiento.

![convolución](imagenes/convolucion.jpg)

Las redes más comunes han sido entrenadas con Imagenet, un conjunto de datos en el que se muestran personas, acciones, objetos, lugares, animales y vegetales clasificados en 20,000 categorías diferentes.

En este proyecto se utilizó la red Inception y fue reentrenada mediante el proceso llamado transferencia de aprendizaje para diferenciar el proceso fotográfico en imágenes de históricas. Para ello se utilizaron 600 ejemplos de fotografías divididas en tres procesos fotográficos: ambrotipo, daguerrotipo y ferrotipo.

El resultado de este proceso fue una red con un porcentaje de 85 % de precisión en la fase de entrenamiento y de 75 % en la de validación.

Una técnica de visualización basada en la reducción multidimensional permitió identificar que la identificación de las imágenes se basa inicialmente en aspectos como la forma de montaje y presentación (estuche, marco o tarjeta) y solo de forma secundaria en las características físicas relacionadas con el proceso fotográfico, a futuro será necesario intentar que la red enfatice este tipo de característica ya que son las que más interesan en este caso.

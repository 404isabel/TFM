
Identificación de tejido metastástico en exploraciones histopatológicas de secciones de ganglios linfáticos:
Basado en el dataset público del reto:
https://www.kaggle.com/c/histopathologic-cancer-detection/overview

El objetivo principal de este trabajo consiste en la creación de un modelo de predicción capaz de discernir entre una imagen histológica sana y una imagen histológica que presente signos de metástasis con un alto grado de exactitud similar o superior al de un humano, de modo que permita a los patólogos enfocarse en otras tareas menos rutinarias y más complejas inherentes a un ser humano.

Para alcanzar este objetivo se tienen en cuenta los siguientes objetivos específicos:

Desarrollo de arquitecturas secuenciales y residuales de redes neuronales convolucionales para la identificación de tejido metastásico, usando métodos de estimación de parámetros con el objetivo de optimizar los resultados obtenidos.

Desarrollo de arquitecturas basadas en redes pre-entrenadas: ResNet50 y VGG16 en particular, estudiando distintas estrategias: entrenamiento de la red neuronal al completo sin congelar ninguna capa, entrenamiento de la red neuronal congelando todas las capas, uso de fine-tunning (congelar parte de las capas de la red neuronal), así como Ensamble Learning (creación de una red neuronal combinando varias arquitecturas).


Estructura de archivos:

PrepararDatos.ipynb: Para dividir las imágenes en una estructura de carpetas para ser usada por flow_from_directory (carpetas principales: train y validation, con subcarpetas cancer y no_cancer)
hcd-modeloSecuencial.ipynb: Creación y entrenamiento de modelo secuencial desde cero.
hcd-modeloResidual.ipynb: Creación y entrenamiento de modelo residual desde cero.
hcd-modelosPreentrenados.ipynb: Creación y entrenamiento de modelos basados en ResNet50 y VGG16

# NN_MINIST_PYTORCH_DP
Aun aplicación de Privacidad Diferencial en una red neuronal de clasificación de imágenes.

# Explorando la Privacidad Diferencial en PyTorch: Implementación y Análisis en MNIST con Opacus

Este repositorio contiene el código fuente de un proyecto que explora la privacidad diferencial en el contexto de la implementación de modelos de aprendizaje automático en PyTorch, específicamente en el conjunto de datos MNIST, utilizando la biblioteca Opacus.

## Importaciones de Bibliotecas

En esta sección, se explican las bibliotecas que se están importando para el proyecto, incluyendo PyTorch, torchvision, numpy, Opacus y tqdm.

## Carga de Datos de Entrenamiento

Aquí se configura un DataLoader para cargar el conjunto de datos de entrenamiento MNIST, aplicando transformaciones necesarias como la conversión a tensores de PyTorch y la normalización.

## Carga de Datos de Prueba

Se establece otro DataLoader para cargar el conjunto de datos de prueba MNIST con las mismas transformaciones que se aplicaron en el conjunto de entrenamiento.

## Definición de la Arquitectura del Modelo

En esta sección, se define la arquitectura del modelo de aprendizaje automático utilizado para el proyecto. El modelo es una red neuronal convolucional (CNN) con capas convolucionales, capas de agrupación y capas completamente conectadas.

## Definición del Optimizador

Aquí se configura el optimizador SGD que se utilizará para entrenar el modelo. Se especifica la tasa de aprendizaje y se pasan los parámetros del modelo al optimizador.

## Configuración de Privacidad Diferencial

Se configura la privacidad diferencial para el entrenamiento del modelo utilizando la biblioteca Opacus. Se establecen parámetros como el número de épocas, el objetivo de epsilon y delta, y la norma máxima del gradiente.

## Entrenamiento del Modelo y Seguimiento de Métricas

Se define una función de entrenamiento que realiza el bucle de entrenamiento sobre los datos de entrenamiento, calcula la pérdida y la precisión, y registra estas métricas a lo largo de las épocas. También se muestra el valor de epsilon en cada época.

## Función de Ploteo de Métricas (plot_metrics)

Se proporciona una función que permite crear gráficos para visualizar métricas como la pérdida y la precisión en función de las épocas o el valor de epsilon.

## Conclusión del Ejercicio de Privacidad Diferencial

Se concluye el proyecto destacando las métricas clave obtenidas, como la pérdida, la precisión y el valor de epsilon, y se discute la importancia del equilibrio entre la precisión y la privacidad diferencial en el entrenamiento del modelo.

## Fuentes y Referencias

Este proyecto se basó en información recopilada de diversas fuentes y publicaciones. A continuación, se enumeran las fuentes utilizadas:

1. **What is the Privacy Accounting usage?**
   - Publicación: Agosto 2022
   - URL: [Discusión en PyTorch](https://discuss.pytorch.org/t/what-is-the-privacy-accounting-usage/159018/3)

2. **Guide: How to migrate to 1.0 API**
   - Consultado el 28-09-2023
   - URL: [GitHub - Opacus](https://github.com/pytorch/opacus/blob/main/Migration_Guide.md)

3. **Privacy Engine**
   - Consultado el 28-09-2023
   - URL: [Documentación de Opacus](https://opacus.ai/api/privacy_engine.html)

4. **Differential Privacy Series Part 1 | DP-SGD Algorithm Explained**
   - Publicado en PyTorch el 31 de agosto de 2020
   - Consultado el 28-09-2023
   - URL: [Medium - PyTorch](https://medium.com/pytorch/differential-privacy-series-part-1-dp-sgd-algorithm-explained-12512c3959a3)

5. **DIFFERENTIALLY PRIVATE DEEP LEARNING IN 20 LINES OF CODE: HOW TO USE THE PYTORCH OPACUS LIBRARY**
   - Publicado el 31 de agosto de 2020
   - URL: [Blog de OpenMined](https://blog.openmined.org/differentially-private-deep-learning-using-opacus-in-20-lines-of-code/)

6. **FAQ**
   - Consultado el 28-09-2023
   - URL: [Documentación de Opacus - FAQ](https://opacus.ai/docs/faq)

Estas fuentes proporcionaron información valiosa para la implementación de la privacidad diferencial en este proyecto.

# Aprendizaje_profundo

Integrantes:
- Alvarez Lupu, Gustavo
- Ambrosis, Nicolás
- Conrrero, Agustina
- Hayas, Laura
- Luna, Andrés

Dataset: MeLi Challenge 2019. Contiene títulos de publicaciones efectuadas por vendedores en la página web de Mercado Libre.
Los datos están divididos en 2 archivos: train, validation y test.

Objetivo : implementar una Red Neuronal que asigne una categoría a cada título.

PREPROCESAMEINTO
- En una primera instancia, se vectorizaron los títulos de las publicaciones para cada conjunto por separado (train, validation y test).(no se utilizó)
- Posteriormente, se concatenaron los 3 datasets, para crear un diccionario común el cual sirvió como base para vectorizar los títulos de las publicaciones 
de todos los datos juntos.

PROCESOS Y EXPERIMENTOS
Todos los experimentos fueron ejecutados en Nabucodonosor usando las placas de video (CUDA).
- Se utilizaron dos Redes Neuronales: 
1- Perceptrón Multicapa con 2 capas ocultas, y una capa de salida. Utilizamos la función de activación RELU para las capas ocultas,y ninguna activación para la capa de salida con 128 neuronas.
2- Red Convolucional con 3 capas convolucionales que hacen convolución 1D con filtros tamaño 2, 3 Y 4 respectivamente, y 128 neuronas en la capa de salida con activación lineal.

RESULTADOS OBTENIDOS
1- Perceptrón Multicapa
                        - train_loss:	
                        - val_loss:	
                        - validation_balanced_accuracy:	
                        - Tiempo de ejecución: 
                        - Test Balance accuracy: 
                        
2- Red Convolucional
                        - train_loss:	1.187
                        - val_loss:	1.21
                        - validation_balanced_accuracy:	0.717
                        - Tiempo de ejecución: 1.8 horas
                        - Test Balance accuracy: 0.773

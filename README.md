
![Logo](https://upload.wikimedia.org/wikipedia/commons/6/6d/LogoUGcolor.png)


# Implementación de Programas de Detección para la Evaluación de la Calidad de Cajas en Procesos Industriales

Este es un proyecto donde usamos el modelo Yolov5 para la calidad de las cajas, se debió
crear un dataset de imágenes ya que el modelo no tenia la clase cajas. Usamos herramientas 
como MakeSensei para realizar el etiquetado de las imágenes que se clasificaban en “box 
good” y “box bad”. Usamos el servicio de Google Coolab para usar sus recursos de 
procesamiento como lo es su GPU para poder entrenar nuestro modelo. Al final logramos que 
pudiera diferenciar entre las cajas correctamente empaquetada y las que no lo estaban con 
algunas excepciones.

## Dataset

Se utilizaron 200 imagenes de cajas que estaban cerradas, abiertas, dobladas o rotas. La forma de la caja es rectangular o cuadrada.
![Dataset](https://github.com/CornejoTG/Grupo4_ia_2024/blob/main/imagenescajas.png?raw=true)

# Etiquetas

La imagenes se etiquetaron en dos clases "box good" y 'box bad'. Las box bad son las cajas que tienen algun hueco o que no estan cerradas.
![prueba1](https://raw.githubusercontent.com/CornejoTG/Grupo4_ia_2024/main/prueba1.png)
![prueba2](https://raw.githubusercontent.com/CornejoTG/Grupo4_ia_2024/main/prueba2.png)

# Resultado

Finalmente el modelo se uso con un video de una linea de produccion de empaques. S puede apreciar que las cajas que estan en la banda de ensamblaje se detectan como defectuosas porque no estan cerradas aun, mientras que las que estan al final se toman como buenas.

![prueba2](https://raw.githubusercontent.com/CornejoTG/Grupo4_ia_2024/main/comparacion.png)

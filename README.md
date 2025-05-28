# TelecomX_LATAM
Challenge del curso de DataScience con Python de Alura Latam

## **Introducción.**

Se presenta el análisis de la empresa de telecomunicaciones TelecomX_LATAM, la cual esta perdiendo muchos clientes, nos solicitó que revisaramos sus datos, 
para  de ser posible que detectemos cual es la causa de que los clientes se este retirando de la compañia.


## **Instrucciones de uso**

* import pandas as pd
* import matplotlib.pyplot as plt
* import seaborn as sns
* import numpy as np
* Se debe dar click en cada una de las celdas del documento Googlecolab


## **Limpieza y tratamiento de datos**

* Se procedió a importar a un dataframe el archivo: 'TelecomX_Data' el cual viene de una API y esta en formato JSON.
* Se revisaron las primeras 5 lineas del dataframe.
* Por medio de df.info(), se obtuvo la información de que el df tiene 7267 lineas y 6 columnas, sólo las dos primeras columnas tiene información individual, en las restantes la información esta en forma de dicccionarios.
* Se procedió a extraer (normalizar) cada diccionario en un nuevo df, que al final se concatenaron con las dos primeras columnas, resultando en un df de 7267 lineas y 21 columnas.
* Se cambió el tipo de data de 'Charges.Total' a float64

  ## **Análisis y exploración de datos**
* Se generaron un dataframe para evasores y otro para usuarios que se mantinen, para compararlos respecto al tiempo que permanecen con el servicio(tenure).
 ![image](https://github.com/user-attachments/assets/75d7bee9-7a81-48a9-b5f7-cfba0660670d)
 Se observa que la mayoria de los usuarios evadidos se van al primer mes.

* Al comparar los usuarios evadidos y actuales respecto al estatus de adulto mayor.
  ![image](https://github.com/user-attachments/assets/0baa19b2-9c23-497e-bfd7-7b952e832875)
  Se observa que la mayoria de los evadidos no son adultos mayores(casi tres veces más)
* Comparación respecto al tipo de contrato.
 ![image](https://github.com/user-attachments/assets/e21fdfd7-e84c-4ecc-af83-db9a3c5d423e)
Los evasores tiene en mayor proporción ( aproximadamente 2 a 1) contratos mes-a-mes respecto a los usuarios no evasores.
* Comparación de la duración promedio para clientes que se dieron de baja y los que no

  ![image](https://github.com/user-attachments/assets/317b3d22-5515-430d-8e2b-f0d5c8786818)
   El promedio de duracion de los evasores es de 17 meses vs 37 meses en los no evasores.

* Matriz de correlacion entre evasión(churn) y variables numéricas seleccionadas.
  ![image](https://github.com/user-attachments/assets/623b57e6-36b7-4fd1-a11b-e2f8135216ec)
  
  La mayor correlación negativa es contra duración(tenure), la mayor correlación positiva es respecto a cargos mensuales
  
## **Conclusiones**
* La mayoria de los evasores se van al primer mes.
*  El costo mensual de los evasores es mayor que el de los no evasores.
*  La mayoria de los evasores no son adultos mayores.
*  Los evasores tenian contratos mes-a-mes en mayor proporción.
*  El promedio de duracion de los evasores es de 17 meses vs 37 meses en los no evasores.

## **Recomendaciones**

* Ofrecerle paquetes anuales o mulitanuales a los clientes con una mejor tárifa mensual, incluyendole dos servicios de su elección entre : películas,TV,líneas multilpes, online-security.
* A los clientes nuevos ademas de ofrecerle lo anterior, incluirle un mes gratis.


  

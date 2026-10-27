# prosperStartup.AI
Modelo de prediccion de startups, regresión logística

Primer paso: Búsqueda de datasets

Hemos encontrado 2 datasets => 

https://www.kaggle.com/datasets/manishkc06/startup-success-prediction
https://www.kaggle.com/datasets/amirataha/startups

Elegimos finalmente 
https://www.kaggle.com/datasets/amirataha/startups

Hay 196.553 empresas, pero 183.441 son operating, es decir, todavía no sabemos si triunfan o fracasan.

Con desenlace conocido quedan 13.112: acquired 9.394, ipo 1.134 y closed 2.584.

El problema: las empresas de éxito tienen muchos más campos vacíos. Por ejemplo, funding_rounds está vacío en el 71 % de las de éxito y solo en el 19 % de las cerradas. Si no se corrige, el modelo aprende que “sin datos = éxito”.

Nos quedaremos con las empresas que tienen datos de financiación, salen 5.172 (60 % éxito, 40 % fracaso) y los nulos quedan parejos entre clases.

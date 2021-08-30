Creo que lo más importante de este paper es como nos muestra la importancia y flexibilidad que posee la factorización del problema mediante el modelo matricial.

Antes de este modelo existieron otros varios que intentaban representar o al usuario ("User-based Collaborative filter"), o a los items ("Item-based Collaborative filter"). Algunos conseguían buenos resultados pero eran modelos que no permitían al operador poder representar pequeños cambios y movimientos que se producen normalmente en la vida cotidiana.

El problema que tuvo en sus inicios el modelo matricial fue que para generar calculos con él necesitamos que en su mayoría la matriz se encuentre llena y no vacía, pero en general los usuarios no evaluan la mayoría de las películas sino que solo una pequeña proporción de estas.
Se solucionó este problema generando una matriz con todo el explicit feedback (ratings) y en las demás columnas datos que fueran de importancia para nosotros como el sesgo del usuario, el sesgo del item, las preferencias del usuario y demases.

La gracia de usar una matriz es que como consiste de distintas entradas, nos permite de alguna forma "dividir para conquistar". Y es que es mucho más simple siempre dividir el gran problema (*predecir rating*) en varios subproblemas (*sesgo del usuario, el sesgo del item, las preferencias del usuario*) de manera que sea más simple tratarlos y lograr un mejor rating general. De esta manera mediante todas estas distintas variables podemos generar un espacio donde los items similares queden cercanos con mucha mayor cantidad de detalles y precisión que como lo hacia KNN. 

Además al tratar cada variable de manera separada como un vector, podemos entrenar un modelo mediante "stochastic gradient descent" o "alternating least squares" que vaya aprendiendo más sobre el usuario y obtener así mejores resultados.

Por otro lado quería comentar que nunca entendí bien la ecuación que se encuentra dos ecuaciones antes de la (6) (No esta numerada). Entiendo la normalización del vectur u, pero no entiendo por que la sumatoria de los X sub i esta elevado a 4.5 y eso me genero ciertas dudas.

Finalmente quería cerrar notando el trabajo en equipo, algo que se tiendía a menospreciar en el área de la computación, pero que a día de hoy sabemos lo importante y clave que es el poder trabajar en equipo. Me pareció muy interesante y lógico que el autor haya juntado fuerzas con otro gran equipo del Netflix price para poder lograr un mejor resultado y casi lograr el millon de dolares.

## Lectura 1

Quiero partir mi comentario con un breve resumen y recalcando que la lectura habla y profundiza justamente todo lo que se hablo esta semana en clases.

El artículo parte mencionando y explicando lo que es el Collaborative Filtering (CF), el porque se aplica hoy en día y como funciona. Se habla sobre como los seres humanos, incluso antes del internet, nos recomendábamos películas, restaurantes, libros, lugares, etc. Y que si tuvieramos el poder de computo podríamos generar programas que sepan exactamente que recomendarnos. Pero como no tenemos ese poder de cómputo y el dinero para llevarlo acabo, lo mas simple, efectivo y razonable es meter a las personas a la ecuación y que el programa encuentre recomendaciones para nosotros a partir de los demás usuarios en la página.

También se habla en el paper las principales 3 funciones de los CF, que consisten en:
a) recomendar items 
b) predecir puntaje de items
c) Recomendaciones con restricciones

Y que existen dos principales visiones para enfrentar este problema. Las dos visiones corresponden a: 
1) modelos no probabilísticos -> los más populares en un comienzo EJ: KNN, grafos, redes neuronales

2) modelos probabílisticos -> de a poco han ido ganando popularidad sobretodo con el auge de las probabilidades Bayesianas por sobre la clásica.  

Pero indendiente de la visión escogida, los modelos actuales son útiles para los siguientes casos y necesita que lo siguiente ocurra porque de lo contrario no pueden realizar recomendaciones eficientes.

-> muchos items (sino no es necesario usar CF)
-> muchos ratings por item
-> mas ratings que items 
-> que los usuarios den varias recomendaciones

También se comenta en el paper lo discutido en clases sobre como estos métodos de CF poseen un Cold start que se refiere a problemas para recomendar cuando tenemos un nuevo usuario, un nuevo item y una nueva comunidad. Se dan distintas soluciones para tratar con cada uno pero cabe destacar que una nueva comunidad es lógicamente las más dificil de hacer andar.

Ahora Finalmente luego de este breve resumen me gustaría comentar sobre los puntos más interesante a mi gusto presentes en el paper.

1 - Novelty: Me gusto mucho el concepto de novelty que corresponde a items que el usuario vió gracias a una recomendación y le gusto pese a que no estaba dentro de sus preferencias y gustos. Es decir el sistema se arriesgo un poco saliendose de la zona de confort y en vez de recomendar puras películas de acción como le gustan a Pedrito, le recomendo una romantíca que a Pedro le encanto. 
Lo que me llama la atención de esto es que claro es muy interesante y llamativo el concepto pero también hay que tener precaución sobre que tanto arriesgarse pues el sistema podría empezar a recomendar cosas que no le agraden para nada al usuario. Me gusta el tradeoff que genera de tal vez recomendar algo indeseado con intentar darle algo nuevo y distinto al usuario.

2- Ataques a Items: Me pareció llamativo e incluso se habló en clases como aún es dificil identificar cuando en verdad una película es mala o si es que un grupo de personas se puso de acuerdo para bombardear con malas reviews a esta película. Esto no solo genera un problema en el sistema sino que también influencia a otras personas a seguir con los mismo por ende el sistema pierde un poco la Fe en sus usuarios. 

3- El último concepto es un poco más simple pero igual me causó interés y corresponde a como los usuarios se dejan influenciar por el score promedio de un item. Se menciona en el paper como esta demostrado que a los usuarios les cuesta mucho evaluar un item muy distinto del score promedio que sale en la página. Esto muestra como los seres humanos nos dejamos influenciar por las masas logrando que incluso en algo tan simple y anónimo siga ocurriendo. 
El paper discute y explica el gran desarrollo que ha tenido el Deep learning sobre todo en el area de los Sistemas recomendadores. Es este de discuten y explicán una recopilación de varios papers sobre Deep learning.

Lo primero que se menciona es algo que ya sabíamos y es que los modelos con Deep Learning se han sometido a pruebas en línea y han mostrado una mejora significativa con respecto a los modelos tradicionales. Por lo tanto, podemos ver que el Deep Learning ha impulsado una revolución notable en las aplicaciones de recomendación.
Por otro lado también se menciona que el número de papers al respecto ha aumentado exponencialmente.
Sin embargo, faltan revisiones exhaustivas sobre los sistemas de recomendación basados ​​en el aprendizaje profundo.

A continuación el artículo describe algunos conceptos y técnicas importantes del deep learning como: 

* El perceptrón multicapa (MLP)
* Un codificador automático (AE)
* The Convolutional Neural Network (CNN)
* The Recurrent Neural Network (RNN)
* Aprendizaje de refuerzo profundo (DRL)

Personalmente yo ya curse el curso de Deep learning y conozco las técnicas mencionadan anteriormente, pero no me parece que la idea de la lectura sea definir los conceptos que de por si ya se definen en el paper sino, al contrario pensar y discutir sobre el concepto que se nos presenta en el artículo.

Algo que sí creo que es importante de remarcar del paper son las propiedades más atractivas de las arquitecturas neuronales por sobre los métodos tradicionales. Estas son: 

(i) diferenciables de extremo a extremo 

(ii) proporcionan sesgos inductivos adecuados para el tipo de datos de entrada. Si hay una estructura inherente que el modelo puede explotar, las redes neuronales profundas deberían ser útiles para ello. Por ejemplo, las CNN y las RNN han explotado durante mucho tiempo la estructura intrínseca de la visión (el lenguaje humano). Del mismo modo, las estructuras secuenciales de sesiones o registros de clics son muy adecuadas para los sesgos inductivos proporcionados por los modelos recurrentes / convolucionales.
Por ejemplo, cuando se trata de datos textuales, datos de imágenes (publicaciones sociales, imágenes de productos), las CNN / RNN se convierten en bloques indispensables.

(iii) Transformación no lineal.
A diferencia de los modelos lineales, las redes neuronales profundas son capaces de modelar la no linealidad en los datos con activaciones no lineales como relu, sigmoid, tanh y similares. Esta propiedad permite capturar patrones de interacción de usuario / elemento complejos.

(iv) Representación Aprendizaje. 
Las redes neuronales profundas son eficaces para aprender los factores explicativos subyacentes y las representaciones útiles a partir de los datos de entrada. En general, una gran cantidad de información descriptiva sobre elementos y usuarios está disponible en aplicaciones del mundo real. Hacer uso de esta información proporciona una forma de mejorar nuestra comprensión de los elementos y los usuarios, lo que resulta en un mejor recomendador. Como tal, es una elección natural aplicar redes neuronales profundas al aprendizaje de representación en modelos de recomendación. Las ventajas de usar redes neuronales profundas para ayudar al aprendizaje de la representación son dos: 

    (i) reduce los esfuerzos en el diseño de características de creación manual. La ingeniería de características es un trabajo que requiere mucha mano de obra y las redes neuronales profundas permiten el aprendizaje automático de características a partir de datos sin procesar, ya sea en un enfoque supervisado o no supervisado.

    (ii) Permite que los modelos de recomendación incluyan información de contenido heterogéneo como texto, imágenes, audio e incluso video.

(v) Flexibilidad.
Las técnicas de aprendizaje profundo poseen una gran flexibilidad, especialmente con el desarrollo y el empuje que poseen actualmente muchos marcos de aprendizaje profundo populares como Tensorflow, Keras, Caffe, MXnet, DeepLearning4j, PyTorch y Theano. La mayoría de estas herramientas se desarrollan de forma modular y cuentan con un apoyo comunitario y profesional activo.
En este punto también podemos añadir algo que se menciona luego que es la recomendación con modelos híbridos profundos. Algunos modelos de recomendación basados ​​en el aprendizaje profundo utilizan más de una técnica de aprendizaje profundo. La flexibilidad de las redes neuronales profundas hace posible combinar varios bloques de construcción neuronales para complementarse entre sí y formar un modelo híbrido más poderoso.

Después el artículo menciona y describe varias técnicas que fueron adaptadas y que hoy se utilizan con Deep learning como:

-Extensión neuronal de los métodos de recomendación tradicionales

-Aprendizaje de representación de funciones con MLP

-Recomendación con modelo semántico estructurado profundo.

-Recomendación basada en codificador automático

-Recomendación basada en redes neuronales convolucionales

Por otro lado otro aspecto importante del artículo que me gustaría remarcar son los argumentos negativos y limitaciones que existen hoy en día en el area de desarrollo frente a las técnicas de Deep learning.
Un argumento común en contra de las redes neuronales profundas es que las ponderaciones y activaciones ocultas generalmente no son interpretables, lo que limita la explicabilidad. Una segunda limitación posible es que se sabe que el aprendizaje profundo consume muchos datos, en el sentido de que requiere datos suficientes para respaldar plenamente su rica parametrización. Un tercer argumento bien establecido contra el aprendizaje profundo es la necesidad de un ajuste exhaustivo de los hiperparámetros. Naturalmente, las redes complejas generalmente introducen más hiperparámetros, que requieren una etapa de ajuste costosa al entrenar modelos (por ejemplo, número y ancho de capas).

Pero a mi parecer la idea más importante que se menciona en el paper es que las redes neuronales profundas se justifican cuando hay una gran cantidad de complejidad o cuando hay una gran cantidad de instancias de entrenamiento. Si bien el Deep learning es muy útil, eficaz y domina el presente de los sistemas de recomendación, no debemos caer en sus encantos. A lo que me refiero es que hay casos y casos y no debemos llegar y aplicar Deep learning porque sí. Si el día de mañana nos contrata una empresa deberíamos evaluar si la información que tenemos la cantidad de usuario de nuetra red, items, etc para luego recien decidir si vale la pena aplicar Deep learning. Esto porque justamente uno cree que realizar lo más dificil traerá los mejores resultados, y bueno esto es cierto para muchos casos, pero no debemos olvidar también métodos más simples que sepamos modificar e implementar. Y me gustaría terminar mi comentario citando a un gran profesor que tuve llamado Néstor Gutierrez el cual muchas veces me mencionó lo siguiente con mucha razón:
"A veces hacer las cosas simples es lo más complicado"


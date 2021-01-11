# Alba Jiménez Arribas 100386906

# Implementación de una aplicación para identificar y detectar billetes 

Se ha desarrollado un identificador de billetes mediante Teachable Machine, una plataforma de inteligencia artificial que sirve para entrenar un sistema y que
este pueda reaccionar a imágenes o sonidos.

Para la implementación de nuestro sistema se ha creado cinco clases, cuatro tipos de billetes (de 5, 10, 20 y 50 euros) y una clase en caso de que el individuo no tenga
ningún billete.
Para cada billete se ha utilizado diferentes imágenes de internet, además de muestras en movimiento mediante la webcam. Aproximadamente para cada billete
se ha utilizado 100 muestras por las dos caras.
Para la clase "sin billete" se han utilizado varias imágenes de diferentes caras, lugares y fondos.

Después de entrenar a nuestro sistema y ver que funciona correctamente hemos exportado el código mediante Tensorflow.js para implementar la aplicación en
glitch.com.

En glitch.com se ha iniciado un proyecto de nodo simple. Por defecto, se crea un proyecto predeterminado que se va mejorando y perfeccionando para cada
sistema. Para la creación de nuestro diseño se han utilizado varios ejemplos que facilita la plataforma como ayuda.

Los archivos .css (reset.css y style.css) sirven para diseñar el estilo de nuestra página https://detector-billetes.glitch.me/
Los archivos .js (bar-graph.js y model-runner.js) son los archivos JavaScript que se ejecutan en la página web.
Por último, el archivo index.html contiene el sistema que hemos diseñado mediante Teachable Machine. Para ello se ha añadido la URL del archivo creado en Teachable
Machine que se había subido a la nube. Este archivo además contiene la interfaz y el título de nuestra página.

# Recomendaciones

Para utilizar el identificador de billetes se recomienda acercar el billete a la cámara para que no haya confusión con el entorno en el que se encuentra. Además se
recomienda un ambiente con buena luz que permita distinguir los billetes, ya que hay billetes de colores parecidos que pueden producir fallos (como el billete de 10 y
de 50).

# Evaluación del resultado

Se han tomado varias muestras de todos los billetes probando diferentes posiciones y ángulos, tanto de cerca como de lejos y por las dos caras. En todas las muestras 
se ha intentado mantener una buena calidad de luz, por ello en ambientes oscuros el sistema puede tener una menor precisión de acierto. 
Además para la clase "sin billete" se han tomado varias muestras en diferentes ambientes con colores parecidos a los de los billetes para que el diseño sea capaz
de diferenciar mejor entre un fondo o un billete y no por ejemplo, que si en el fondo hay algún tono naranja se confunda con un billete de 50. Aún así si la calidad 
de la cámara no es suficientemente buena esto puede seguir sucediendo, por ello se recomienda acercar lo máximo posible el billete para que los colores no se mezclen con 
el ambiente. En nuestro caso hemos utilizado una cámara incorporada en el ordenador de estándar VGA con dimensiones de anchura y altura de 640x480 y 0.307 megapíxeles.
Este hardware no es el más optimo pero es suficiente para una precisión aceptable en nuestro prototipo.
También debe tenerse en cuenta la calidad de la luz, la precisión cambia según la luz que se utilice. Si se utiliza una luz natural o blanca que sea limpia y clara se
obtendrán mejores resultados. Si, por ejemplo, se utilizan luces o bombillas que tienden al naranja, estas consiguen que el reflejo en el billete se anaranje y tienda
(aunque minimamente) al billete de 50. 
Con las pruebas que hemos realizado se ha visto un porcentaje de acierto de aproximadamente el 80% con el billete a una media distancia y del 97% a una cercana 
distancia. Cuanto más se alejaba el billete menos porcentaje de aciertos ocurría.

# Hardware del sistema

Se ha utilizado una cámara de ordenador de estándar VGA con dimensiones de anchura y altura de 640x480 y 0.307 megapíxeles.
En cuanto al ordenador en el que se ha probado es un HUAWEI MateBook con procesador Intel Core i7-7500U CPU @2.70 GHz y 8 GB de RAM.

# Posibles utilizaciones y usos

Se ha decidido realizar este prototipo de detector de billetes por su útil uso en comercios y tiendas. Como se ha explicado anteriormente, este diseño 
no es totalmente óptimo y seguro pero con la utilización de mejores equipos y un mejor desarrollo podría diseñarse una
aplicación que favoreciese y facilitase la movilidad de efectivo en los establecimientos debido a la sencillez y rapidez del diseño.

# Modelo de cajas en HTML5
Puede parecer complicado (y de hecho, para mi lo fué ~~por culpa del señor que me lo "intentó" enseñar sobre todo~~) pero no es más que el *espacio* que hay entre el contenido, que puede ser un texto, hasta otro elemento, pasando por el espacio comprendido del contenido al borde, la anchura del propio borde y, finalmente, el espacio desde el borde a otro elemento.
Cada uno de estos espacios (y anchura en el caso del borde) pueden ser configurados mediante css con las instrucciones:
* *padding: 10px;* - aumenta el espacio **entre el contenido y el borde** en *10 píxeles*.
[+info_padding] (https://developer.mozilla.org/es/docs/Web/CSS/padding)
* *border: 1px solid;* - aumenta la **anchura** del propio borde, haciéndolo visible, en *1 píxel*.
[+info_border] (https://developer.mozilla.org/es/docs/Web/CSS/border)
* *margin: 10px;* - aumenta el espacio **entre el borde y otro elemento** en *10 píxeles*.
[+info_margin] (https://developer.mozilla.org/es/docs/Web/CSS/margin)
Cabe destacar que, tanto padding como margin, pueden aumentar el espacio de un lado específico:
* *padding-top: 10px* - aumenta el espacio en la parte *superior*.
* *padding-bottom: 10px* - aumenta el espacio en la parte *inferior*.
* *padding-right: 10px* - aumenta el espacio en la parte *derecha*.
* *padding-left: 10px* - aumenta el espacio en la parte *izquierda*.
Ejemplo de modelo de Cajas:
![Modelo-de-cajas] (../img/box-model.PNG)
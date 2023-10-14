# Audio con etiquetas HTML
Se puede insertar y utilizar audio en una  página web mediante la inserción de la etiqueta:

    <audio id="audioID" controls>
    	<source src="sounds/alarma.mp3" type="audio/mpeg">
    	Sonido no habilitado
    </audio>
<br>

* Con el id se puede apuntar a esta etiqueta para utilizarla, en caso de que no queramos ponerle controles de este tipo, el cual se añade con el atributo *controls* :
<br><br>

![image](https://github.com/fjlinval/MiGuiaDeCampo/assets/136980197/51cf8c09-a032-4bfc-bff4-142998ff217d)

* La etiqueta *source* se utiliza para encontrar el archivo, pudiéndose encontrar de manera local o con una url., mientras que el *type* es el tipo de audio a enviar.
* El mensaje *"Sonido no habilitado"* puede usarse en caso de que el sonido no pueda ser activado, de un error o no se encuentre mediante el source, **como los mensajes de las imagenes**.
<br>
Para escuchar un audio mediante javascript debemos utilizar la función:

```
play();
```

Y suele ser utilizada como:

```
document.getElementById("ID").play();
```

Hay más funciones que pueden utilizarse con esta etiqueta, pero no las pongo aquí porque ~~soy un flojo~~ sería muy engorroso ponerle ejemplos de todos, así que os dejo la wiki de siempre.

+info audio ---> (https://developer.mozilla.org/es/docs/Web/HTML/Element/audio)

# Trabajar con fecha y hora
Podemos trabajar con tiempo y fechas gracias a la función:

```
new Date ();
```

Lo recomendable es guardar esto es una variable y, desde ahí, sacar **horas minutos y segundos** en diferentes variables:

```
let time = new Date ();
let timeHours = tiempo.getHours();
let timeMinutes = tiempo.getMinutes();
let timeSeconds = tiempo.getSeconds();
```

Con esto guardamos en las variables la hora, minutos y segundos, respectivamente, de la hora local del pc, pero el problema llega cuando lo que nos devuelve es sólo **un número**, es decir, que si son la 1:00 am nos va a devolver como hora un **"1"**, lo que quedaría bastante feo si quisiéramos construir, por ejemplo, un reloj digital, por lo que podríamos utilizar este snippet:

```
let time = new Date ();
let timeHours = String(tiempoActual.getHours()).padStart(2,"0");
let timeMinutes = String(tiempoActual.getMinutes()).padStart(2,"0");
let timeSeconds = String(tiempoActual.getSeconds()).padStart(2,"0");
let timeDigital = timeHours + ":" + timeMinutes + ":" + timeSeconds;
```
Con esto lo que hacemos es pasar a *String* las variables y, con **padStart(2,"0")**, rellenamos la cadena de caracteres que hemos convertido, que pueden ser de 1-2 si se da el caso de ser las 1:00 am, con **2** caracteres obligatoriamente, añadiendo **desde la izquierda** los caracteres que pongamos entre comillas en la función, en este caso **"0"**. En definitiva, te añade un **0** si sólo hay *1* carácter en el String.
Con **"let timeDigital"** prácticamente concatenamos las variables anteriores y las ponemos en formato de reloj digital, como por ejemplo:

```
06:07:33
```

## **Importante**
Si queréis que vuestro reloj se vaya actualizando constantemente, ya que el código anterior es sólo para capturar la hora en el momento concreto, podéis hacerlo de la siguiente manera:

```
function digitalClock (){
  let time = new Date ();
  let timeHours = String(tiempoActual.getHours()).padStart(2,"0");
  let timeMinutes = String(tiempoActual.getMinutes()).padStart(2,"0");
  let timeSeconds = String(tiempoActual.getSeconds()).padStart(2,"0");
  let timeDigital = timeHours + ":" + timeMinutes + ":" + timeSeconds;
}
function reloadTime (){
  setInterval(digitalClock,1000);
}
function onloadWebpage (){
  digitalClock();
  reloadTime ()
}
```
Con la función **"digitalClock()"** creamos el reloj y, con **"reloadTime ()"** utilizamos la función **setInterval(digitalClock,1000)** para ir recargando la función del reloj cada segundo, es decir, recargamos **"digitalClock()"** cada **"1000"** milisegundos (cada segundo).
La función **"onloadWebpage ()"** la utilizo en el body con el atributo **"onload='onloadWebpage ()'"** para que se ejecute, aunque lo recomendable sería modificar una etiqueta específica **vacía** con estilos predeterminados y, mediante *"DOM"*, modificar su "innerHTML" para que aparezca el reloj.
Por cierto, si no se colocan ambas funciones y sólo cargamos **"reloadTime ()"** el reloj aparecerá un segundo después de ser cargada la página.


### Enlaces
+info Date --> (https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Global_Objects/Date)<br>
+info padStart --> (https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Global_Objects/String/padStart)
+info setInterval --> (https://developer.mozilla.org/es/docs/Web/API/setInterval)

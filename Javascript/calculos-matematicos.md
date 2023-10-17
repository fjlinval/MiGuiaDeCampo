# Cálculos matemáticos con la función Math
La función *Math* consta de varios métodos para especificar el cálculo que se quiere realizar, siendo algunos de ellos los siguientes.

## Potencias
Para realizar operaciones con potencias utilizamos el método **pow**:

```
Math.pow(a,b);
```

Donde *a* es la base y *b* el exponente, es decir, que **Math.pow(2,3)** devolverá un resultado de *8*, ya que 2 elevado a 3 es *2x2x2*.

## Raíz cuadrada
Para realizar operaciones con potencias utilizamos la función **sqrt**:

```
Math.sqrt(c);
```

Donde *c* es el número a calcular, es decir, que **Math.sqrt(25)** devolverá un resultado de *5*, ya que esa es su raíz cuadrada.

## Sacar los números mayor y menor de una serie dada
Podemos utilizar dos métodos para saber el número mayor y menor de una serie o, un caso más util, un *array*, mediante el uso de los métodos *max y min*:

```
Math.max(a,b,c,d,...);
Math.min(a,b,c,d,...);
```

Para dar un ejemplo sobre estos métodos la función **Math.max(1,2,3,-2)** devolverá *3*, mientras que **Math.min(1,2,3,-2)** devolverá *-2*.
Algo **muy muy útil** sobre esto es que podemos combinarlo con un array de datos **numéricos** para sacar el mayor o menor, según nos convenga, mediante la inserción del siguiente código:

```
let miArray = [1,5,-4,4];
let maxArray = Math.max(...peperray); // Devolverá 5
let minArray = Math.min(...peperray); // Devolverá -4
```

Es **Imporante** colocar los **...** delante de la variable array llamada o dará un resultado **NaN**.

## Recibir un número aleatorio

Con el método **random** podemos montar una función (ya que por sí sola nos muestra un número decimal entre 0 y 0.9999...) para conseguir un **int** aleatorio, introduciendo nosotros el número máximo **(que no se incluirá)** en la propia funcion:

```
function randomInt (minNumber,maxNumber) {
    return Math.floor(Math.random() * ((maxNumber + 1) - minNumber) + minNumber);
}
```

Por lo que, si insertamos **randomInt (0,100)** nos devolverá un número comprendido entre *0 - 100*.

## Número PI
La propiedad PI sirve para tener el propio número PI y poder guardarlo en una constante:

```
Math.PI;
```

+info Math --> (https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Global_Objects/Math)

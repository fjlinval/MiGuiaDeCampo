# Ejecutar una funcion en un tiempo determinado
## Caso 1
Podemos ejecutar la función (o el trozo de código) que queramos en los segundos que necesitemos mediante la función:
```javascript
    setTimeout (X,1000);
```
En X se puede insertar el nombre de la función a ejecutar y "1000" se refiere a los milisegundos, es decir, que si queremos realizar la función "activarsonido()" en 9 segundos el código sería:
```javascript
    setTimeout (activarsonido, (1000 * 9));
```
Además, podemos añadir una variable para los segundos, en caso de que queramos que sea el usuario, por ejemplo, el que elija el tiempo de activación de la función
## Caso 2
También se puede utilizar un "string" con un console.log mediante esta función, pero debe ser ejecutada de la siguiente manera:
```javascript
    setTimeout(() => {
        console.log("Hello World!");
    }, (1000 * 9));
```
Para información detallada sobre esto:<br>
[setTimeout_Web_Docs](https://developer.mozilla.org/en-US/docs/Web/API/setTimeout)

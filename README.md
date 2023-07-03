# cursojs03072023

## variables
Una variable, es un espacio de memoria que se puede modificar.

### definir una variable:
```js
let nombrevariable="valor"; // variable de tipo string
var nombrevariable2="valor"; // variable del tipo string
nombrevariable="hola"; // la variable tiene un valor nuevo
nombrevariable=20; // la variable puede cambiar su tipo de datos
```

## constantes
Una constante es un espacio de memoria que no se puede modificar
```js
const IVA=1.19; // por lo general, la constantes se escriben en mayuscula
IVA=222; // genera un error 
```

## tipos de datos basicos

```js
let string1="hola";  // texto (string)
let string2='hola'; // texto (string)
let entero1=20; // entero (int)
let flotante1=22.2; // flotante (float)
let booleano1=true; // booleano (bool)
// NaN (not a number)
// null (no tiene valor, pero la variable esta definida)
// undefined (es una variable no definida)
```

## tipos de datos compuesto

Ejemplo: quiero tener un producto
```js
let nombre="cocacola";
let precio=5555;
let categoria="bebida";
```
Cuando quiero tener un conjunto de variables:
```js
let producto={
   nombre:"cocacola",
   precio:5555,
   categoria:"bebida";
}; // variable del tipo objeto.
```

Ejemplo: quiero tener un listado de productos

```js
let productos=["cocacola","fanta",'sprite'];
```

## funciones


```js
function sumar(n1,n2) {
   return n1+n2; // opcionalmente la funcion puede regresar algo
}
let total=sumar(20,30);
document.write(total); // 50
```

En javascript una variable puede ser una funcion:
```js
let variable1=function(n1,n2) {
    return n1+n2;
}
let total=variable1(20,30);
document.write(total); // 50

// redefiniendo las variables:

variable1=function(n1,n2) {
    return n1*n2;
}
total=variable1(20,30);
document.write(total); // 600
```

## ejemplo factura

```js
let factura={
    numfactura:1,
    nombrecliente:"john",
    fecha:"01/01/2020",
    detalle:[
        {descripcion:"cocacola",cantidad:3,precio:5000},
        {descripcion:"fanta",cantidad:1,precio:2000}
    ],
    mostrar:function() {
        document.write("hola");
    }
};
```
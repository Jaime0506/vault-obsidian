# Guía 2
EL área donde se almacenan los datos de una computadora real, tales como memoria, registros y medios externos, normalmente tienen una estructura relativamente simple, como secuencias  de bits agrupadas en bytes.

### **Variable**:
Las variables en un lenguaje de programación permiten almacenar información de forma temporal en la memoria del computador para ser utilizadas por un programa para realizar cálculos matemáticos con los valores almacenados en ellas, realizar comparaciones, condiciones, toma de decisiones o simplemente imprimir datos.

### **Constantes**:
Son variables que no cambian su valor en tiempos de ejecución, es decir independientemente de la función o procesos del código, esta variable no podrá mutar su valor.

```ad-example
Un ejemplo de variable tipo constante, podria ser **PI**:

~~~JavaScript
	const PI = 3,141515
	//Ejemplo de codigo en JavaScript
~~~
Por mas que intentemos asignarle o cambiarle el valor a la variable PI, no lo lograremos ya que la definimos como un tipo de dato constante.
```

### **Tipos de datos**:
El tipo de dato de una variable o constante es la característica natural propia del valor que almacenara, es decir dependiendo el tipo de dato que definamos al momento de declarar una variable o constante, esta solo podrá recibir o almacenar ese tipo de dato correspondiente.

```ad-example
~~~ Java
	String nombre;
	int numero;
	boolean condicion;
	
	//Ejemplo en Java
~~~
En este ejemplo, declaramos 3 variables, de tipo String, int y boolean, es decir estas variables solo podran almacenar tipos de datos correspondiente a su declaracion.

```ad-warning
title:
Tener encuenta que en cada lenguaje, existen tipos de datos distintos y hay lenguajes mas flexibles que otros en cuestio del tipado de datos.

```

### **Reglas para definir variables**:

---
 - **Nombres de variables con sentido**:
```ad-note
title:
Es decir que el nombre al que le asignemos a la variable, tenga relación con los datos que va a almacenar.
```
- **Debe empezar por una letra**:
```ad-note
title:
El nombre de las variables debe empezar siempre por una letra, se concidera buena practica.
```ad-example
title:
~~~Java
	String nombre;
	boolean Condicion;
	int Numero_entero;
~~~

Ni debe tener caracteres en blanco o espacios.
```ad-warning
title: 
Debido a que los caracteres en blanco (espacios), al momento de designarle el nombre a una raviable, estan prohibidos, se recomienda usar **_**
```
- **No usar caracteres especiales como:**
```ad-error
title:
$, %, #, -, +, (),
```

### **Tipos de datos en Java**:

![[ArcoLinux_2022-08-24_11-10-01.png]]

---

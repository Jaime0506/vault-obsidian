# Guía 3
### **Estructuras de decisión**
Como su propio nombre lo dice, una estructura de decisión evalúa el valor de una variable o una expresión como condición, si dicha expresión es verdadera ejecutara cierta porción de código y si dicha expresión es falda, puede:

- No ejecutar nada mas.
- Evaluar otra expresión.
- Ejecutar instrucciones de código en caso de que la expresión sea falsa o no se cumpla.

```ad-example
![[ArcoLinux_2022-08-24_11-21-34.png]]
```

### **Estructura de Decisión Múltiple**:
Este tipo de estructura permite seleccionar una, dentro de un conjunto de alternativas, con base en el valor almacenado, para evaluar las condiciones.

```ad-example
![[ArcoLinux_2022-08-24_11-26-36.png]]

Si la variable pasada en ==swith(variable)==, cumple con alguno de los casos creados, ejecutara dicha porcion de codigo y usara la palabra reservada **break;** para decirle al ==switch== que ya encontro el caso que cumple la condicion y que deje de buscar.
```

```ad-important
Si, la variable evaluada no cumple con ningudo de los casos, podemos definir un caso **default** que se ejecturar solo si, no se cumple la condicion con ninguno de los casos.

```ad-example
~~~ Java
	switch(variable) {
		case 1: 
			// Instrucciones de codigo
			break;
		case 2:
			// Instrucciones de codigo
			break;
		default:
			// Instrucciones de codigo si, ninguno
			// Ninguno de los casos cumple la condicion
			break;
	}
~~~
```
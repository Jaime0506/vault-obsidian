# **Scanner**

Scanner es una clase pre definida en Java que nos permite recibir datos de entrada a través de la consola.
- **Ejemplo**:
~~~Java
import java.util.Scanner;

public class Ejemplo {	
	public Ejemplo() {
		Scanner sc = new Scanner(System.in);

		System.out.println("Digite su nombre");

		String nombre = sc.nextLine();

		System.out.println("" + nombre);
	}
	
	public static void main(String[] args) throws Exception {
		Ejemplo result = new Ejemplo();	
	}
}
~~~

```ad-info
El escaner es una clase en Java, donde permite leer entradas del usuario, pero, dicha clase contiene diversos metodos para cada tipo de dato, boolean, String, double, int, se debe tener muy encuenta el tipo de dato esperado que va a digitar el usuario, para evitar errores.
```

En el ejemplo anterior, creamos un objeto a partir de la Clase Scanner y esto objeto, heredara todas las propiedades y atributos de dicha Clase, de tal manera que nos permitirá leer datos de los usuario a través de la consola de formas muy sencilla. 

```ad-attention
title: Variable sc
Para este ejemplo hemos usado la variable de tipo Scanner para inicializar la Clase Scanner
```

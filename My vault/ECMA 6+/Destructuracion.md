# Destructuracion - Destructuring

La destructuracion como su propio nombre lo dice,  es separar, desarmar o  extraer. En el caso de JavaScript en ECMAScript 6 se introdujo este nuevo concepto, que permite extraer los valores que deseemos de un objeto o arreglo, para ser usado de manera mas sencilla.

- *Ejemplo:*

**Objetos**

~~~JavaScript
const objeto = {
	color: 'red',
	size: 16,
	price: 380,
}

const { color } = objeto

console.log(`El color del objeto es ${color}`)
~~~

==En este ejemplo en concreto, estamos extrayendo del objeto la propiedad color, ya que en este caso, es la única que deseamos manipular, ademas de que si necesitamos cambiar esta propiedad posteriormente evitaremos el código repetitivo de==  **objeto.color**

**Arreglos**

~~~JavaScript
const arreglo = [
    cosa = {
	    color: 'orange',
	    size: 12,
	    price: 200
    },
    {
	    author: {
			nombre: 'Jaime'
	    } 
    }
]
~~~

==En el ejemplo con arreglos, podemos ver que tenemos múltiples objetos y valores dentro de este y puede ser molesto estar apuntando al indice que necesitemos cada vez que debamos llamar o cambiar algún valor==

- Para esto podemos destructurar, de acuerdo a su posición, y así poder acceder a este valor de forma sencilla en el resto de nuestro código.

~~~JavaScript
const [item1, item2] = arreglo

/*  item1 = {
		color: 'orange',
	    size: 12,
	    price: 200
	}

	item2 = { nombre: 'Jaime'}
/
~~~

- Ademas podemos jugar con la concadenacion de destructuraciones.

~~~JavaScript
	const [item1, item2] = arreglo

	const { color, size, price } = item1

	// o podemos destructurarlo directamente del arreglo de la 
	// siguiente manera

	const [{ color, size, price }, item2] = arreglo
~~~

- y en objetos dentro de mas objetos de la siguiente manera.

~~~JavaScript
const objeto = {
	cosa: {
	  color: 'orange',
	  size: 12,
	  price: 200
	},
	creador: {
	  author: {
		nombre: 'Jaime'
	  } 
	}
}

const {cosa: { color }, creador: { author: { nombre } }} = objeto
~~~
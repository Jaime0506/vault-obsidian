# Props
[[React]] al ser una librería que permite componetizar nuestro código, debemos tener una manera de pasar información de un componente padre a un componente hijo de forma sencilla.

En react tenemos los props, que es donde llegan los valores, varariables, funciones o propiedades a nuestros componentes hijos, del componente padre.

**Ejemplo**

- ==Componente padre==
~~~jsx
import { Child } from './child'

export const Father = () => {
	return(
		<div>
			<h1>
				Este es el componente padre
			</h1>
			<Child 
				title='Soy el componente hijo'
			/>
		</div>
	)
}
~~~

- ==Componente hijo==
~~~jsx
	export const Child = (props) => {
		
		const { title } = props
		
		return (
			<div>
				<h1>{ titlle }</h1>
			</div>
		)
	}
~~~

En el ejemplo anterior, el padre esta renderizando al componente hijo, pasandole unas props, en este caso la propiedad title, con un valor definido.

Esta propiedad queda en los parámetros que le hemos creado en la función, para que pueda ser llamada y utilizada en el hijo.

En el ejemplo anterior pasamos title, llamamos al objeto props y de este destructuramos la propiedad title, que fue la que le pasamos desde el padre, de esta manera podemos utilizar la propiedad con dicho valor. 

--- 

**(NOTA)**: actualmente es recomendable destructurar los valores directamente en el objeto props, ya que cada vez es menos usada la manera tradicional de hacerlo.

*Ejemplo:* 

~~~jsx

// de esta manera accedemos directamente a las propiedades
// pasadas de componentes padre.

	export const Child = ({ title }) => {

		//const { title } = props 
		
		return (
			<div>
				<h1>{ titlle }</h1>
			</div>
		)
	}
~~~

> debemos conocer como destructurar objetos y arreglos [[Destructuracion]].

Para exigir parámetros desde los componentes hijos, que sean obligatorios y de un tipo de dato en especifico, tenemos [[PropTypes]].
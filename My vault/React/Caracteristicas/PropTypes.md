# PropTypes

[[React]]

En JS , no tenemos tipado fuerte, por lo cual se puede prestar para errores, o comportamientos inesperado entre nuestro componentes, para esto existe la librería prop-types.

Instalación:

- npm:
~~~
npm i prop-types
~~~

- yarn:
~~~
yarn add prop-types
~~~
prop-types nos permite darle tipado fuerte a nuestras [[Props]], que pasamos entre componentes.

~~~JavaScript
import PropTypes from 'prop-types'

Component.propTypes = {
	value: PropTypes.string,
	value2: PropTypes.string.isRequired
}
~~~
> **Component**: viene siendo el nombre de nuestro componente **JSX**, importamos PropTypes de prop-types y lo usamos accediendo a la propienda propTypes de nuestro componente.

Definimos el tipo de dato a nuestros respectivos props y si es requerido.

- Ejemplo de uso de PropTypes:

Componente <Card /> que resive como props { name, edad, getData }
~~~JavaScript
import PropTypes from 'prop-types'

export const Card = ({ name, age, getData }) => {

	return (
		<div>
			<h1>{ name }</h1>
			<p>{ age }</p>
			<button onClick={ getData } />
		</div>
	)
}

Card.propTypes = {
	name: PropTypes.string,
	age: PropTypes.number,
	getData: PropTypes.func.isRequired //Pedimos que por props nos llegeue esa propieda obligatoria mente y que sea de tipo func (function)
}
~~~

De esta manera, gracias a la librería prop-types podemos darle tipado mas fuerte a los props de nuestros componentes **JSX** en **ReactJS**

==En la pagina oficial se encuentra la documentación mas detallada y completa de las funciones y utilidades de la librería.==

[prop-types Documentacion](https://www.npmjs.com/package/prop-types)

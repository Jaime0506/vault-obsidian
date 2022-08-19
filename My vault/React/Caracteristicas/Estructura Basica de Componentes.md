# Estructura Básica de Componentes

En React existen dos tipo de componentes, de clase y de función, en esta caso explicare solo de función ya que los componentes de clase están quedando obsoletos y los propios desarrolladores de React recomiendan los componentes de función.

**Ejemplo:**
~~~jsx

export const ComponenteEjemplo = () => {
	return (
		<div>
			<h1>Esto es un componente</h1>		
		</div>
	)
}
~~~

~~~jsx
export default function ComponenteEjemplo() {
	return (
		<div>
			<h1>Esto es un componente</h1>		
		</div>	
	)
}
~~~

> Para usar nuestros componentes en los demás componentes debemos necesariamente exportarlos, ya sea como default o como objeto.

DEBE HACER GIT


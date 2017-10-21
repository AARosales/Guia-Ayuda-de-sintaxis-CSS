## ÍNDICE DE CONTENIDOS
 1. Introducción al CSS.
 2. ¿Cómo es CSS? Sintaxis general.
 3. Reglas.
 4. Selectores.
 5. Class.
 6. Div y Span.
 7. Uso de las hojas de estilo. 

   ## Introducción al CSS.

    ### CSS (CASCADING STYLE SHEETS)
	- Nace en torno a 1995. En 1996 el W3C publica la
	primera recomendación oficial “CSS nivel 1”.
	- Actualmente se trabaja en la versión CSS3.
	- Permite definir el aspecto visual de una página HTML o
	XHTML.
	- Antes de CSS la estructura de las páginas era definida
	mediante tablas.

   ### HTML + CSS
	- HTML define el marcado de los contenidos, es decir, qué es un
	párrafo, un titular o una lista.
	- CSS define el aspecto de todos los contenidos, es decir, color,
	tamaño y tipo de letra de los párrafos de texto, separación
	entre titulares y párrafos, tabulación entre los elementos de
	una lista, etc.
	- Es la mejor forma de separar los contenidos de la presentación
	lo que conlleva las siguientes ventajas:
	- Obliga a crear HTML/XHTML bien definidos (o “semánticos”).
	- Mejora la accesibilidad, reduce la complejidad de su mantenimiento
	y permite visualizar el mismo documento en diferentes dispositivos.

   ## ¿Cómo es CSS?
    
    ### ...cómo es CSS?
	- Se trata de un fichero de texto plano que contiene “reglas”.
	- Cada regla tiene dos partes:
		- Selector (para seleccionar las etiquetas HTML sobre las que actúa).
	        - Descriptor (para decir qué hace con ellas)
		   h1: {color:green; font-family:Verdana}
	- El fichero CSS es una lista de reglas (pares selector+descriptor)
		- Los selectores pueden ser una o varias etiquetas HTML.
		- Los descriptores están definidos en CSS, hay una larga lista.

    ### ...cómo es CSS? (II)
	- Las reglas CSS:
		- selector {propiedad: valor}
		- selector, selector, …, selector {
	           propiedad: valor;
	           …
	           propiedad: valor;
	           } 
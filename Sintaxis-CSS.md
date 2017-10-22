## ÍNDICE DE CONTENIDOS
 1. Introducción al CSS.
 2. ¿Cómo es CSS? Sintaxis general.
 3. Reglas.
 4. Selectores.
 5. Class.
 6. Div y Span.
 7. Uso de las hojas de estilo. 

   ## Introducción al CSS.

   #### CSS (CASCADING STYLE SHEETS)
	- Nace en torno a 1995. En 1996 el W3C publica la
	primera recomendación oficial “CSS nivel 1”.
	- Actualmente se trabaja en la versión CSS3.
	- Permite definir el aspecto visual de una página HTML o
	XHTML.
	- Antes de CSS la estructura de las páginas era definida
	mediante tablas.

   #### HTML + CSS
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
    
   #### ...cómo es CSS?
	- Se trata de un fichero de texto plano que contiene “reglas”.
	- Cada regla tiene dos partes:
		- Selector (para seleccionar las etiquetas HTML sobre las que actúa).
	        - Descriptor (para decir qué hace con ellas)
		   h1: {color:green; font-family:Verdana}
	- El fichero CSS es una lista de reglas (pares selector+descriptor)
		- Los selectores pueden ser una o varias etiquetas HTML.
		- Los descriptores están definidos en CSS, hay una larga lista.

   #### ...cómo es CSS? (II)
	- Las reglas CSS:
		- selector {propiedad: valor}
		- selector, selector, …, selector {
	           propiedad: valor;
	           …
	           propiedad: valor;
	           } 
## CLASS
		
   #### EL ATRIBUTO CLASS
	- El atributo “class” permite tener diferentes estilos para
	elementos del mismo tipo.
	  - HTML
	   <p class = “importante”>Este párrafo aparecerá en negrita y grande</p>
	   <p class = “normal”>Este párrafo aparecerá sin negrita y pequeño</p>
	  - CSS
	    p.importante { font-weight: bold; font-size: 24pt; }
	    p.normal { font-size: 10pt; }
	- Para definir una regla que aplique a cualquier elemento de
	una clase concreta se puede usar indiferentemente:
	  - .importante { font-weight: bold; font-size: 24pt; }
	  - *.importante { font-weight: bold; font-size: 24pt; }

   #### EL ATRIBUTO CLASS (II)
	- Ejemplo:
	  - CSS
	   *.coloreado { color: red; }
	   h1.coloreado { color: green; }
	  - HTML
	   <h1>no aparece de ni rojo ni verde</h1>
	   <h1 class = “coloreado”>aparece verde</h1>
	   <p class = “coloreado”>aparece rojo</p>

#### EL ATRIBUTO CLASS (III)
	- Subconjunto del atributo “class”:
	  - CSS
	   p.importante.coloreado { color: green; }
	   _Regla:_ que sea al menos de la clase importante y coloreado.
	- HTML
	 <p class = “importante grande coloreado”>sale verde </p>	
	 <p class = “importante grande ”>NO sale verde</p>
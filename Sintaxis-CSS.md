## �NDICE DE CONTENIDOS
 1. Introducci�n al CSS.
 2. �C�mo es CSS? Sintaxis general.
 3. Reglas.
 4. Selectores.
 5. Class.
 6. Div y Span.
 7. Uso de las hojas de estilo. 

   ## Introducci�n al CSS.

   #### CSS (CASCADING STYLE SHEETS)
	- Nace en torno a 1995. En 1996 el W3C publica la
	primera recomendaci�n oficial �CSS nivel 1�.
	- Actualmente se trabaja en la versi�n CSS3.
	- Permite definir el aspecto visual de una p�gina HTML o
	XHTML.
	- Antes de CSS la estructura de las p�ginas era definida
	mediante tablas.

   #### HTML + CSS
	- HTML define el marcado de los contenidos, es decir, qu� es un
	p�rrafo, un titular o una lista.
	- CSS define el aspecto de todos los contenidos, es decir, color,
	tama�o y tipo de letra de los p�rrafos de texto, separaci�n
	entre titulares y p�rrafos, tabulaci�n entre los elementos de
	una lista, etc.
	- Es la mejor forma de separar los contenidos de la presentaci�n
	lo que conlleva las siguientes ventajas:
	- Obliga a crear HTML/XHTML bien definidos (o �sem�nticos�).
	- Mejora la accesibilidad, reduce la complejidad de su mantenimiento
	y permite visualizar el mismo documento en diferentes dispositivos.

   ## �C�mo es CSS?
    
   #### ...c�mo es CSS?
	- Se trata de un fichero de texto plano que contiene �reglas�.
	- Cada regla tiene dos partes:
		- Selector (para seleccionar las etiquetas HTML sobre las que act�a).
	        - Descriptor (para decir qu� hace con ellas)
		   h1: {color:green; font-family:Verdana}
	- El fichero CSS es una lista de reglas (pares selector+descriptor)
		- Los selectores pueden ser una o varias etiquetas HTML.
		- Los descriptores est�n definidos en CSS, hay una larga lista.

   #### ...c�mo es CSS? (II)
	- Las reglas CSS:
		- selector {propiedad: valor}
		- selector, selector, �, selector {
	           propiedad: valor;
	           �
	           propiedad: valor;
	           } 
## CLASS
		
   #### EL ATRIBUTO CLASS
	- El atributo �class� permite tener diferentes estilos para
	elementos del mismo tipo.
	  - HTML
	   <p class = �importante�>Este p�rrafo aparecer� en negrita y grande</p>
	   <p class = �normal�>Este p�rrafo aparecer� sin negrita y peque�o</p>
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
	   <h1 class = �coloreado�>aparece verde</h1>
	   <p class = �coloreado�>aparece rojo</p>

#### EL ATRIBUTO CLASS (III)
	- Subconjunto del atributo �class�:
	  - CSS
	   p.importante.coloreado { color: green; }
	   _Regla:_ que sea al menos de la clase importante y coloreado.
	- HTML
	 <p class = �importante grande coloreado�>sale verde </p>	
	 <p class = �importante grande �>NO sale verde</p>

## Div y Span.

   #### LAS ETIQUETAS <DIV> Y <SPAN>
	- <div> y <span> son etiquetas HTML que permiten aplicar
	  reglas CSS a diferentes elementos:
	  - <div> asegura que habr� una nueva l�nea antes y despu�s del
	    bloque.
	  - <span> no a�ade l�neas antes ni despu�s, solo espacios simples.
	    Ejemplo:
	  - CSS
	     div { background-color: #66FFFF; }
	     span.color { color: red; }
	  - HTML
	     <div>Este div se trata como un p�rafo con fondo de color pero
	     <span class = �color�>este span aparece con letras
	     rojas.</span></div>

   #### EL SELECTOR ID
	- Este selector se usa para aplicar estilo a un elemento
	  concreto.
	  - CSS
	    #cabecera { width: 740px; top: 0px; }
	  - HTML
	    <div id = �cabecera�>Esta divisi�n o �caja� tiene que aparecer
	    con un ancho de 740px y situado en la parte superior</div>


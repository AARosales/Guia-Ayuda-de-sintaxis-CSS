## ÍNDICE DE CONTENIDOS
 1. Introducción al CSS.
 2. ¿Cómo es CSS? Sintaxis general.
 3. Reglas.
 4. Selectores.
 5. Class.
 6. Div y Span.
 7. Uso de las hojas de estilo. 

##CAPÍTULO 3

## EJEMPLOS DE REGLAS
 h1, h2, h3 { font-family: helvetica }
 h1 {
font-weight: bold;
font-size: 12pt;
line-height: 14pt;
font-family: helvetica;
font-variant: normal;
font-style: normal;
}

## EJEMPLOS DE REGLAS (II) -
#### HTTP://WWW.W3SCHOOLS.COM/CSS/DEMO_DEFAULT.HTM
h1,h2,h3 {
font-family: "lucida calligraphy", arial, 'sans serif';
}
p,table,li, {
font-family: "lucida calligraphy", arial, 'sans serif'; margin-left: 10pt;
}
body {
background-color:#fffaf0;
}
p,li,th,td {
font-size: 75%;
}
h1,h2,h3,hr {
color:#483d8b;
}
table { border-style:outset}
li {list-style: square;)}

## CAPÍTULO 4

## TIPOS DE SELECTORES
Podemos seleccionar un solo elemento HTML
 ul { list-style: disc; } (lista con círculo relleno)
 Seleccionar varios elementos HTML
 h1, h3{ font-family: verdana; } (ambos títulos con ese tipo de letra)
 Repetir selectores
 h1, h3{ font-family: verdana; }
 h1, h2, h3, hr { color: black; }
 Si un valor no coincide, la última regla es la que se tiene en cuenta.
 Utilizar el selector universal *. Se aplica a todos los elementos.
 * { color: green; }
 Si los valores no coinciden, prevalecen las reglas más específicas.

## HERENCIA EN SELECTORES
h1 { color: blue ; }
body { color: black; background: url(texture.gif) white; }
 Si no se especifica una propiedad, se hereda del elemento
padre:
<h1>El titular <em>es</em> corto</h1>
 “es” será azul porque <h1> es azul y <em> lo hereda por ser su hijo.
 La página tendría texto negro sobre fondo blanco en el caso de que
no se encuentre la imagen de fondo “texture.gif”.

## SELECTORES ADYACENTES
 Seleccionando elementos adyacentes o consecutivos que
están al mismo nivel (no son hijos unos de otros):
 HTML
<h1>Separa tras esta línea</h1>
<h2>Importante</h2>
<h2>Otro título</h2>
 CSS
h1 + h2 { margin-top: 11px; }
El efecto de la regla es un margen entre h1 y h2.

## SELECTOR ATRIBUTO
 Se selecciona un elemento que tenga un atributo:
 Sintaxis: elemento[atributo] { … }
 Ejemplo: table[border] { … }
 Se puede seleccionar una elemento que tenga un atributo
con un valor determinado:
 Sintaxis: elemento[atributo=“valor”] { … }
 Ejemplo: table[border = “0”] { … }

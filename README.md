# CSS-Selectors-con-CSS-Diner


### Resumen de los Selectores Aplicados.

------



**1-Seleccionar todos o un elementos.**

Selecciona todos los elementos del tipo A. Tipo se refiere al tipo de etiqueta, por lo que div, pag y ul. Son todos tipos de elementos diferentes.


### Ejemplo:

~~~
* {
  color: blue;
}
~~~

------

**2-Seleccionar elementos con un ID.**

Selecciona el elemento con un ID espesifico. También puedes combinar el selector de ID con el selector de tipo.


### Ejemplo:

~~~
#miId {
  background-color: yellow;
}
~~~

------

**3-Selector de descendientes.**

El selector de descendientes en CSS selecciona todos los elementos que son descendientes de un elemento específico. Este selector se representa con un espacio entre dos selectores.


### Ejemplo:

~~~
nav a {
  text-decoration: none;
}
~~~

------
**4-Combinación de selectores descendientes & selector ID.**

Permite aplicar estilos a elementos que son descendientes de un elemento específico identificado por su ID. Esto se logra utilizando una cadena de selectores donde un selector de ID especifica el elemento base y los selectores descendientes especifican los elementos dentro de ese elemento base que recibirán los estilos.


### Ejemplo:

~~~
#menu li {
  font-weight: bold;
}
~~~

------

**5-Selector de clases.**

El selector de clases en CSS se utiliza para seleccionar elementos HTML que tienen un atributo de clase específico. Esto permite aplicar estilos a uno o varios elementos que comparten la misma clase.


### Ejemplo:

~~~
.lista {
  list-style-type: none;
}
~~~

------

**6-Combinación del selector de clases.**
 
En CSS, puedes combinar selectores de clases con otros selectores (como selectores de tipo, ID, atributos, etc.) para aplicar estilos a elementos que cumplen con múltiples condiciones. Esto te permite una mayor precisión y control en la aplicación de estilos.


### Ejemplo:

~~~
.azul.destacado {
  color: blue;
  font-weight: bold;
}
~~~

------

**7-Combinador de comas y selectors.**

El combinador de comas en CSS permite aplicar los mismos estilos a múltiples selectores a la vez. Es útil para reducir la redundancia en el código y mantener la hoja de estilos más limpia y legible.


### Ejemplo:

~~~
h1, h2, h3 {
  font-family: Arial, sans-serif;
}
~~~

------

**8-Selector universal.**

 El selector universal en CSS selecciona todos los elementos de la página, sin importar el tipo, clase, ID u otros atributos. Es representado por un asterisco (*) y es útil cuando se necesita aplicar un estilo a todos los elementos de manera uniforme.


### Ejemplo:

~~~
* {
  margin: 0;
  padding: 0;
}
~~~

------
 
**9-Combinación de selector universal.**

La combinación del selector universal con otros selectores en CSS puede ser útil para aplicar estilos de manera específica a ciertos elementos o grupos de elementos. 


### Ejemplo:

~~~
div * {
  border: 1px solid black;
}
~~~

------

**10-Selector de hermanos adyacentes.**

El selector de hermanos adyacentes en CSS te permite seleccionar un elemento que es inmediatamente precedido por otro elemento específico. Se representa con el símbolo + .
 

### Ejemplo:

~~~
h2 + p {
  margin-top: 0;
}
~~~

------

**11-Selector general de hermanos.**

El selector general de hermanos en CSS te permite seleccionar todos los elementos que son hermanos de otro elemento específico, independientemente de su posición relativa. Se representa con el símbolo ~ .


### Ejemplo:

~~~
h2 ~ p {
  font-style: italic;
}
~~~

------

**12-Selector hijo.**

El selector hijo en CSS te permite seleccionar elementos que son hijos directos de otro elemento específico. Se representa con el símbolo >.


### Ejemplo:

~~~
ul > li {
  padding-left: 20px;
}
~~~

------

**13-Primer pseudoselector infantil.**

El pseudoselector :first-child en CSS te permite seleccionar el primer hijo de un elemento padre específico. Selecciona cualquier elemento que sea el primer hijo entre sus hermanos dentro de su contenedor.


### Ejemplo:

~~~
ul li:first-child {
  font-weight: bold;
}
~~~

------

**14-Pseudoselector de hijo único.**

El pseudoselector :only-child en CSS te permite seleccionar elementos que son hijos únicos de su elemento padre, es decir, aquellos que son el único hijo dentro de su contenedor.


### Ejemplo:

~~~
p:only-child {
  color: red;
}
~~~

------

**15-Pseudoselector del último hijo.**

El pseudoselector :last-child en CSS te permite seleccionar el último hijo de un elemento padre específico. Selecciona cualquier elemento que sea el último hijo entre sus hermanos dentro de su contenedor.


### Ejemplo:

~~~
p:last-child {
  font-style: italic;
}
~~~

------

**16-Pseudoselector enésimo hijo.**

El pseudoselector :nth-child() en CSS te permite seleccionar elementos que son el enésimo hijo de su elemento padre, donde "n" es un número o una fórmula algebraica. Esto te permite seleccionar elementos específicos basados en su posición dentro de su contenedor. 


### Ejemplo:

~~~
ul li:nth-child(2) {
  color: green;
}
~~~

------

**17-Enésimo último selector secundario.**

El pseudoselector :nth-last-child() en CSS es similar a :nth-child(), pero cuenta los elementos desde el final del conjunto de elementos secundarios en lugar del principio. Esto te permite seleccionar elementos específicos basados en su posición desde el final del contenedor. 


### Ejemplo:

~~~
ul li:nth-last-child(2) {
  background-color: yellow;
}
~~~

------

**18-Primer tipo de selector.**

El selector de tipo en CSS te permite seleccionar elementos basados en su tipo, es decir, el nombre del elemento HTML. 


### Ejemplo:

~~~
p:first-of-type {
  font-size: 20px;
}
~~~

------

**19-Selector enésimo de tipo.**

El pseudoselector :nth-of-type() en CSS te permite seleccionar elementos específicos basados en su tipo y su posición dentro de su contenedor. Esto te permite aplicar estilos a elementos específicos basados en su posición relativa respecto a otros elementos del mismo tipo dentro del mismo contenedor. 


### Ejemplo:

~~~
p:nth-of-type(odd) {
  background-color: lightgray;
}
~~~

------

**20-Selector de tipo enésimo con fórmula.**

El pseudoselector :nth-of-type((An+B)) en CSS admite fórmulas matemáticas para seleccionar elementos específicos basados en su tipo y su posición dentro de su contenedor. Esto te permite seleccionar elementos de manera más precisa utilizando una expresión matemática.


### Ejemplo:

~~~
p:nth-of-type(3n+1) {
  color: blue;
}
~~~

------

**21-Last of Type Selector.**


El pseudoselector :only-of-type en CSS selecciona elementos que son el único elemento de su tipo entre sus hermanos dentro de su contenedor. Esto significa que el elemento seleccionado es el único de su tipo dentro de su contenedor y no tiene otros elementos del mismo tipo como hermanos.


### Ejemplo:

~~~
p:last-of-type {
  text-align: right;
}
~~~

------

**22-Selector vacío.**

El selector vacío (:empty) en CSS te permite seleccionar elementos que no contienen ningún contenido, ya sea texto, elementos hijos u otros nodos. Esto puede ser útil para aplicar estilos a elementos que están vacíos en tu documento HTML. 


### Ejemplo:

~~~
div:empty {
  border: 1px dashed gray;
}
~~~

------


**23-Pseudoclase de negación.**

La pseudoclase de negación (:not()) en CSS te permite seleccionar elementos que no coinciden con un selector especificado. Esto es útil cuando deseas aplicar estilos a elementos que no cumplen con ciertos criterios de selección. 


### Ejemplo:

~~~
p:not(.importante) {
  color: gray;
}
~~~

------

**24-Selector de atributos.**

El selector de atributos en CSS te permite seleccionar elementos HTML que tienen un atributo específico y, opcionalmente, un valor específico para ese atributo. Esto es útil cuando deseas aplicar estilos a elementos basados en la presencia o valor de sus atributos.


### Ejemplo:

~~~
a[target="_blank"] {
  color: red;
}
~~~

------
**25-Selector de valor de atributo.**

El selector de valor de atributo en CSS te permite seleccionar elementos HTML que tienen un atributo específico con un valor específico. Esto es útil cuando deseas aplicar estilos a elementos que tienen un atributo con un valor particular.


### Ejemplo:

~~~
input[type="text"] {
  width: 200px;
}
~~~

------

**26-Attribute Starts With Selector.**

El selector de atributos que comienza con un valor específico en CSS te permite seleccionar elementos cuyo atributo comienza con cierto valor. Esto es útil cuando deseas aplicar estilos a elementos que tienen un atributo cuyo valor empieza con una cadena específica. 


### Ejemplo:

~~~
img[src^="https"] {
  border: 2px solid green;
}
~~~

------


**27-Attribute Ends With Selector.**

El selector de atributos que termina con un valor específico en CSS te permite seleccionar elementos cuyo atributo termina con cierto valor. Esto es útil cuando deseas aplicar estilos a elementos que tienen un atributo cuyo valor termina con una cadena específica. 


### Ejemplo:

~~~
a[href$=".pdf"] {
  color: blue;
}
~~~

------


**28-Attribute Wildcard Selector.**


El selector de atributos comodín en CSS te permite seleccionar elementos cuyo atributo contiene un valor específico en cualquier parte del texto del atributo. Esto es útil cuando deseas aplicar estilos a elementos que tienen un atributo que contiene una cadena específica en cualquier posición. 


### Ejemplo:

~~~
input[name*="pass"] {
  background-color: yellow;
}
~~~

------
------

## Score de niveles realizados:

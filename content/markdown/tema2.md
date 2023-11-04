+++
title = 'Usar Markdwon'
date = 2023-11-01T13:43:59+01:00
draft = false
+++
## Expliación de como usar Markdown
### Elementos de bloque

#### Parrafos y saltos de linea
Igual que en HTML, markdown no soporta dobles liineas en blanco.  
Para realizar un salto de linea tendras que usar doble espacio al final antes que pulses intro  


Si quisieras separar texos, recuerda siempre el doble espacio.  
para asi despues continuar en otra linea.


#### Titulos o Encabezados

Para crear titulos se usa almohadilla #.  
Para un titulo H1 se usa una almohadilla # Titulo  
Para uno H2 se usa dos ## Titulo  
Y asi hasta un H6, serian el numero de almohadillas del <<H>> que queremos
<!--
> encabezado 1: # Titulo H1     
> encabezado 2: ## Titulo H2  
> encabezado 3: ### Titulo H3     
> encabezado 4: #### Titulo H4  
> encabezado 5: ##### Titulo H5   
> encabezado 6: ###### Titulo H6   
-->
~~~ markdown
# Titulo H1     
## Titulo H2  
### Titulo H3     
#### Titulo H4  
##### Titulo H5   
###### Titulo H6   
~~~

El resulado seria:  
# Titulo H1
## Titulo H2  
### Titulo H3    
#### Titulo H4  
##### Titulo H5   
###### Titulo H6 

--- 

## Citas  
Las citas se pueden generar utilizando el caracter > al comienzo

~~~ markdown
> Esto es una cita de prueba.
~~~

El resultado seria asi:
> Esto es una cita de prueba.

Si la cita tiene varios parrafos se debe añadir el mismo simbolo > al comienzo de cada uno de ellos

~~~Markdown
> Esto es una cita de un primer parrafo   
> Esto es un segundo parrafo de texto
~~~  

El resultado es este:  

> Esto es una cita de un primer parrafo  
> Esto es un segundo parrafo de texto

Tambien se puede anidar una cita en otra usando doble >>
~~~ markdown
> Esto es una cita    
>> Con otra cita anidada como ejemplo.  
y puede seguir  
~~~

El resultado es asi: 
> Esto es una cita    
>> Con otra cita anidada como ejemplo.  
y puede seguir  
  
---

#### Listas


Se pueden crear listas, de manera muy sencilla, tanto ordenadas como desordenadas.  
##### Listas desordenadas
Para listas desordenadas usa * asteriscos, - guiones, o + simbolo de suma.

~~~ Markdown
* Manzanas
* Melocotones
- Peras
- Almendras
+ Uvas
+ Cerezas
~~~~
El resultado es asi:
* Manzanas
* Melocotones
- Peras
- Almendras
+ Uvas
+ Cerezas

###### Lista anidadas  
Para una lista anidada simplemente hay que añadir 4 espacios en blanco
~~~ Markdown
* Elemento 1
* Elemento 2
    * Elemento anidado 1
        * Elemento anidado 2
* Elemento 3
* Elemento 4
~~~

El resultado es asi:
* Elemento 1
* Elemento 2
    * Elemento anidado 1
    * Elemento anidado 2
* Elemento 3
* Elemento 4

##### Listas ordenadas
Para la listas ordenadas debes usar la  sintaxis tipo: <<numero>> y un punto. y el elemento. Tambien puedes combinar con listas desordenadas y anidarlas
~~~ markdown
1. Elemento 1
    1. Subelemento 1
    2. Subelemento 2
2. Elemento 2
    * Subelemento 3
        * Subelemento 4
3. Elemento 3
4. Elemento 4
~~~
El resultado es asi:
1. Elemento 1
    1. Subelemento 1
    2. Subelemento 2
2. Elemento 2
    * Subelemento 3
        * Subelemento 4
3. Elemento 3
4. Elemento 4

--- 

#### Códigos de bloque

Si quieres insertar un bloque que contenga código, deberas "encerrar" ese codigo entre 3 simbolos ~ << virgulillas>>  
Si quieres especificar el codigo ,en la pimera linea de virgulillas puedes especificarlo

~~~ html
    ~~~ html
    <h1> titulo principal </h1>
    <p class="texto1"> parrafo </p>
    ~~~
~~~

~~~ java
    ~~~ java
    for(int i=0, x < i, i++){
    System.out.println(x)}
    ~~~
~~~
El resultado queda asi:
~~~ html
<h1> titulo principal </h1>
<p class="texto1"> parrafo </p>
~~~

~~~ java
for(int i=0, x < i, i++){
System.out.println(x)}
~~~

---
#### Reglas horizontales

Para crear una regla o division horizonal en Markdown es simplemente poner tres guiones <<- - ->>
~~~ markdown

---

~~~
El resultado:


---

Y asi ya puedes incluir reglas horizontales

---
### Elementos de linea
##### Enfasis, negritas y cursivas


Para poder escribir palabras o frases en negrita o cursiva se utiliza el simbolo <<*>> asterisco o <<_>> guion bajo, dependiendo de cuantos sera negrita, cursiva o ambas.

~~~ markdown
*cursiva*
**negrita**
_cursiva_
__negrita__
***negrita y cursiva***
___negrita y cursiva___
~~~
El resultado es este:
*cursiva*  
**negrita**  
_cursiva_  
__negrita__  
***negrita y cursiva***  
___negrita y cursiva___  


##### Enlaces o Links

Para añadir enlaces a una publicacion o una web la forma de hacerla es la siguiente.  
se escribe la palabra enlazada entre corchetes <<[]>> y el link entre parentesis <<()>>
~~~ markdown
[google](https://www.google.es)
~~~
El resultado es el siguiente:  
[google](https://www.google.es)

##### Código 

Para poder añadir secciones donde mostrar otro codigo de lenguaje, podras usar las comillas sencillas en HTML seria `<code>`  
en Markdown usaras <<`>>

~~~markdown
`<h3>`
`<javascript>`
`system.out.println("Hola mundo")`
~~~

El resultado seria:  
`<h3> </h3>`  
`<style> </style>`  
`system.out.println("Hola mundo")`  

Puedes usar este metodo para introducir `<p> pates de codigo </p>` entre las lineas que escribes.

##### Imágenes

Para introducir imagenes en Markdown es tan sencillo como incluir el simbolo de excalamacion al principo <<!>> y el enlace a la ubicación de la imagen entre parentesis <<( )>>, tambien es conveniente añadir entre corchetes <<[ ]>> un texto alternativo.  
Tambien podriamos poner una ruta a una web, añadiendo el correspondiente https://...


~~~ markdown
![Logo de Markdown](/markdown/logo.png)
~~~
con una imagen se veria asi:
![Logo de Markdown](/markdown/logo.png)


---

Y esto seria por encima una explicación de como podemos usar Markdown.
# Tema: Análisis de mercado de Ropa para Tallas Extra (Parte 2)

<img src="https://github.com/Deltarios/Deltarios.github.io/blob/master/assets/img_street.png" align="right" height="250" width="350" hspace="10">
<div style="text-align: justify;">
  
 ### Introducción:
 
 ### Por una publicidad (para tiendas de ropa) inteligente y efectiva basado en datos y análisis.

Con base al desarrollado en [**`la primera etapa del módulo`**](https://github.com/Deltarios/analisis-ropa-bedu), nuestro proyecto tomó como estudio dos condiciones que son consideradas potencialmente una problemática creciente en México.

- La obesidad.
- El sobrepeso.

#### El análisis se encuentra específicamente enfocado en el siguiente tópico:

> En el sector textil y su ámbito de la industria de la confección, analizando la escasa  oferta y comercialización de sucursales enfocadas a la venta de __Ropa de Talla Extra__ que son cada vez más solicitadas en personas desde  temprana edad y de manera constante en la edad adulta.

_En la primera parte del proyecto se obtuvo mediante el análisis de 4 variables un top 5 de estados_ [**`Ver Aquí`**](https://axel-flores.shinyapps.io/TallasExtraXL)


---
### Integrantes: 

- Axel Flores Guarneros.
- Marco Antonio Armas Santillán.
- Ariel Arturo Ríos Sierra.  
- Evelyn Jocelyn Gonzalez Acevedo

---
### Contenido del Repositorio:

> NOTA: Los archivos **`Proyecto.ipynb`** y **`Scrapping_google_populartimes.ipynb`** pueden tardar en cargar en github, reintentar abrir si marca error de lo contrario abrilos en [**`Colab by Google`**](https://colab.research.google.com/)

-  [**`Proyecto.ipynb`**](proyecto/Proyecto.ipynb)
   Contiene todas las gráficas y resultados sobre puntos estrategicos generados por el estudio de mercado del estado de Nuevo León. [**`Ver en Colab Aquí`**](https://colab.research.google.com/github/Deltarios/analisis_ropa_bedu_2/blob/master/proyecto/Proyecto.ipynb)
   
-  [**`Scrapping_google_populartimes.ipynb`**](proyecto/Scrapping_google_populartimes.ipynb)
   Contiene la metodología para extraer la información del API de google relacionada a las riendas de ropa del estado de Nuevo León. [**`Ver en Colab Aquí`**](https://colab.research.google.com/github/Deltarios/analisis_ropa_bedu_2/blob/master/proyecto/Scrapping_google_populartimes.ipynb)
   
-  [**`puntos_clave_publicidad.html`**](proyecto/puntos_clave_publicidad.html)
   Mapa con los resultados sobre puntos estrategicos generados por el estudio de mercado del estado de Nuevo León (Se generá igualmente con     [**`Proyecto.ipynb`**](proyecto/proyecto.ipynb)).

-  [**`Archivos NUEVOLEON2`**](proyecto/Scrapping_google_populartimes.ipynb)
   Archivos necesarios para hacer correr el script [**`Proyecto.ipynb`**](proyecto/proyecto.ipynb) <span style="color:red;">*importante que esten en la misma carpeta.</span>

-  [**`Datasets`**](dataset)
   Grupo de datasets utilizados en el proyecto (El código se llaman en red, pero se incluye los datasets de la información si se requieren).
   
---
### Desarrollo: 

> NOTA: Esto es en modo de resúmen, dentro de Scripts **`Proyecto.ipynb`** y **`Scrapping_google_populartimes.ipynb`** se encuentra explicado cada detalle de la obtención de la información.

#### _¿Cuáles son los pasos y objetivos de nuestro  estudio?_

- Mediante un estudio se encontrará la ubicación  geográfica puntual a nivel municipal para la apertura del establecimiento, asimismo encontrando puntos de publicidad para la  difusión del concepto de la Comercialización  de tallas extras.

- Tomar la opción que englobe todas las ventajas tanto para la parte comercializadora como para el consumidor en la creación de un concepto como una marca específica que se inserte en el mercado, y en los establecimientos ya aberturados que cuenten con mayor tiempo en el mercado y además con cierto prestigio, así ofertando en una misma línea "Marca y  Publicidad" lo que implicaría una reducción de costos.

- Selección puntual de la ubicación de la tienda
_(Para poder llevar a cabo estos dos puntos se procedió elegir un estado del Top 5 generado en el proyecto anterior para su análisis.)_

- Este estado fue __NUEVO LEÓN__.

#### _¿Por que Nuevo Leon?_

Fue elegido debido a que dentro del TOP y de los 32 estados es aquel que lidera el ranking con el mayor Índice Progreso Social, el cual está relacionado con el desempeño económico del país y así mismo es un indicador para  evaluar la calidad de vida de la población.

Una vez seleccionado nuestro Estado se procedió a comprar una Base de datos relacionada con el tema a investigar del estado seleccionado.

#### _API_

La API de lugares de Google permite a los desarrolladores acceder a una gran cantidad de información de la base de datos de Google, incluidos datos de ubicación, información de contacto, calificaciones, horarios pico, tiempo promedio de estancia, número de comentarios principalmente.

Se utilizó el API de LivePopularTimes https://github.com/GrocerCheck/LivePopularTimes la cual hace vez hace un data scraping de Google Maps con base en la dirección de las tiendas de ropa.

Por medio de la API de Google analizando 4000 tiendas de ropa del estado de Nuevo leon realizando un filtrado con 4 parámetros 
- Porcentaje de Obesidad por municipio.
- Número por municipio.
- Concentración de tiendas por colonia.
- Concentración de tiendas por municipio.

Las tiendas de tamaño grande y mediano se seleccionan por Default, Se realizó un merge con el porcentaje de obesidad, numero de ventas por municipio y cantidad  de concentración de tiendas por colonia, para poder elegir de forma adecuada las tiendas de categoría pequeña. 

Todas estas variables nos ayudaron a realizar una elección de una forma más consciente y exacta, basada en datos duros la elección de los puntos de interés de las tiendas de ropa.

Se obtuvo como resultado final un listado del contacto de las tiendas en 5 de los 51 municipios de nuevo león.  
- Monterrey. 
- Cadereyta Jiménez.
- San Nicolás De Los Garza.
- General Escobedo.
- San Pedro Garza García. 

Dicha lista se utilizará para contactar a las tiendas ubicadas  en los 5 municipios y poder ofrecer nuestra línea para su difusión en tiendas físicas. Ya que como marca se busca no solo tener una tienda establecida sino crear una red de ventas con otras establecimientos de ropa que estuvieran interesadas en crear una colaboración comercial.

#### _Publicidad a nivel Puntual_

Se busca encontrar los puntos con mejor calificación así como los horarios en los que se encuentra mayor número de usuarios en dichos puntos.
Estos puntos concurren en el punto no solo de rentabilidad , también  altamente seguro y eficiente en aspectos publicitarios.

De las tiendas de ropa dentro de la base de datos se aplicó un filtro para encontrar los lugares en donde dichas tiendas tuvieron las mejores calificaciones y números de comentarios de acuerdo a la API de Google. Se tomó en cuenta un mínimo de calificación de __4.5 y mínimo 70 comentarios del recinto.__ 

El API de Google nos arroja en qué horarios es mayor o menor el número de usuarios, es decir, ___¿Cual es la hora donde hay mayor afluencia de posibles compradores?___, al conocer estos puntos estratégicos y los horarios en los que hay mayor número de personas podremos saber cuáles puntos y horarios son clave para repartir o colocar propaganda de nuestra tienda y de esta forma los usuarios puedan conocer nuestro producto o utilizarse para implementar medidas publicitarias que pueden ir desde la repartición de volantes, hasta anuncios físicos.

---
## Problemas en el desarrollo

- Debido a que las bases de datos de registros de empresas solo se pueden obtener mediante la compra de las mismas a terceros , se tuvo que recurrir a la compra de registros de Telemarketing para tener mejor precisión de los datos.
- Debido a que se utilizo la API de Google , se tuvo que tener cuidado por su limitado número de peticiones.

---
## ¿Qué es lo que sigue en nuestro estudio?

- A que publico va dirigido.
- ecommerce.

Es importante mencionar que una vez seleccionado los locales, tenemos que proceder a delimitar el sector al que principalmente va dirigido nuestro producto. Para esto, se tomó de referencia el Estudio del ingreso promedio trimestral (2018) por entidad federativa que nos permitió observar un incremento sustancial entre las edades de 20 a 40 años tanto para  hombres y mujeres, por lo que podemos inferir que el público entre estas edades tiene una mayor capacidad adquisitiva, sin una responsabilidad familiar directa, que les permite acceder a una compra con mayor recurrencia.

Aunado a esto, la percepción positiva que se tiene en México sobre la apertura al mundo digital, así como el aumento exponencial del uso de internet en México en los últimos años se ha convertido en factores sustanciales en el auge de las ventas en línea de toda clase de productos, y la venta de ropa en línea no es la excepción, es por ello que dentro del proyecto también nos enfocamos en la posibilidad de implementar la venta de ropa de tallas extra en línea, impulsando su popularidad a través de la difusión de su publicidad en lugares estratégicos. 

Respecto a las ecommerce se debe tener en cuenta que en México, las medianas y grandes empresas se han posicionado en la transformación digital en los últimos años,actualmente el comercio electrónico ha ido en aumento, esto promete permanecer a largo plazo derivado del impacto positivo y acelerado del número de visitas y ventas en línea que muchas empresas con ventas online han vivido.
Se muestra en la siguiente gráfica el un incremento sustancial en el uso del Internet en Mexico , además se analizo una encuesta realizada en 2015 sobre su opinión del uso de las herramientas o servicios digitales en distintos países. En nuestro caso solamente selecionamos los valores de méxico de 6 afirmaciones que se les plantearon a los participantes. 
Para más detalles: [**`Aquí`**](https://read.oecd-ilibrary.org/education/pisa-2015-results-volume-iii_9789264273856-en#page1)

### La importancia de estos estudios
Aunque las ventas online ya eran una tendencia creciente, el confinamiento ha acelerado los cambios en los hábitos de los consumidores y muchos de estos cambios se quedarán con nosotros en el futuro por ello es importante 

# Tema: Análisis de mercado de Ropa para Tallas Extra (Parte 2)

<img src="https://github.com/Deltarios/Deltarios.github.io/blob/master/assets/img_street.png" align="right" height="250" width="350" hspace="10">
<div style="text-align: justify;">
  
 ### Introducción:

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

---
### Desarrollo: 

¿Cuáles son los pasos y objetivos de nuestro  estudio?

- Mediante un estudio se encontrará la ubicación  geográfica puntual a nivel municipal para la apertura del establecimiento, asimismo encontrando puntos de publicidad para la  difusión del concepto de la Comercialización  de tallas extras.

- Tomar la opción que englobe todas las ventajas tanto para la parte comercializadora como para el consumidor en la creación de un concepto como una marca específica que se inserte en el mercado, y en los establecimientos ya aberturados que cuenten con mayor tiempo en el mercado y además con cierto prestigio, así ofertando en una misma línea "Marca y  Publicidad" lo que implicaría una reducción de costos.

- Selección puntual de la ubicación de la tienda
_(Para poder llevar a cabo estos dos puntos se procedió elegir un estado del Top 5 generado en el proyecto anterior para su análisis.)_

- Este estado fue __NUEVO LEÓN__.

¿Por que Nuevo Leon?

Fue elegido debido a que dentro del TOP y de los 32 estados es aquel que lidera el ranking con el mayor Índice Progreso Social, el cual está relacionado con el desempeño económico del país y así mismo es un indicador para  evaluar la calidad de vida de la población.

Una vez seleccionado nuestro Estado se procedió a comprar una Base de datos relacionada con el tema a investigar del estado seleccionado.

#### API

La API de lugares de Google permite a los desarrolladores acceder a una gran cantidad de información de la base de datos de Google, incluidos datos de ubicación, información de contacto, calificaciones, horarios pico, tiempo promedio de estancia, número de comentarios principalmente.

Se utilizó el API de LivePopularTimes https://github.com/GrocerCheck/LivePopularTimes la cual hace vez hace un data scraping de Google Maps con base en la dirección de las tiendas de ropa.

Por medio de la API de Google analizando 4000 tiendas de ropa del estado de Nuevo leon realizando un filtrado con 4 parámetros 
- Porcentaje de Obesidad por municipio.
- Número por municipio.
- Concentración de tiendas por colonia.
- Concentración de tiendas por municipio.

Las tiendas de tamaño grande y mediano se seleccionan por Default, Se realizó un merge con el porcentaje de obesidad, numero de ventas por municipio y cantidad  de concentración de tiendas por colonia, para poder elegir de forma adecuada las tiendas de categoría pequeña. 

Todas estas variables nos ayudaron a realizar una elección de una forma más consciente y exacta, basada en datos duros la elección de los puntos de interés de las tiendas de ropa.

---
## Problemas en el desarrollo

- Debido a que las bases de datos de registros de empresas solo se pueden obtener mediante la compra de las mismas a terceros , se tuvo que recurrir a la compra de registros de Telemarketing para tener mejor precisión de los datos.
- Debido a que se utilizo la API de Google , se tuvo que tener cuidado por su limitado número de peticiones.

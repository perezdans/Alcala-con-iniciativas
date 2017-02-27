![Logo CIVICS](http://www.viveroiniciativasciudadanas.net/civics/img/civics_logo_medio.png "Imagen del Logo CIVICS")

# Alcalá con Iniciativas

Alcalá con Iniciativas es una plataforma donde encontrarás información geolocalizada de las iniciativas de Alcalá de Henares. Desde el mapa puedes acceder a un formulario realizado con Google Docs para dar de alta nuevas iniciativas.

Se encuentra disponible en: [asociacionsimbiosis.org/alcala-con-iniciativas/](http://asociacionsimbiosis.org/alcala-con-iniciativas/)

Para una descripción detallada de las tablas de datos y de sus atributos consulta el documento [DatasetDescription.md](https://github.com/perezdans/Alcala-con-iniciativas/blob/master/DatasetDescription.md)

---
# Indice para este documento

[Mapa de iniciativas](#mapa-de-iniciativas)

* [Funcionalidades del mapa de iniciativas](#funcionalidades-del-mapa-de-iniciativas)
* [Descripción de los documentos del mapa de iniciativas](#descripción-de-los-documentos-del-mapa-de-iniciativas)
* [Dependencias](#dependencias)

[Formulario de entrada de nuevas iniciativas](#formulario-de-entrada-de-nuevas-iniciativas)

* [Descripción de los documentos del formulario de entrada de nueva iniciativa](#descripción-de-los-documentos-del-formulario-de-entrada-de-nueva-iniciativa)
* [Dependencias](#dependencias-1)


[Acerca de los datos](#acerca-de-los-datos)

* [Fuente de los datos](#fuente-de-los-datos)
* [Acceso a los datos](#acceso-a-los-datos)
* [Descripción de los datos](#descripción-de-los-datos)

[Equipo de desarrollo de la versión alpha v3](#equipo-de-desarrollo-de-la-versión-alpha-v3)

[Licencias](#licencias)

---
# Mapa de iniciativas

## Funcionalidades del mapa de iniciativas

* Visualizar puntos en un mapa, correspondientes a la localización de iniciativas ciudadanas
* Filtrado de datos según Ciudad, Temática, Tipo de Espacio y Tipo de Agente impulsor de las iniciativas, mediante menús desplegables
* Consultar información completa de la iniciativa seleccionada
* Compartir los datos de una actividad seleccionada, mediante redes sociales como Facebook o Twitter
* Introducir nuevos datos mediante formulario de Google Docs
* Consultar leyenda del mapa

## Descripción de los documentos del mapa de Alcalá con iniciativas

### ./index.html
Documento HTML con los menús, canvás del mapa y desplegables con información

### ./favicon.png
Archivo de imagen en formato PNG correspondiente al icono a representar en el navegador

### ./css/style.css
Documento CSS con estilos a utilizar en la web y mapa

### ./js/script.js
Documento JavaScript para tomar datos de la base de datos y organizarlos para su visualización

### Dependencias

* [CartoDB.js:](http://docs.cartodb.com/cartodb-platform/cartodb-js.html) Librería JavaScript para interactuar con el servicio de datos CartoDB. Se trata de una librería descendiente de Leaflet
* [Overlapping Marker Spiderfier  for Leaflet:](https://github.com/jawj/OverlappingMarkerSpiderfier-Leaflet) Librería JavaScript
Copyright (c) 2011 - 2012 George MacKerron. El código se encuentra incluido en ./iniciativas/js/script.js
Released under the [MIT licence](http://opensource.org/licenses/mit-license)
* [Font Awesome 4.7.0:](http://fortawesome.github.io/Font-Awesome/) Biblioteca de iconos abierta
* [Moment.js](http://momentjs.com/) Librería JavaScript para parsear, validar, manipular y representar datos en forma de fecha.
* [Google Fonts API](https://developers.google.com/fonts/) Servicio para añadir fuentes de texto

# Formulario de entrada de nuevas iniciativas

El formulario de entrada de nuevas iniciativas se ha realizado en Google Docs y, por tanto, es ajeno a esta Web.

### Dependencias

* [JQUERY v1.72](http://jquery.com/)
Biblioteca JavaScript para la simplificación de código
* [jquery-latitude-longitude-picker-gmaps](https://github.com/wimagguc/jquery-latitude-longitude-picker-gmaps)
Biblioteca JavaScript  construida sobre JQuery para la ventana de mapa de geocodificación (obtención de coordenadas geográficas a partir de direcciones postales mediante la API de Google)


---
# Acerca de los datos

## Fuente de los datos

Los datos corresponden a la información facilitada por las iniciativas

## Acceso a los datos.

Puedes consultar, descargar o utilizar el API que los proporciona desde el servicio de www.cartodb.com:

* [Tabla de las iniciativas recopiladas](https://alcalaconiniciativas.carto.com/tables/iniciativas_aci_02_2017_n2/public)

## Descripción de los datos

Para una descripción detallada de las tablas de datos y de sus atributos consulta el documento [DatasetDescription.md](https://github.com/perezdans/Alcala-con-iniciativas/blob/master/DatasetDescription.md)

Se distribuyen en una tabla:

* **iniciativas:** Tabla de datos correspondientes a las iniciativas ciudadanas. Una iniciativa es una entidad ciudadana que realiza actividades.

---
#Desarrollo
@perezdans

El código de Alcalá con iniciativas está basado en el código de CIVICS
https://github.com/CIVICS-VIC/civics-alpha-v3 (CIVICS)



---
# Licencias

![CC](https://i.creativecommons.org/l/by-sa/4.0/88x31.png "Imagen del Logo de Creative Commons")

Esta obra está bajo una [Licencia Creative Commons Atribución-CompartirIgual 4.0 Internacional](http://creativecommons.org/licenses/by-sa/4.0/)

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
* Introducir nuevos datos mediante formulario
* Consultar leyenda del mapa

## Descripción de los documentos del mapa de iniciativas

Los documentos correspondientes se encuentran en la carpeta **./iniciativas/**

### ./iniciativas/index.html
Documento HTML con los menús, canvás del mapa y desplegables con información

### ./iniciativas/favicon.png
Archivo de imagen en formato PNG correspondiente al icono a representar en el navegador

### ./css/mapa_general.css
Documento CSS con estilos comunes en los dos mapas

### ./iniciativas/css/mapa_ini.css
Documento CSS con estilos del mapa de iniciativas

### ./iniciativas/js/script.js
Documento JavaScript para tomar datos de la base de datos y organizarlos para su visualización

### Dependencias

* [CartoDB.js:](http://docs.cartodb.com/cartodb-platform/cartodb-js.html) Librería JavaScript para interactuar con el servicio de datos CartoDB. Se trata de una librería descendiente de Leaflet
* [Overlapping Marker Spiderfier  for Leaflet:](https://github.com/jawj/OverlappingMarkerSpiderfier-Leaflet) Librería JavaScript
Copyright (c) 2011 - 2012 George MacKerron. El código se encuentra incluido en ./iniciativas/js/script.js
Released under the [MIT licence](http://opensource.org/licenses/mit-license)
* [Font Awesome 4.4.0:](http://fortawesome.github.io/Font-Awesome/) Biblioteca de iconos abierta
* [Moment.js](http://momentjs.com/) Librería JavaScript para parsear, validar, manipular y representar datos en forma de fecha.
* [Google Fonts API](https://developers.google.com/fonts/) Servicio para añadir fuentes de texto

# Formulario de entrada de nuevas iniciativas

## Descripción de los documentos del formulario de entrada de nueva iniciativa

### ./iniciativas/formulario/index.php
Documento con el formulario de entrada de nuevas iniciativas. Mediante scipt en JavaScript, los datos previos se ajustan a la ciudad que se visualiza en el mapa desde el que se ha convocado al formulario añadiendo a la URL: ?city=NombreCiudad. En esta versión alpha v3, se encuentran disponibles dos valores para Nombreciudad: Madrid y MexicoDF

### ./iniciativas/formulario/css/form_styles.css
Documento CSS con estilos de visualización del formulario

### ./iniciativas/formulario/functions.php
Documento PHP que se conecta a la base de datos para mostrar en el formulario valores existentes, correspondientes a la ciudad desde donde se ha llamado al formulario

### ./iniciativas/formulario/processFormData.php
Documento PHP que toma los datos introducidos en el formulario por el usuario y crea entradas nuevas en la base datos

### ./actividades/formulario/cartodb.class.php
Script para manipular información obtenida de la base de datos alojada en la cuenta del servicio www.cartodb.com asociada al proyecto

### ./actividades/formulario/oauth.php
Script para la conexión a la base de datos mediante servicio de oauth

### ./actividades/formulario/cartodb.config.php
Documento PHP con las credenciales para obtener permiso para editar la base de datos de la cuenta del servicio www.cartodb.com asociada al proyecto

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

* [Tabla de las iniciativas recopiladas](https://mappemad.cartodb.com/tables/iniciativas/public)
* [Tabla de las actividades recopiladas](https://mappemad.cartodb.com/tables/actividades/public)

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

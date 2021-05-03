# Web scraping: Properati.com

En el presente repositorio se realiza la extracción de la información de la página [properati.com](https://www.properati.com.ec/), l cual presenta información relevante sobre la oferta de viviendas en Ecuador. El objeto de estudio del presente proyecto es el análisis descriptivo de los anuncios de ventas de casas en el Distrito Metropolitano de Quito - Ecuador.

El sitio web elegido, actualmente consta de las variables necesarias para poder realizar el análisis anteriormente descrito y cumplir con los objetivos propuestos.

Actualmente la página web [properati.com](https://www.properati.com.ec/) es una de las más conocidas y demandadas del país, se encarga de publicar anuncios sobre compra venta y alquiler de varios inmuebles a nivel nacional y actualmente esta página o empresa ofrece una aplicación móvil que facilita la navegación y día a día sigue creciendo el número de personas que accede a ella, para publicar sus bienes inmuebles que pretenden vender.

### Descripción del conjunto de datos

El conjunto de datos contiene la información capturada desde el sitio web:  [properati.com](https://www.properati.com.ec/). El Dataset contiene la información más relevante de los anuncios de ventas de bienes inmuebles para el Distrito Metropolitano de Quito en Ecuador. El principal objetivo del Dataset es responder preguntas acerca del precio de los inmuebles según el área, número de habitaciones, ubicación, etc.

Unos de los inconvenientes del dataset puede ser que presenta los anuncios de solo una página web, para análisis más relevantes se debería utilizar información obtenida desde diferentes sitios web de anuncios de ventas de bienes inmuebles. otro incoveniente es que el dataset no presenta importación más desagregada de los anuncios como por ejemplo el número de baños, si cuenta o no con patio, si está ubicado dentro de un conjunto residencial y si el inmueble  cuenta con servicios básicos.

Se debería realizar un tratamiento de la información antes de realizar el análisis. por ejemplo se deberia realizar la eliminación de caracteres especiales del campo descripción, eliminación del signo de dólar ($) del campo precio, eliminación del símbolo de metros cuadrados del campo área.


### Capturas de la página web properati.com

![alt text](https://github.com/difercast/web_scraping/blob/master/images/properati.png?raw=true "Anuncio Properati")

![alt text](https://github.com/difercast/web_scraping/blob/master/images/estadisticas.png?raw=true "Estadísticas de los anuncios")

### Descripción de los campos extraídos

Los campos contenidos en el dataset son:
- __Descripción:__ Descripción del anuncio detallando las características del inmueble por parte del venderor.
- __Precio:__ Valor en Dólares del Inmueble.
- __Tipo:__ Variables que describe si inmueble es casa o departamento.
- __Ubicación:__ Dirección del Inmueble.
- __Fecha de publicación:__ Fecha en la que se publicó el anuncio de venta del inmueble.
- __Área:__ Área (en metros cuadrados) del inmueble.
- __Núm. habitaciones:__ Número de habiataciones con las que cuenta el inmueble.

La recolección de la información se realizó el día 06.04.2018. Estos datos se recogieron mediante técnicas de Web scraping utilizando la librería BeautifulSoup sobre el entorno Jupiter.
Por motivo de no saturar la página web de peticiones únicamente se capturo el resultado de las primeras 20 páginas de anuncios.

Algunas rutas importantes en el repositorio:

El código utilizado para la realización de la práctica se encuentra en la sifuiente ruta del repositorio:

`web_scraping/src/scraper.py`


El conjunto de datos resultante del ejercicio realizado se encuentra en la ruta indicada a continuación:

`web_scraping/data/casas.csv`

El separador del conjunto de datos es `|`

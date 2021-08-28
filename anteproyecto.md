# Visiones de la Investigación 202110, Maestría en Humanidades Digitales, Universidad de los Andes
# Anteproyecto de trabajo de grado

## Felipe Salas Noguera, código 201413117

## Fecha: Mayo 26 de 2021

## Título
**Algoritmos de recomendación de música: filtro burbuja, sesgos y la estética del algoritmo curador**

## Palabras clave
* Algoritmos de recomendación; Plataformas de Streaming (Apple Music, Spotify, Youtube Music); AI; Sesgos de los Algoritmos; Música Emergente; Filtro Burbuja

## Abstract

Con la aparición de las plataformas de streaming de música, el funcionamiento de la industria musical y el consumo de música ha cambiado radicalmente. El descubrimiento de nueva música ha pasado de ser influenciada por emisoras de radio, o por escuchar nuevos proyectos en tiendas de discos, a ser dictadas, en su mayoría, por algoritmos de recomendación (algoritmos BART) que hacen parte de las plataformas de streaming. Con esto, los algoritmos se convirtieron en los curadores personales de música para los usuarios. La experiencia que cada oyente tiene en las plataformas de streaming está mediada por un algoritmo que decide que música poner en aleatorio, o que canciones mostrar en las listas de reproducción para descubrir nueva música.  

En consecuencia, los algoritmos disminuyen la diversidad de consumo de música, y tienen sesgos que afectan a proyectos musicales que no aportan al afán de lucro de las plataformas de streaming. Este proyecto, se va a basar en dos partes, en la primera, se investigará sobre la estética de los algoritmos, los sesgos y el fitro burbuja; en la segunda, se va a desarrollar una plataforma donde usuarios de Spotify van a poder recibir recomendaciones de proyectos musicales bogotanos que, probablemente, el algoritmo no les va a recomendar en otras situaciones. Con esto, busco comprobar si es posible que, usando el mismo algoritmo de Spotify y su API, se logre bajar los sesgos y aumentar la diversidad de consumo de música en esta plataforma de streaming.  

With the rise of music streaming platforms, the music industry and music consumption has changed radically. The discovery of new music has gone from being influenced by radio stations, or by listening to new projects in record stores, to being dictated, for the most part, by recommendation algorithms (BART algorithms) that are part of the streaming platforms. With this, algorithms became the personal music curators for users. The experience each listener has on streaming platforms is mediated by an algorithm that decides what music to shuffle, or what songs to show in playlists to discover new music.  

Consequently, algorithms decrease the diversity of music consumption, and have biases that affect music projects that do not contribute to the profit motive of streaming platforms.This project will be based on two parts, in the first, we will investigate the aesthetics of algorithms, biases and the bubble filter; in the second, I will develop a platform where Spotify users will be able to receive recommendations of Bogota music projects that, probably, the algorithm will not recommend in other situations.  With this, I seek to test whether it is possible, using the same Spotify algorithm and its API, to lower the biases and increase the diversity of music consumption in this streaming platform.  



## Objetivo general

Investigar sobre la estética de los algoritmos, sus sesgos, el filtro burbuja, y cómo son los mediadores de a experiencia en las plataformas de streaming. Con la finalidad de identificar cómo estos aspectos de los algoritmos afectan el descubrimiento de proyectos musicales emergentes que no aportan al afán de lucro de las plataformas de streaming.


### Objetivos Específicos

1. Investigar los aspectos estéticos de los algoritmos y ver cómo estos hacen parte de la experiencia musical en el siglo XXI
2. Crear una aplicación que intenta contrarrestar el filtro burbuja usando el API de Spotify
3. Estudiar cómo el algoritmo de Sppotify afecta a la escena musical emergenten de Bogotá


## Lista de productos esperados 

1. * Reflexión sobre la estética de los algoritmos de los resultados de la plataforma
2. * Aplicación web que permite a los usuarios agregar nueva música a sus cuentas de las plataformas de streaming

## Problema

Los algoritmos de recomendación, desde su concepción, están sesgados y siguen un modelo capitalista de busqueda de lucro. Esto ha provocado que baje la diversidad de contenido consumido en las plataformas de streaming. En consecuencia, los nuevos proyectos musicales tienen dificultad para ser descubiertos y que sean escuchados por más usuarios. 

¿Existe la posibilidad de crear una herramienta que ayude a contrarrestar el filtro burbuja y la baja diversidad de consumo en Spotify?


## Hipótesis de trabajo

Los algoritmos de recomendación tienen sesgos, disminuyen la diversidad de consumo y afectan el consumo de música que no aporta a su afán de lucro. Sin embargo, usando el API de Spotify se puede cambiar el comportamiento del algoritmo y contrarestar sus efectos negativos en el consumo de música.

## Fuentes

- Base de datos de músicos Bogotanos, tengo acceso a la de La Cara de Emer, legalmente puedo usar los datos. puedo solicitar el de el IDRD por medio de un derecho de petición. y hacer una convocatoria (revisar si tengo que hacer algo con el cómite de ética)

**APIs**

Un posible inconveniente con el uso de las APIs es que estas pueden cambiar la cantidad y los datos que se pueden obtener de la plataforma. Por ahora, su uso es gratuito y permiten crear una cuenta de desarrollador para hacer uso de la herramienta. Sin embargo, se debe tener en cuenta los términos y condiciones del uso de las APIs y revisar que el proyecto sigue respetando el uso de las plataformas.

* Apple. Apple Music API | Apple Developer Documentation. https://developer.apple.com/documentation/applemusicapi/. Consultado el 9 de febrero de 2021.

* Google. “Youtube API”. Google Developers API, https://developers.google.com/youtube/v3.

* Spotify. Web API | Spotify for Developers. https://developer.spotify.com/documentation/web-api/. Consultado el 9 de febrero de 2021.


## Metodología

Este proyecto se divide en dos partes, una teórica y una práctica. Para la primera parte, estudiaré los aspectos estéticos y los sesgos del algoritmo de recomendación de música de Spotify. Esta sección será la base para la creación de la plataforma, se basa en la hipótesis que es imposible que los algoritmos de recomendación no estén sesgados y contribuyan a filtro burbuja, más que todo cuándo están al servicio de la búsqueda de lucro. 
  
Para el desarrollo de la segunda parte, se usará un servidor web, el frontend va a ser en HTML y CSS y el back end, para ser compatible con los APIs de las plataformas de streaming, va a hacerse en JSON basándose en REST y en JS (estoy considerando Python). Para poder desplegar los primeros prototipos de la plataforma usaré la capa gratuita de Amazon AWS, la cual me permitirá, por un año, tener acceso a un servidor web en la nube para hacer las pruebas y prototipos.   
   
La plataforma consiste en recomendar nuevos proyectos musicales a los usuarios. Para hacer esto, se va a tener en cuenta su librería de música, las recomendaciones que da el algoritmo de las plataformas y la base datos propia de proyectos musicales. El producto final es una playlist creada a la medida de cada usuario.   
   
Es importante tener en cuenta que las APIs pueden limitar el número de datos entregados por cada consulta, esto puede ser un problema al consultar la librería musical de los usuarios. Por lo anterior, es necesario recopilar información de proyectos musicales bogotanos de fuentes externas (fuentes propias, colectivos musicales de la ciudad como La Cara de Emer, El Enemigo, EMV –una rama del IDRD–, y bases de datos distritales de músicos), para después categorizarlas y hacer recomendaciones en grupos más pequeños. 


- Usar Knime y tensor flow para el manejo de datos



## Bibliografía anotada

El enlace de la bibliografía es este: https://www.zotero.org/groups/2803661/bibliografavisiones/library

## Preguntas Diseño de Proyecto

### Análisis

#### Qué preguntas le voy a hacer a las fuentes ?

Para de desarrollo de mi proyecto voy a hacer dos bloques de preguntas. El primero está relacionado con el funcionamiento del algoritmo y cómo este afecta el consumo de música. Y el segundo, sobre la estética del algoritmo y cómo el algoritmo entiende los objetos estéticos.

Para el primer bloque tengo pensadas estas preguntas:

1. ¿Qué efectos tiene el algoritmo de recomendación de música en el descubrimiento de música? 
2. ¿cuáles son los parámetros que el algoritmo tiene en cuenta para recomendar o no recomendar la música?
3. ¿Se han detectado consecuencias negativas en que el consumo de música esté mediado por un algoritmo BART?
    3.1 Esto está relacionado con la estética del algoritmo y cómo es la experiencia del usuario y del algoritmo
4. ¿Cómo cambia la experiencia del usuario con la curaduría algorítmica y con la curaduría humana?
5. ¿Entienden las empresas de Streaming al algoritmo de recomendación?
5. ¿Es el algoritmo de recomendación considerado un algoritmo curador por sus creadores?

Para el segundo bloque tengo pensadas estas preguntas:

1. ¿Cómo entiende el algoritmo los objetos estéticos?
2. ¿Puede el algoritmo entender lo bello? 
3. ¿Qué papel tiene el animo de lucro en la curaduría de objetos estéticos?
4. ¿Cuál es la estética del algoritmo?
    4.1 ¿Cómo es la experiencia estética del algoritmo?
    4.2 ¿Cómo el algoritmo nos permite relacionarnos con la música? - Visto desde la estética
    
#### Pueden estas preguntas ser formuladas por un computador ?

Si bien para la mayoría de las preguntas puede ser útil tener datos que pueden ser recopilados por un computador, es necesario un análisis posterior por un investigador que permita interpretar los datos. 

#### Qué metodología, tecnología o modelo me permite formular esta pregunta computacionalmente ?

En la mayoría de papers que tratan estas preguntas usan calculo y matemáticas para análizar los datos que da el algoritmo a los creadores de la plataforma. Sin embargo, usando el API de Spotify y big data se podrían obtener datos que ayuden a responder estas preguntas.

### Problema

#### Cómo es el contexto del que surge el problema ?

Con la aparición de las plataformas de streaming de música, el funcionamiento de la industria musical y el consumo de música ha cambiado radicalmente. El descubrimiento de nueva música ha pasado de ser influenciada por emisoras de radio, o por escuchar nuevos proyectos en tiendas de discos, a ser dictadas, en su mayoría, por algoritmos de recomendación (algoritmos BART) que hacen parte de las plataformas de streaming. Con esto, los algoritmos se convirtieron en los curadores personales de música para los usuarios. La experiencia que cada oyente tiene en las plataformas de streaming está mediada por un algoritmo que decide que música poner en aleatorio, o que canciones mostrar en las listas de reproducción para descubrir nueva música.  

#### Tengo contacto directo con el contexto/comunidad ?

Si y no, si bien tengo una cuenta en varias plataformas de streaming y puedo usar el API de estas para obtener datos de cómo funciona el algoritmo, las empresas siguen siendo hermeticas en cuanto al funcionamiento (también que la mayoría no saben en su totalidad cómo funciona su algortimo de recomendación) y muchos de los datos solamente los divulgan en papers y conferencias.


#### Si tengo contacto directo.  Qué instrumentos me permiten recopilar la información que necesito para tomar decisiones y formular una solución ?

El API de las plataformas


##### Si no tengo contacto directo.  Qué fuentes preexistentes de información puedo usar para tomar decisiones ? (otros casos similares, contextos similares, etc)

Los papers de las empresas de streaming y libros que han estudiado los efectos de los algoritmos en otros contextos, que apesar de estar diseñados para otros medios, su funcionamiento es similar. Por lo tanto, las consecuencias pueden ser similares o las mismas. 

## Comentarios de mis compañeras y de Nicolás

> Pensar en la divuglación con personas de la Escena. mirar con la Cara de Emer!! 
> Si voy a alcanzar a salir de eso

> - Salir del filtro burbuja 
> - En que medida se puede salir 
> - comparar papers sobre los datos de los algoritmos. 
> - Echarle cabeza si quiero llegar a la plataforma o desde lo investigativo


## Comentarios presentación

> Añadir lo que quiero hacer, mis objetivos
> Añadir que es lo que busco 
> Aclarar si voy a poder responder las dos preguntas, quizá la segunda solamente por encima
> Añadir una diapositiva con la hipotesis y poner fuentes 
> No tiene que ser tan rigido, puedo añadir más partes

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
3. * Mapa interactivo sobre el funcionamiento del algoritmo

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

## Referentes

* https://forgotify.com


## Metodología

Este proyecto se divide en dos partes, una teórica y una práctica. Para la primera parte, estudiaré los aspectos estéticos y los sesgos del algoritmo de recomendación de música de Spotify. Esta sección será la base para la creación de la plataforma, se basa en la hipótesis que es imposible que los algoritmos de recomendación no estén sesgados y contribuyan a filtro burbuja, más que todo cuándo están al servicio de la búsqueda de lucro. 
  
Para el desarrollo de la segunda parte, se usará un servidor web, el frontend va a ser en HTML y CSS y el back end, para ser compatible con los APIs de las plataformas de streaming, va a hacerse en JSON basándose en REST y en JS (estoy considerando Python). Para poder desplegar los primeros prototipos de la plataforma usaré la capa gratuita de Amazon AWS, la cual me permitirá, por un año, tener acceso a un servidor web en la nube para hacer las pruebas y prototipos.   
   
La plataforma consiste en recomendar nuevos proyectos musicales a los usuarios. Para hacer esto, se va a tener en cuenta su librería de música, las recomendaciones que da el algoritmo de las plataformas y la base datos propia de proyectos musicales. El producto final es una playlist creada a la medida de cada usuario.   
   
Es importante tener en cuenta que las APIs pueden limitar el número de datos entregados por cada consulta, esto puede ser un problema al consultar la librería musical de los usuarios. Por lo anterior, es necesario recopilar información de proyectos musicales bogotanos de fuentes externas (fuentes propias, colectivos musicales de la ciudad como La Cara de Emer, El Enemigo, EMV –una rama del IDRD–, y bases de datos distritales de músicos), para después categorizarlas y hacer recomendaciones en grupos más pequeños. 


- Usar Knime y tensor flow para el manejo de datos



## Bibliografía anotada

El enlace de la bibliografía es este: https://www.zotero.org/groups/2803661/bibliografavisiones/library

## Link al Mapa Interactivo 

https://miro.com/app/board/o9J_ltwhxZE=/?invite_link_id=690582374007

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

### Formulación de la Solución

#### El problema puede resolverse con el uso de una herramienta por los agentes del contexto ?

El problema puede solucionarse modificando el algoritmo para lograr contrarrestar sus efectos negativos.

#### La herramienta puede usarse en otros contextos similares o para resolver problemas similares ?

Sí, si se logra modificar o crear *contra algoritmos* estos pueden ser usados en cualquier otro contexto que use algoritmos de recomendación BART y de curaduría algorítmica.

#### Cómo puedo asegurar la adopción de la herramienta y promover su uso ?

La única forma es que este *contra algoritmo* ayude al afán de lucro de las plataformas o mejore de forma significativa la experiencia de los usuarios en las plataformas.

### Evaluar la Solución

#### Qué instrumentos puedo usar para evaluar el resultado del uso de la herramienta ?

1. Datos y analíticas que se puedan recopilar de los usuarios de este *contra algoritmo* 
2. Uso de Knime o herramientas de big data para lograr encontrar si la herramienta útil o si tiene efectos en el descubrimiento y adopción de nueva música


#### Cómo puedo incorporar los resultados de esta evaluación para refinar la solución en iteraciones posteriores ?

Crear varias versiones del *contra algoritmo* y hacer pruebas A/B para ver cuál funciona mejor.

#### Hasta dónde puedo realizar iteraciones en el contexto de este proyecto, o etapa del proyecto ?

Creo que apenas esté la herramienta puedo realizar iteraciones hasta la etapa de análisis de los datos, donde es necesarioo dejar de recopilar datos para dedicarse al análisis. 

<<<<<<< Updated upstream:README.md
# Estética del algoritmo

## El algoritmo espia 

## El algoritmo cómo un conjunto de tecnologías

## El algoritmo Gatekeeper

## Burbuja Estética 

* Esto es un paralelo a las burbujas epistémicas

* El algoritmo es un espejo, nos muestra los gustos que nosotros ya le mostramos. Cada vez el algoritmo es menos arriesgado a mostrarnos algo nuevo para evitar un experiencia no agradable en la plataforma (Anderson et al.)

* Buscar si tiene funcionamientos similaes con las burbujas epistémicas 


## El Algorítmo Curador 

### Funciones de un Curador

Dever Restrepo, Paula, y Amparo Carrizosa. Manual básico de montaje museográﬁco. División de museografía Museo Nacional de Colombia, abril de 2021, p. 41.


1. Distribuir las obras en el espacio
2. Crear el concepto de una exposición  
* Definir el carácter de una exposición
3. Crear una puesta en escena a partir de una colección de objetos
4. Escribir un guión para las exposiciones

### Funciones del algoritmo de Spotify

1. Definir que elementos (canciones) y subcolecciones de elementos (Playlist) le muestra a los usuarios
2. Crea una experiencia *única* para cada usuario en la plataforma
* Recomienda que música escuchar según los gustos personales y el perfil al que se está asignado
3. Crea narrativas sobre que música se debería escuchar según el estado de ánimo, género o situación
4. Se adapta para crear una mejor experiencia para el usuario
* Su objetivo principal es que el usuario siga usando la plataforma

### Ideas

* HARD - CORE. Un grupo de artistas que desarrolla metodos de curaduría algorítmica.
[Ejemplos de Algoritmos Curadores](http://the-hard-core.eu/?page_id=13918)

* Mackenzie, Adrian. “From API to AI: Platforms and Their Opacities”. Information, Communication & Society, vol. 22, núm. 13, noviembre de 2019, pp. 1989–2006. DOI.org (Crossref), https://doi.org/10.1080/1369118X.2018.1476569.

> Los *Algoritmos de las redes sociales* crean formas opacas de propiedad y capitalización de los objetos.

* La curaduría algorítmica no tiene nada negativo por si sola
* Los algoritmos siempre están sesgados, debido a que su creador está sesgado (Kitchin)

* Kowalski, Michael J. “The Curatorial Muse”. Contemporary Aesthetics, vol. 8, 2010, http://hdl.handle.net/2027/spo.7523862.0008.017.

> As if the praxis-theory dialectic weren't enough of a challenge for curators in their role as educators, the very nature of the theories to be embodied in shows is actually much more unstable than a typical glossy catalogue essay would have one believe. There is a clear difference between the difficulty of demonstrating the value of a previously established canon, on the one hand, and the difficulty of making a case for the museum quality of new works, on the other, to say nothing of making a case for new ideas about the very nature of the project of art.  The nature of the power wielded by a curator in a given show and, hence, the complexion of that curator's educational function, varies with the type of theory being imparted.  I shall return to the paradoxical nature of well-intentioned teaching later in this essay. (p. 3)

> The modern curator, whether of a custodial or activist bent, is typically an expert in many fields: history, conservation, administration, and the production of shows, to cite but the obvious.

* Entra el algoritmo de Spotify en esta definición de *curador moderno*: ¿si es experto en muchos campos?
* ¿Cómo puede el algoritmo de Spotify curar objetos estéticos si solamente los entiende como datos?

> Curators create physical manifestations of analytic theories formulated primarily by critics. 

* ¿Cuál es la crítica que hace el algoritmo de recomendación a las canciones? 
~~* ¿Puede considerarse el algoritmo un elemento del algoritmo? ¿Es Spotify en su totalidad el curador y por lo tanto el algoritmo es la parte *computacional* de este curado humano-algoritmo? ~~
* El algoritmo tiene una relación *capitalista* con los objetos estéticos, su crítica está inclinada hacía si es popular y/o comercial.




## Prototipo

* Usar Rapsberry Pi



#### Por seguir investigando

* La estética del curador humano y de la curaduría.
* Leer de estética, Kant, Reynolds, Hegel




## Comentarios Avances 4 de septiembre

* Me sirve más el cáracter narrativo de la curaduría mas que la parte museográfica
* Las AI normalmente se entiende como problemas cuantitativos
* Definir bien mi hipótesis
* Establecer la definición de curadoría que voy a usar

¡Cómo el algoritmo de Spotify es Curador!
* El algooritmo crea un curador a partir de mi críterio, un espejo de los gustos del usuario 
* La experiencia estética del algoritmo es una copia de la experiencia estética que yo he buscado dentro de la plataforma 
* Un algoritmo anti curaduría, o un nuevo tipo de curaduría
* Mi pryecto puede ser un artefacto retórico, un objeto crítico que no tiene que ser 100% funcional

[https://dhdebates.gc.cuny.edu/projects/making-things-and-drawing-boundaries](https://dhdebates.gc.cuny.edu/projects/making-things-and-drawing-boundaries)


## Tutoría 11 de Septiembre

* ¿Cuál es el prótotipo para mi parte teórica, ¿Es La hipótesis?
* ¿Puede ser comparable el rol de un gatekeeper con el de un curador?
* ¿Son estas labores iguales o son complementarias?
* Dentro de Spotify se usa el término Curaduría Algorítmica. Algo-Torial por Bonini (2019)
* Puede haber una relación entre los Gatekeepers y los curadores, Bonini pone po ejemplo a los programadores de radio cómo

## Comentarios de Paez

* Los curadores dan juicio de valor, no son solo juicios de gusto 
* El algoritmo no es tan complejo y robusto como para decirle al algoritmo que es un curador
* Pensar los bueno y lo malo de tener esta curaduría, filtro burbuja, cámaras de eco. Permite enriquecerla pero no deja salirse de ella 
* Instrumental, intermediario entre mi gusto y mi gusto
* el conocimiento que el algoritmo tiene sobre mi música es sobre mi gusto. y el interés comercial 
* Parte de mi análisis es que el algoritmo no es 100% curador
* El papel del curador en moldear los gustos. El taste maker
* La influencia de las personas en la cultura pop para moldear los gustos. un DJ o una emisora
* Paralelo con las burbujas epistémicas
* EL CONCEPTO CLAVE ES LA BRUBUJA ESTÉTICA, en el GUSTO
* El gusto desde la sociología y no desde la filosofía
* Mirar literatura en Psicología sobre los gustos
* Literatura sobre cómo los sesgos afectan el gusto en el arte

## Comentarios Camilo 11 de Septiembre

* Este gatekeeping está relacionado con los agentes involucrados en la plataforma de música
* Curaduria es mostrar unas cosas y ocultar otras
* Al escuchar lo más popular lo vuelve más popular y cierra el universo 
* Comparar el encontrar nueva música con el resultado de busqueda de Google
* El Gatekeeping es una consecuencia intensional para cumplir con los intereses de Spotify
* Spotify tiene todo el control de la plataforma, pero al final que el usuario tenga un buena experiencia los beneficia a ellos también 
* El comportamiento del algoritmo es un territorio de disputa entre los intereses de los usuarios y los de Spotify
* Puedo hacer una playlist o algo así para usalo cómo ejemplo
* Hacer una colección de conceptos 

## Comentarios Camilo 25 de Septiembre

* Próxima tutoria ver que extrategía sirve 

## Comentarios tutoria 23 de octubre

* Dar un juicio de valor al algoritmo es humanizarlo 
* El algoritmo si sigue unos intereses de sus creadores
* Crear un mapa de los intereses en los que está el algoritmo 
* El algoritmo si puede pivilegiar cosas e intereses, pero toca entender bajo que condiciones funciona
* Que el algoritmo funcione como otros intereses 
* Hacer encuestas y preguntas más especificas, preguntar si les gustó la experiencia, comparar una plyalist creada automaticamente y una por mi app
* Que mi app le de play y con esa canción cree la playlist 
* No tengo que comprobrar todo, con ka experimentación puedo apoyar mi argumento
* esto puede servir para caracterizar el algoritmo, cuidado no humanizarlo
* Usar las eval

## Comentarios Camilo 

> El algoritmo curador, extender sobre esto. Cuál punto de vista de la curaduría me afirma que el algoritmo es curador! . puedo apropiar un concepto de una práctica y extrapolarlo a otro contexto/práctica
> Quienes son los agentes de esta experiencia estética. 
> Cómo decribir esta experiencia estética. Qué características son importantes para mi investigación. Tengo que describir esta experiencia, compararla con una experiencia en un museo.
> Cómo puedo evaluar esta experiencia, ética, moral o pueden ser evaluados númericamente. Es cualitativa o Cuantitativa? Es el tiempo de las canciones. Definir que quiero como experiencia estética.
> Elaborar sobre los términos de Algoritmo Curador y Experiencia Estética del algoritmo.



=======
## Comentarios Camilo 

El algoritmo curador, extender sobre esto. Cuál punto de vista de la curaduría me afirma que el algoritmo es curador! . puedo apropiar un concepto de una práctica y extrapolarlo a otro contexto/práctica
>>>>>>> Stashed changes:anteproyecto.md

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

## Tutoria 20 de Noviembre 

> Marco teorico 
Estado del arte
Marco teorico
Mirar la Tesis de Hugo Idarraga
Mirar la tesis de Santiago Arteaga
La presentación del colocio es rápida, sacar los conceptos más importantes, navegar el mapa como presentación


## Comentarios 22 nov Andrés Paéz 

* Las cajas de resonacia son activas en cuanto le muestro lo que no me gusta

* Las burbujas estéticas son individuales, no excluyen individuos 

* Las personas no se enteran que hay intereses comerciales

* El curador no me está vendiendo cosas 

* Burbuja Estética en cuanto a que afecta los sentidos

* Su justo está siendo moldeado 

* Volver a estudiar esto del taste making 

* Burbuja pasiva a que no me expone a nuevos generos 

* La manipulación es por el aumento la popularidad y la cantidad de playlist 

* Hacer mini ensayos, uno de la parta comercial, uno de la técnica y uno de la teorica 

## Comentarios Coloquio 1 Diciembre 

### Comentarios María José

* Trabajar más en los sesgos de los algoritmos 

* El algoritmo no tiene agencia, los sesgos son de los creadores

* Que significa una experiencia buena para los usuarios de Spotify 

* Que sería una experienca no hegemónica 

* Definir la experience Hegemónica 

### Comentarios Camilo 

* La agencia como influencia, pero también como lo que dejan de hacer. Entender cómo está distribuido el poder.

### Sistemas de recomendación colaborativos 

* leer más sobre que Sistema de recomendación tiene Spotify, si User based or Item based. Con esto en mente, tengo que tener en cuenta que si es Item-based Spotify no toma en cuenta la información de otros usuarios (Las recomendaciones están en una burbuja estética), si es User-based toma en cuenta usuarios similares para recomendar nuevas cosas a los usaurios. Por ahora yo he asumido que el algoritmo es User-Based, quizá Spotify es Item-Based y User based según la información que tenga del usuario. 
* Impacto del Long Tail, p.39 de Aggarwal. As discussed in section 2.2, the distribution of ratings typically shows a long-tail distribution in many real scenarios. Some movies may be very popular and they may repeatedly occur as commonly rated items by diﬀerent users. Such ratings can sometimes worsen the quality of the recommendations because they tend to be less discriminative across different users..
* Leer bien el subtítutlo 2.3.4 sobre los beneficios del user y del item sobre diversidad.
* En Spotify la cantidad de Items y de Usuarios aumenta siempre, quizá si utilizan un sistema de recomendación user e Item based al mismo tiempo 
* Sparsity, pensar como puede afectar las burbujas estéticas
* Leer sobre los Clusters methods, esto podría explicar como son los sesgos del algoritmo.

### Performance
* Schechner tambien dice que todo performance es una acción entrenada y ensayada. los sujetos deben aprender patrones culturales de comportamiento y los roles que debe desempeñar en determinadas circustancias sociales.
* El algoritmo hace parte de este performance de la escucha de la música en las plataformas, es un objeto más de este performance, sin embargo este puede que no cumpla todas las expectativas culturales. Acá se puede relacionar con el paper de como funciona el algoritmo en america latina
* Revisar conducta restauradda (restored behavior) de Schechner (p34-35) Schenker, Heinric. 2002. The Art of Performance. Oxford: Oxford University Press.

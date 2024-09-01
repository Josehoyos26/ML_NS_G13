![Portada](../Semana%202/figs/ans_banner_1920x200.png)

# Mejor servicio de streaming en relación calidad/precio

## Resumen:
El mercado de servicios de streaming ha crecido significativamente, ofreciendo muchas opciones para el entretenimiento digital. Sin embargo, esta variedad presenta el desafío de determinar cuál servicio ofrece la mejor relación calidad-precio. Este análisis busca resolver este reto, proporcionando una evaluación clara y accesible para una audiencia general.

El objetivo es comparar los principales servicios de streaming, evaluando factores como el costo de suscripción, la calidad del contenido y la variedad de títulos. Se recopilarán datos de reseñas de usuarios, puntuaciones y popularidad de las peliculas de IMDB.

El resultado esperado es una guía que ayude a los consumidores a tomar decisiones informadas sobre qué servicio de streaming se adapta mejor a sus necesidades y presupuesto. Este análisis también ofrecerá información valiosa a los proveedores de servicios de streaming, destacando áreas de mejora y oportunidades en el mercado.

En resumen, este análisis pretende ser una herramienta útil para maximizar el valor de la inversión en servicios de streaming, ofreciendo una evaluación equilibrada de las opciones disponibles.

## Introducción:
El entretenimiento digital es esencial en la vida cotidiana, y los servicios de streaming son una opción popular para consumir contenido audiovisual. Sin embargo, la abundancia de estas plataformas presenta un desafío: determinar cuál ofrece la mejor relación calidad-precio. Este análisis busca resolver esta pregunta, proporcionando una evaluación accesible para una audiencia general.

El cliente potencial incluye a cualquier consumidor de servicios de streaming que desee maximizar el valor de su inversión, desde usuarios individuales hasta familias. Utilizando técnicas de aprendizaje no supervisado, específicamente análisis de clústeres, se agruparán los servicios de streaming según sus características para evaluar su relación calidad-precio.

El objetivo es identificar patrones y tendencias que permitan a los consumidores tomar decisiones informadas sobre qué servicio se adapta mejor a sus necesidades y presupuesto. Además, este análisis ofrecerá información valiosa a los proveedores de servicios de streaming, destacando áreas de mejora y oportunidades en el mercado.

## Revisión preliminar de la literatura:
La literatura existente sobre la evaluación de servicios de streaming se ha centrado en diversos aspectos, como la calidad del contenido, la experiencia del usuario y el costo de suscripción. Estudios nacionales e internacionales han utilizado métodos similares para abordar preguntas relacionadas con la relación calidad-precio de estos servicios.

Por ejemplo, investigaciones previas han empleado análisis de clústeres para agrupar servicios de streaming según características como la resolución de video, la variedad de contenido y la frecuencia de actualización de la biblioteca. Otros estudios han utilizado encuestas de satisfacción del usuario para evaluar la percepción de valor.

Nuestro enfoque se diferencia al combinar tanto métricas objetivas como subjetivas en un análisis integral. Una medida subjetiva podría ser la popularidad de las películas. Mientras que algunos estudios se han centrado exclusivamente en aspectos técnicos o en la percepción del usuario, nuestra propuesta busca integrar ambos enfoques para proporcionar una evaluación más completa y equilibrada.

## Descripción de los datos:
Los datos se obtienen de la base de título de la pagína IMDB y están estructurados de la siguiente manera:

- `title`: Título de la película o serie. Categórica nominal.
- `platform`: Plataforma digital donde se puede encontrar la película (por ejemplo, Netflix, Amazon Prime, etc.). Categórica nominal.
- `type`: Tipo de contenido (IMAGE, SHOW). Categórica nominal.
- `imdbVotes`: Número de votos que la película ha recibido en IMDB. Numérica discreta.
- `imdbScore`: Puntuación media de la película en IMDB. Numérica continua.
- `tmdbPopularity`: Puntuación de popularidad de la película en TMDB. Numérica continua.
- `tmdbScore`: Puntuación media de la película en TMDB. Numérica continua. 
- `runtime`: Duración de la película en minutos. Numérica discreta.
- `genres`: Géneros a los que pertenece la película (puede haber más de uno). Categórica nominal
- `director`: Director de la película. Categórica nominal.
- `year_range`: Rango de años en el que fue lanzada la película. Categórica ordinal.
- `url`: URL de la página de la película en su respectiva plataforma. Categórica nominal

## Propuesta metodológica:
Para abordar la pregunta de interés, se planea utilizar el algoritmo de K-means clustering debido a su simplicidad y eficacia en la identificación de grupos homogéneos dentro de los datos. Este algoritmo es adecuado para agrupar los servicios de streaming en función de sus características y evaluar su relación calidad-precio. Otros algoritmos candidatos incluyen DBSCAN, que también podrían ser útiles para identificar patrones en los datos, sin embargo, a medida que avance el curso podríamos seguir probando modelos más sofisticados.

## Referencias

- [IMDB](https://www.imdb.com)
- [TMDB](https://www.themoviedb.org)
- [Netflix tech blog](https://netflixtechblog.com/)
- https://repositorio.usm.cl/server/api/core/bitstreams/d67c307d-1a49-4c90-b54d-335457c3938d/content
- https://www.xataka.com/basics/comparativa-disney-netflix-hbo-movistar-prime-video-apple-filmin-catalogo-funciones-precios

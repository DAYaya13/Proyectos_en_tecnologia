**Proyecto SQL** **Análisis de Datos de Libros**

El coronavirus tomó al mundo entero por sorpresa, cambiando la rutina diaria de todos y todas. Los habitantes de las ciudades ya no pasaban su tiempo libre fuera, yendo a cafés y centros comerciales; sino que más gente se quedaba en casa, leyendo libros. Eso atrajo la atención de las startups (empresas emergentes) que se apresuraron a desarrollar nuevas aplicaciones para los amantes de los libros.

Te han dado una base de datos de uno de los servicios que compiten en este mercado. Contiene datos sobre libros, editoriales, autores y calificaciones de clientes y reseñas de libros. Esta información se utilizará para generar una propuesta de valor para un nuevo producto.

**Diccionario de Datos**
**books**

**Contiene datos sobre libros:**

**book_id:** identificación del libro
**author_id:** identificación del autor o autora
**title:** título
**num_pages:** número de páginas
**publication_date:** fecha de la publicación
**publisher_id:** identificación de la editorial

**authors**

Contiene datos sobre autores:

**author_id:** identificación del autor o autora
**author:** el autor o la autora

**publishers**

Contiene datos sobre editoriales:

**publisher_id:** identificación de la editorial
**publisher:** la editorial

**ratings**

Contiene datos sobre las calificaciones de usuarios:

**rating_id:** identificación de la calificación
**book_id:** identificación del libro
**username:** el nombre del usuario que revisó el libro
**rating:** calificación

**reviews**

Contiene datos sobre las reseñas de los y las clientes:

review_id: identificación de la reseña
book_id: identificación del libro
username: el nombre del usuario que revisó el libro
text: el texto de la reseña

**Objetivos del estudio**

**Número de libros publicados después del 1 de enero de 2000:** Conocer uántos libros se han publicado después de esta fecha para entender la tendencia de publicaciones en el siglo XXI.

**Número de reseñas y calificación promedio por libro:** Analizar la interacción de los usuarios con los libros, midiendo cuántas reseñas han recibido y cuál es la calificación promedio.

**Editorial con más libros publicados con más de 50 páginas:** Queremos identificar la editorial más activa en la publicación de libros sustanciales, excluyendo folletos y publicaciones cortas.

**Autor con la más alta calificación promedio en libros con al menos 50 calificaciones:** Encontrar al autor más valorado por los lectores, considerando solo libros con un número significativo de calificaciones.

**Número promedio de reseñas de texto entre usuarios que calificaron más de 50 libros:** Entender el comportamiento de los usuarios más activos, midiendo cuántas reseñas de texto suelen hacer.

**Valor del Análisis**

Este proyecto permite:

Identificar patrones de publicación y lectura en el mercado editorial digital.
Reconocer autores y editoriales más valorados por los usuarios.
Comprender la interacción de los lectores más activos, generando insights clave para el desarrollo de productos y estrategias de marketing.

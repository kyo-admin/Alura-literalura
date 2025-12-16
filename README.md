
<h1>Challenge Literalura</h1> 
<img width="817" height="287" alt="image" src="https://github.com/user-attachments/assets/d8c564d2-79b2-4a5d-806e-79e1ffe52c20" />

<h2>Reseña</h2>
<p>Aplicación de Spring Boot con PostgreSQL y la API de Gutenberg
Con la resolución del desafío LiterAlura, experimentará directamente el papel de un desarrollador back-end en el día a día, creando una aplicación con conexión a una base de datos relacional. Es imprescindible que completes este desafío, ya que es una parte esencial del programa ONE, donde tendrás la oportunidad de aplicar conceptos avanzados de Java y Spring, como el consumo de APIs externas, la persistencia de datos, entre otros.</p>

<h2>Indice</h2>

<a href="https://github.com/kyo-admin/Alura-literalura/blob/main/README.md#gutendex"># Gutendex</a>

<a href="https://github.com/kyo-admin/Alura-literalura/blob/main/README.md#construyendo-una-solicitud-de-api"># Construyendo una solicitud de API</a>

<a href="https://github.com/kyo-admin/Alura-literalura/blob/main/README.md#-analizando-la-respuesta-en-formato-json"># Analizando la respuesta en formato JSON</a>

<a href="https://github.com/kyo-admin/Alura-literalura/blob/main/README.md#convertiendo-los-datos"># Convertiendo los datos</a>

<a href="https://github.com/kyo-admin/Alura-literalura/blob/main/README.md#interactuando-con-el-usuario"># Interactuando con el usuario</a>

<a href="https://github.com/kyo-admin/Alura-literalura/blob/main/README.md#consultar-libros"># Consultar libros</a>

<a href="https://github.com/kyo-admin/Alura-literalura/blob/main/README.md#persistencia-de-datos"># Persistencia de datos</a>




<h2>Gutendex</h2>
<img width="842" height="750" alt="image" src="https://github.com/user-attachments/assets/117257ed-64eb-4885-b28b-98fcb99c9874" />

<p>La API Gutendex es un catálogo de información de más de 70.000 libros presentes en Project Gutenberg (biblioteca en línea y gratuita).</p>

<p>En este paso crucial, es fundamental comprender mejor la API de los libros, revisar su documentación y aprender cómo realizar las consultas en la API. En este desafío no es necesario obtener una clave de acceso, solo realizar consultas como se describe en el sitio web oficial.</p>

<p>Asegúrate de seguir cuidadosamente las instrucciones proporcionadas por la API Gutendex.</p>

<h2>Construyendo una solicitud de API</h2>
<h3>Construyendo el Cliente para Solicitudes (HttpClient)</h3>
<p> En la tercera fase de nuestro desafío, empleamos la clase HttpClient para realizar solicitudes a la API de libros y obtener datos esenciales. El uso de HttpClient en Java facilita la conexión y la obtención de respuestas de manera eficiente. Además, proporciona una base sólida para realizar operaciones HTTP de manera más estructurada y versátil. Explorar y entender el manejo de esta clase en Java optimiza el proceso de solicitud.</p>
<h3>Construyendo la Solicitud (HttpRequest)</h3>
<p>
  Además, nos sumergimos en el uso de la clase HttpRequest para configurar y personalizar nuestras solicitudes a la API de libros. La clase HttpRequest en Java nos brinda un control detallado sobre los parámetros de nuestras solicitudes, lo que resulta esencial para adaptar la consulta a nuestras necesidades específicas. Aprender a utilizar la clase HttpRequest no solo es crucial para el éxito de nuestro proyecto, sino que también proporciona una comprensión más profunda de cómo interactuar eficientemente con APIs en Java.
</p>
<h3>Construyendo la Respuesta (HttpResponse)</h3>

<p>
  Finalmente, nos enfocamos en el uso de la interfaz HttpResponse para gestionar las respuestas recibidas de la API. La interfaz HttpResponse en Java ofrece una estructura que permite analizar y acceder a los diferentes elementos de una respuesta HTTP. Al entender cómo trabajar con esta interfaz, podrás extraer información significativa de las respuestas, como códigos de estado, encabezados y el cuerpo de la respuesta, que normalmente se presenta en formato JSON.
</p>
<img width="699" height="687" alt="image" src="https://github.com/user-attachments/assets/5dc4b9e3-e93c-477f-8584-4bc73fe4ea65" />

<h2> Analizando la respuesta en formato JSON</h2>
<p>En la cuarta fase de nuestro desafío, nos sumergimos en el análisis de la respuesta JSON utilizando la biblioteca Jackson en Java. La manipulación de datos JSON es esencial, ya que la mayoría de las respuestas de las API se presentan en este formato.
→ Para facilitar el análisis de los datos que se obtendrán de la API, recomendamos el uso del sitio de API para realizar consulta de libros o autores.
Con la biblioteca Jackson, puedes realizar el mapeo eficiente de los datos JSON a objetos Java, facilitando así la extracción y manipulación de la información necesaria.
→ No olvides agregar la biblioteca Jackson al proyecto como dependencia del archivo POM.xml - sugerimos usar la versión 2.16.
Recuerda utilizar las clases proporcionadas por Jackson, como ObjectMapper, para acceder a las distintas propiedades de la respuesta JSON.</p>
<img width="586" height="443" alt="image" src="https://github.com/user-attachments/assets/d442e59b-59ba-4643-924c-b3f6ee3f2a43" />

<h2>Convertiendo los datos</h2>
<img width="941" height="421" alt="image" src="https://github.com/user-attachments/assets/e7677af7-f369-46c4-9566-8d195ee68369" />

<p>En esta etapa, llevaremos a cabo las conversiones con los datos de libros y autores, ahora que contamos con la información en nuestro poder.raised_hands
Experimenta utilizando clases java para recibir los datos obtenidos mediante la API, transformar los atributos del cuerpo JSON a una clase Java y mostrar los resultados.
Es fundamental crear métodos específicos para manejar estos datos, lo que hará que el código sea más modular y fácil de entender, como getters, setters and toString().
→ No olvides utilizar las anotaciones @JsonIgnoreProperties y @JsonAlias para obtener los atributos deseados del cuerpo de respuesta json.</p>


<h2>Interactuando con el usuario</h2>
<img width="469" height="281" alt="image" src="https://github.com/user-attachments/assets/2d697ec5-b5ea-4bb1-9fd1-ed76c0d47fd7" />
<p>En esta etapa del desafío, nos adentraremos en la interacción con el usuario. El método Main debe implementar la interfaz CommandLineRunner y su método run() donde deberás llamar un método para exhibir el menu. En este método, debes crear un bucle para presentar a tu usuario las opciones de insercion y consulta. El usuario deberá seleccionar un número que corresponderá a la opcion numérica y proporcionar los datos que la aplicación recibirá, utilizando la clase Scanner para capturar la entrada do usuário.

Recuerda exhibirle al usuario las informaciones que han sido demandadas y informarle cuando hay un error. Además, es fundamental realizar pruebas exhaustivas para garantizar el correcto funcionamiento del programa, simulando diversas situaciones y recorridos para identificar y corregir posibles errores.</p>

<h2>Consultar libros</h2>
<img width="447" height="492" alt="image" src="https://github.com/user-attachments/assets/beede13d-ecfd-485b-9d3e-3d65dd2aee26" />

<p>Bien, ahora vamos a empezar a construir nuestro catálogo de libros y autores. En esta etapa realizamos consulta de libro en la API, con la ayuda de la URL base “https://gutendex.com/books/” (sugerimos ver la documentación oficial para diferentes ejemplos de consulta).

En este caso, realizamos la consulta por título del libro en la API para retener el primer resultado obtenido. Un libro debe tener los siguientes atributos:

Título;

Autor;

Idiomas;

Número de Descargas.

Con esta funcionalidad lista, será posible presentar en la consola un listado de todos los libros que ya fueron buscados.

Además, también debes posibilitar al usuario ver un listado con base en el idioma que uno o más libros fueron escritos, con la ayuda de las derived queries.

→ En este desafío vamos a considerar que un libro posee solo un idioma, para que las consultas hechas con tal objeto sean más comprensibles y sencillas. En otras palabras, nos quedaremos solo con el primer resultado de idioma de la lista de idiomas recibida.

En resumen tenemos estas dos funcionalidades obligatorias en el proyecto:

Búsqueda de libro por título

Lista de todos los libros</p>

<h2>Persistencia de datos</h2>
<p>Ha llegado el momento de enfocamos en construir una base de datos, con tablas y atributos relacionados a nuestros objetos de interés: Libro y Autor.

En este desafío vamos a utilizar la base de datos llamada PostgreSQL, una de las bases de datos open source más utilizadas en el mercado.</p>

<img width="854" height="429" alt="image" src="https://github.com/user-attachments/assets/73062569-9207-4f89-abcb-45a54e8fd11c" />


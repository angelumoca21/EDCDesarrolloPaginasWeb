# 3.Estructura básica de un documento HTML

El código HTML se compone de etiquetas o marcas. Las etiquetas en HTML son palabras clave que se escriben entre los signos <> y que el navegador entiende.
Normalmente las etiquetas se componen de una etiqueta de apertura (entre los signos <>), una etiqueta de cierre (entre los signos </>) y un contenido. El contenido puede ser texto u otras etiquetas. Aunque existen algunas etiquetas que no tienen ni contenido ni etiqueta de cierre, son una excepción. La sintaxis sería la siguiente:

```
<etiqueta>
    contenido
</etiqueta>    
```

HTML es un lenguaje que se compone por **elementos** que permiten definir la estructura del documento. Estos elementos son los que nos posibilitan determinar cómo estará armada la página y sus secciones. Las etiquetas nos brindan la oportunidad de definir los elementos en el código.

```
<elemento1>
    Contenido del elemento 1
</elemento1>
<elemento2>
    Contenido del elemento 2
</elemento2>
```

Todos los elementos se dividen en dos categorías:

- **Elementos en bloque:** estos son los elementos que estructuran la parte principal de la
página web, dividiendo una página en bloques coherentes. Un elemento a nivel de bloque
siempre comienza con una nueva línea y ocupa todo el ancho de la página web, de
izquierda a derecha.

Los siguientes son algunos de los elementos en bloque en HTML:
```<address>, <article>, <aside>, <blockquote>, <canvas>, <dd>, <div>, <dl>, <dt>, <fieldset>,<figcaption>, <figure>, <footer>, <form>, <h1> hasta <h6>, <header>, <hr>, <li>, <main>,<nav>, <noscript>, <ol>, <output>, <p>, <pre>, <section>, <table>, <tfoot>, <ul> y <video>```

- **Elementos en línea:** son aquellos elementos que diferencian la parte de un texto dado y le proporcionan una función particular. Estos elementos no comienzan con una nueva línea y toman el ancho según el requisito. Los elementos en línea se utilizan principalmente con otros elementos.

Los siguientes son algunos de los elementos en bloque en HTML:
```<a>, <abbr>, <acronym>, <b>, <bdo>, <big>, <br>, <button>, <cite>, <code>, <dfn>, <em>, <i>,<img>, <input>, <kbd>, <label>, <map>, <object>, <q>, <samp>, <script>, <select>, <small>,<span>, <strong>, <sub>, <sup>, <textarea>, <time>, <tt>, <var>```

Un **atributo** en HTML son palabras especiales utilizadas dentro de la etiqueta de apertura, para controlar el comportamiento del elemento. Los atributos HTML brindan información adicional sobre el elemento. Cada atributo HTML tiene su nombre y valor:

`<elemento atributo=”valor">Contenido del elemento</elemento>`

**Elementos vacíos:** algunos elementos no poseen contenido, y son llamados elementos vacíos. Por ejemplo:
`<img src="images/firefox-icon.png" alt="Mi imagen de prueba" />`
Posee dos atributos, pero no hay etiqueta de cierre `</img>` ni contenido encerrado. Esto es porque un elemento de imagen no encierra contenido al cual afectar. Su propósito es desplegar una imagen en la página HTML, en el lugar en que aparece.

## Semántica

En 2004, Ian Hickson, el autor de la especificación de HTML5, analizó 1,000,000,000 de páginas web utilizando el motor de Google, intentando identificar la manera en la que la web real estaba construida. Uno de los resultados de este análisis, fue la publicación de una lista con los nombres de clases más utilizados. Este estudio revela que los desarrolladores utilizan clases o IDs comunes para estructurar los documentos. Esto llevó a considerar que quizás fuese una buena idea crear etiquetas concretas para reflejar estas estructuras: la web semántica.

HTML5 proporciona elementos semánticos que facilitan la comprensión del código. En este sentido, la semántica define el significado de palabras y frases, es decir, tener elementos semánticos es equivalente a tener elementos con significado. Los elementos semánticos tienen un significado simple y claro tanto para el navegador como para el desarrollador.

¿Por qué usar elementos semánticos? Porque es mucho más fácil de leer, como programador podría estar leyendo cientos o miles de líneas de código. Cuanto más fácil sea leer y comprender ese código, más fácil será su trabajo.
Los motores de búsqueda y las tecnologías de asistencia (como lectores de pantalla para usuarios con discapacidad visual) también podrán comprender mejor el contexto y el contenido de tu sitio web, lo que significa una mejor experiencia para los usuarios.

HTML5 introduce elementos específicos para poder definir secciones del documento y también características que pretenden hacer de la semántica una capacidad importante para el lenguaje.

A partir de HTML5 se definen etiquetas que nos permiten estructurar el cuerpo de una página con una semántica específica para cada elemento: 
```<header> <hgroup> <nav> <section> <article> <aside> <footer> <figure> <figcaption> <time> <details> <summary> <mark>```

![HTMLsemantico](https://static.semrush.com/blog/uploads/media/0a/0f/0a0fd07d0a6ee7a7f893b0e21379c0ae/ES-Semantic-Search-Non-Semantic.png)

Vamos ahora a estructurar una página en HTML5 desde cero. En este punto ya debimos de haber realizado maquetas del sitio, analizado la necesidades, así como haber verificado aspectos de usabilidad, accesibilidad y navegabilidad.

![Mockup](https://img.freepik.com/vector-gratis/diseno-sitio-web-responsivo-diseno-plano_23-2149483805.jpg)

 Teniendo esto, partimos a andar en el camino de estructurarlo con HTML5. Una recomendación que se hace en estos casos es realizar primero la estructura HTML de las secciones más importantes del cuerpo del documento (cabecera, contenido principal, barra de navegación, pie, etcétera) y, luego, ir agregando los elementos que se incorporan en ellas: trabajaremos el código del cuerpo del documento con un encabezado `<header>`, una barra de navegación `<nav>`, seguido de un bloque principal denominado `<section>` que contiene dos artículos `<article>`, una barra con información adicional `<aside>` y también un pie `<footer>`.

```
<header>
    <h1>Título del encabezado</h1>
    <p><strong>Texto del encabezado</strong></p>
</header>
<nav>
    <ul>
        <li>Elemento 1</li>
        <li>Elemento 2</li>
    </ul>
</nav>
<section>
    <article>
        <h2>Título del artículo 1</h2>
        <p>Texto del artículo 2</p>
    </article>
    <article>
        <h2>Título del artículo 2</h2>
        <p>Texto del artículo 2</p>
    </article>
</section>
<aside>
    <h3>Título del Aside</h3>
    <p>Contenido del Aside</p>
</aside>
<footer>
    <p>Texto de pie de página</p>
</footer>
```

La estructura que hemos visto aquí puede adaptarse, fácilmente, a cualquier tipo de necesidad, ya sea un e-commerce, una red social, un foro o cualquier otra opción que podamos imaginar. Luego será solo cuestión de incorporar los elementos para personalizar nuestro proyecto y, con ellos, terminar de darle la estructura deseada a cada página.
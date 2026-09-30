# HTML5

## Unidad 9 · Ejercicios

**Módulos 0373 (LMH) · 0488 (DI)**

Lenguajes de marcas y sistemas de gestión de información (DAW) · Desarrollo de Interfaces (DAM)

Curso 2026/2027

Note:
Unidad puramente práctica: diez retos de semántica, tablas, formularios HTML5, multimedia y accesibilidad. Se resuelven en orden creciente de dificultad y por vuestro cuenta, y después se comparan con las soluciones de la unidad 10. El objetivo no es que la página «se vea bien», sino que el marcado sea <mark>semántico, accesible y validado</mark>. Pregunta de arranque: ¿quién ha abierto esta semana el validador del W3C?

---

## Objetivos de aprendizaje

<span class="fragment">1. Seguir una <mark>metodología</mark>: intento propio, validación y prueba con teclado</span>

<span class="fragment">2. Organizar los diez ejercicios en <mark>cinco bloques</mark> y subir de nivel al validar</span>

<span class="fragment">3. Interpretar el enunciado y <mark>entregar solo lo pedido</mark>, sin tocar el CSS</span>

<span class="fragment">4. Autoevaluar el trabajo con la <mark>rúbrica</mark> antes de entregar</span>

Note:
Cuatro objetivos, el segundo de proceso: se avanza bloque a bloque y solo cuando el anterior valida sin errores. El tercero es el que más falla: se termina entregando de más o se modifica el aspecto visual. La rúbrica se aplica siempre antes de pulsar «entregar», nunca después.

---

## Cómo trabajar

<span class="fragment"><mark>Intenta antes de mirar</mark>: entrega tu versión y solo después consulta la solución</span>

<span class="fragment">Valida siempre en <https://validator.w3.org/>: verlo bien en el navegador no basta</span>

<span class="fragment">Pruébalo con <mark>teclado y lector de pantalla</mark>: menús, tablas, formularios, avisos</span>

<span class="fragment"><mark>No toques el CSS</mark>: si cambia el aspecto, es que has roto la estructura</span>

<span class="fragment">Sube de nivel solo cuando valides sin errores el bloque anterior</span>

Note:
Estas cinco reglas sostienen la unidad entera. La primera evita el copia-pega automático y la segunda, el «en mi equipo se ve bien». La cuarta es el detector de errores más rápido que tenéis: si algo se descoloca, hay un contenedor mal anidado. Si un ejercicio se bloquea, volved antes a la teoría de su capítulo.

---

## Qué debo entregar

<span class="fragment">Un fichero HTML por ejercicio, con el <mark>nombre indicado</mark> en el enunciado</span>

<span class="fragment">Código comentado donde se explique el <mark>porqué</mark> de cada etiqueta elegida</span>

<span class="fragment">Las respuestas escritas al quiz del ejercicio 6 y a la lista del ejercicio 10</span>

<span class="fragment">El informe del validador W3C de la <mark>última versión</mark>, sin errores</span>

<span class="fragment">El texto idéntico al código inicial: <mark>solo cambian los contenedores</mark></span>

Note:
Entregar no es solo el HTML: también van las respuestas escritas y el informe del validador. El comentario del código debe justificar la decisión, no repetir el nombre de la etiqueta. Si el texto del enunciado aparece alterado, el ejercicio se devuelve corregido. El nombre del fichero también cuenta: sin él no se localiza la entrega.

---

## Criterios de evaluación

<span class="fragment"><mark>Semántica</mark>: landmarks bien usados en lugar de div, sin ninguno sobrante</span>

<span class="fragment"><mark>Encabezados</mark>: un solo h1 y niveles sin saltos</span>

<span class="fragment"><mark>Textos y tablas</mark>: time, abbr, blockquote, caption y th con scope</span>

<span class="fragment"><mark>Formularios</mark>: tipos nativos, required, pattern y etiquetas visibles</span>

<span class="fragment"><mark>Accesibilidad</mark>: skip link, teclado, ARIA y lector de pantalla</span>

<span class="fragment">Separa Excelente de Suficiente: <mark>validar sin errores</mark> y repasar el teclado</span>

Note:
Son los ocho criterios de la rúbrica comprimidos en seis líneas. Un trabajo puede lucir idéntico al excelente y quedarse en Suficiente por un validador con errores o por un foco invisible. Los tres primeros puntos son los que más pesan en la nota final. El último es la frontera real entre un cinco y un diez.

---

## Cómo se corrige cada ejercicio

<div class="mermaid">
graph LR
  A[Enunciado<br>y código inicial] --> B[Intento propio<br>sin mirar solución]
  B --> C[Validador W3C<br>sin errores]
  C --> D[Prueba con teclado<br>y lector de pantalla]
  D --> E[Entrega comentada<br>con el quiz]
</div>

<span class="fragment">Si un paso falla, se <mark>retrocede</mark>: no se parchea el siguiente</span>

Note:
Este es el flujo que se espera de vosotros en cada ejercicio, no solo en el último. La validación va antes de la entrega y la prueba de accesibilidad antes de cerrar el fichero. El paso que más se salta es el segundo: intentar sin mirar.

---

## Bloque A · Estructura semántica

<div style="font-size: 1em; text-align: left;">

Ejercicios 1 y 3 · capítulo 07 · <mark>acabar con la divitis</mark>

</div>

<span class="fragment">Ej. 1: header, nav, main y footer en lugar de los cuatro div</span>

<span class="fragment">Ej. 3: un solo main y fragmentos #inicio, #proyectos y #contacto</span>

<span class="fragment">Cada proyecto en article con h3, párrafo, enlace e imagen con alt</span>

<span class="fragment">figure + figcaption para el avatar; aside para el bloque de contacto</span>

<span class="fragment">Los id referenciados deben existir: el menú no puede apuntar al vacío</span>

Note:
Aquí entran los ejercicios 1 y 3, los dos que más se parecen: uno sustituye contenedores y el otro monta una página completa. La clave es no alterar el texto ni el aspecto. Si sobra un div, es que no lo habéis sustituido: lo habéis duplicado.

---

## Bloque B · Textos enriquecidos

<div style="font-size: 1em; text-align: left;">

Ejercicios 2 y 4 · capítulo 02 · <mark>marcar fechas, citas, siglas e imágenes</mark>

</div>

<span class="fragment">Ej. 2: article con header interno, dos section y footer propio</span>

<span class="fragment">Fecha con time datetime en <mark>formato ISO</mark>: 2026-06-10</span>

<span class="fragment">Ej. 4: abbr para IA y ANDA, blockquote con cite para la cita</span>

<span class="fragment">figure con figcaption <mark>distinto</mark> del alt de la imagen</span>

<span class="fragment">Tabla con caption, thead, tfoot y th scope en filas y columnas</span>

Note:
Ejercicios 2 y 4: el enriquecimiento de textos. La fecha legible por máquina y la tabla con cabeceras declaradas son los dos puntos donde más se pierden notas. Recuerda que figcaption y alt nunca deben repetir el mismo texto.

---

## Bloque C · Perfil y formularios

<div style="font-size: 1em; text-align: left;">

Ejercicios 5 y 7 · capítulos 07 y 06 · <mark>validar en cliente sin JavaScript</mark>

</div>

<span class="fragment">Ej. 5: secciones jerarquizadas con h2 y h3, sin saltos de nivel</span>

<span class="fragment">fieldset con legend y label for/id en <mark>todos</mark> los campos</span>

<span class="fragment">Ej. 7: tipos email, date y number con min 16 y max 99</span>

<span class="fragment">required en los obligatorios; pattern con su title explicativo</span>

<span class="fragment">datalist para los ciclos, textarea rows=4 y button type=submit</span>

Note:
Ejercicios 5 y 7: secciones jerarquizadas y validación nativa. Aquí se concentran los errores de etiqueta asociada, el label sin for y el fieldset sin legend. Si pulsar el texto no lleva el foco al campo, el for está mal escrito.

---

## Bloque D · Tablas y multimedia

<div style="font-size: 1em; text-align: left;">

Ejercicios 8 y 6 · capítulos 05 y 04 · <mark>tabla accesible y canvas</mark>

</div>

<span class="fragment">Ej. 8: caption, thead, tbody, tfoot y th scope en filas y columnas</span>

<span class="fragment">Todos los huecos con colspan: las filas suman las <mark>mismas celdas</mark></span>

<span class="fragment">Ej. 6: video con crossorigin y canvas con willReadFrequently</span>

<span class="fragment">Bucle drawImage, getImageData y putImageData con requestAnimationFrame</span>

<span class="fragment">Respuestas escritas al quiz: canvas vacío, paso de cuatro en cuatro</span>

Note:
El ejercicio 8 es tabla accesible y el 6 es el único que permite JavaScript, porque canvas lo exige. En la tabla se mira el scope y la cuadratura de las filas; en canvas, el crossorigin y el avance de cuatro en cuatro. Ambos admiten prueba objetiva: lector de pantalla y pestaña oculta. Ninguno de los dos se puede dar por bueno solo con mirarlos.

---

## Bloque E · Accesibilidad total

<div style="font-size: 1em; text-align: left;">

Ejercicios 9 y 10 · capítulos 03, 04 y 07 · <mark>recorrer con teclado</mark>

</div>

<span class="fragment">Ej. 9: figure en vez de «ver imagen», alt ≠ figcaption</span>

<span class="fragment">srcset con sizes y versiones de 400, 800 y 1600 px</span>

<span class="fragment">Vídeo con poster y dos track: subtítulos en español e inglés</span>

<span class="fragment">Ej. 10: skip link como <mark>primer elemento</mark> del body</span>

<span class="fragment">aria-expanded con aria-controls; role=status en los avisos</span>

Note:
Ejercicios 9 y 10, los más exigentes porque piden accesibilidad real, no decorativa. Todo se comprueba con el teclado y el lector de pantalla, sin librerías. Si el skip link no aparece con el primer Tab, el ejercicio queda incompleto.

---

## Ejemplo resuelto · De divitis a landmarks

<div style="font-size: 1em; text-align: left;">

Ejercicio 1, esqueleto final: <mark>solo cambian los contenedores</mark>

</div>

```html
<body>
  <header>
    <h1>Bienvenido a mi Web</h1>
    <nav><ul><li><a href="#">Inicio</a></li><li><a href="#">Contacto</a></li></ul></nav>
  </header>
  <main><p>Este es el contenido principal de la página.</p></main>
  <footer><p>&copy; 2026 Mi Web</p></footer>
</body>
```

<span class="fragment"><mark>nav dentro de header</mark> si el menú es parte de la cabecera</span>

<span class="fragment">El <code>h1</code> y la lista de enlaces intactos: solo cambia el contenedor</span>

<span class="fragment">Ninguna etiqueta necesita atributos: la semántica la da el nombre</span>

Note:
Es el ejercicio 1 reducido a su mínima expresión: cuatro etiquetas de bloque y ningún atributo. El nav queda dentro del header porque el menú forma parte de la cabecera de la página. Fijaos en que el texto no ha cambiado ni una coma. Si el aspecto se modifica, es señal de que se ha tocado algo que no tocaba.

---

## Ejemplo resuelto · Matrícula validada

<div style="font-size: 1em; text-align: left;">

Ejercicio 7, dos campos con <mark>validación nativa</mark> sin JavaScript

</div>

```html
<form action="/matricula" method="post">
  <fieldset>
    <legend>Datos del estudiante</legend>
    <p><label for="email">Correo</label>
       <input type="email" id="email" name="email" required></p>
    <p><label for="nif">NIF</label>
       <input type="text" id="nif" pattern="[0-9]{8}[A-Za-z]"
              title="Ocho dígitos y una letra" required></p>
    <label for="ciclo">Ciclo</label> <input id="ciclo" list="ciclos" required>
    <datalist id="ciclos"><option value="DAM"><option value="DAW"></datalist>
  </fieldset>
</form>
```

<span class="fragment"><mark>pattern + title</mark>: la expresión valida y el title explica el error</span>

<span class="fragment">El datalist se asocia con <code>list="ciclos"</code> frente al <code>id="ciclos"</code></span>

Note:
Dos campos muestran las tres piezas de la validación nativa: tipo correcto, required y pattern. El title solo aparece cuando la expresión no coincide, por eso debe describir el formato esperado. El datalist sugiere sin cerrar la opción: eso lo hace el select. Con esto el formulario rechaza los datos inválidos antes de enviarlos.

---

## Antes de entregar

<span class="fragment">He validado el HTML en el W3C sin <mark>errores</mark></span>

<span class="fragment">He recorrido la página solo con <mark>teclado</mark>: el foco siempre visible</span>

<span class="fragment">Ninguna imagen sin <code>alt</code> y ninguna leyenda repitiendo su <code>alt</code></span>

<span class="fragment">Todos los campos con <mark>etiqueta visible</mark> y con tipo nativo</span>

<span class="fragment">El <mark>texto no ha cambiado</mark> respecto al inicial y ningún div sobra</span>

<span class="fragment">He probado con lector de pantalla tablas, formularios y avisos</span>

Note:
Este checklist es el mínimo para dar un ejercicio por terminado. Los dos puntos más olvidados son el foco visible con teclado y comprobar que ninguna leyenda repite el alt. Pasadlo antes de cada entrega, no solo al final de la unidad.

---

## Errores frecuentes

<span class="fragment">Repetir <code>main</code> o dejar el menú como <code>div</code> a medio convertir</span>

<span class="fragment">Varios <code>h1</code> por página o saltos de <code>h1</code> a <code>h3</code></span>

<span class="fragment">Tabla de puras <code>td</code> y encabezados declarados sin <code>scope</code></span>

<span class="fragment"><code>label</code> sin <code>for</code>, <code>pattern</code> sin <code>title</code> y sin <code>required</code></span>

<span class="fragment"><code>target="_blank"</code> sin <code>rel="noopener"</code> y vídeos sin <code>track</code></span>

Note:
Casi todos los fallos de esta lista son de detalle y se detectan en dos minutos con el validador. El de los encabezados es el más costoso de corregir después, porque obliga a reordenar toda la página. El de ARIA aparece en los ejercicios 9 y 10. Si los conocéis de antemano, os ahorráis la segunda entrega.

---

## Autoevaluación

Sin mirar todavía la solución: ¿qué cuatro etiquetas sustituyen a la «divitis», cuál puede haber **solo una vez** por página y qué atributo declara la dirección de un `<th>`?

<span class="fragment"><mark>Respuesta:</mark> <code>header</code>, <code>nav</code>, <code>main</code> y <code>footer</code>; un solo <code>main</code>; la dirección la declara <code>scope</code></span>

Note:
Tres datos que salen en casi cualquier examen de esta unidad. Si dudas con los landmarks, recuerda que header y footer pueden repetirse dentro de secciones, pero main solo una vez. El scope es col para columnas y row para filas, junto a caption y thead o tfoot.

---

## Claves para el examen

<span class="fragment"><mark>Cuatro landmarks</mark>: header, nav, main y footer, y solo un main</span>

<span class="fragment"><mark>section</mark> lleva encabezado; sin él, sigue siendo un div</span>

<span class="fragment">Fecha con time en <mark>formato ISO</mark>; tabla con caption y scope</span>

<span class="fragment">Formulario: etiqueta visible, tipo nativo, required y pattern con title</span>

<span class="fragment">Accesibilidad: skip link, foco visible, aria-expanded y role=status</span>

<span class="fragment">Validar en el W3C y no tocar el CSS: lo primero que mira la rúbrica</span>

Note:
Si memorizáis estas seis líneas, tenéis media unidad 9 hecha. La mitad de los errores de corrección son de jerarquía de encabezados y de formularios sin etiqueta. El validador y el teclado son los dos instrumentos de comprobación que pide la rúbrica.

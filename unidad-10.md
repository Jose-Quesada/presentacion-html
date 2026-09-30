# HTML5

## Unidad 10 · Ejercicios: soluciones

**Módulos 0373 (LMH) · 0488 (DI)**

Lenguajes de marcas y sistemas de gestión de información (DAW) · Desarrollo de Interfaces (DAM)

Curso 2026/2027

Note:
Aquí están las soluciones comentadas de los diez retos de la unidad 9. Cada bloque es código completo y funcional, pero se usa para comparar con vuestra versión; copiarlo sin entenderlo no cuenta como ejercicio. Nos centraremos en los <mark>puntos clave</mark> y en el error típico de cada ejercicio. Pregunta de arranque: ¿cuántos habéis entregado ya la unidad 9?

---

## Cómo usar estas soluciones

<span class="fragment"><mark>Compara, no copies</mark>: si tu versión difiere, rehazla antes de seguir</span>

<span class="fragment">Cada diapositiva resume el <mark>punto clave</mark> y el error típico del ejercicio</span>

<span class="fragment">Lee primero los puntos clave y solo después abre el código completo</span>

<span class="fragment">Si tu solución usa otra etiqueta, comprueba antes en la teoría cuál es la correcta</span>

<span class="fragment">Corrige sobre tu propio fichero: <mark>la entrega sigue siendo tuya</mark></span>

Note:
La regla de oro es comparar y justificar, no transcribir. Si vuestra solución llega al mismo resultado por otro camino, comprobadlo en el apunte antes de darlo por bueno. Los errores típicos se repiten curso tras curso: merece la pena leerlos. El formato de estas diapositivas es el mismo que se pide en los comentarios del entregable.

---

## Objetivos de aprendizaje

<span class="fragment">1. Contrastar cada entrega con la <mark>solución de referencia</mark> y justificar las diferencias</span>

<span class="fragment">2. Interiorizar los <mark>puntos clave</mark> de semántica, tablas, formularios y multimedia</span>

<span class="fragment">3. Corregir los <mark>errores típicos</mark> que más se repiten en la corrección</span>

<span class="fragment">4. Fijar las <mark>claves para el examen</mark> a partir de ejemplos reales resueltos</span>

Note:
Cuatro objetivos centrados en la comparación crítica entre vuestra versión y la de referencia. El tercero es el que más os va a servir para el examen, porque los fallos son siempre los mismos. El cuarto conecta directamente con el cierre de la unidad.

---

## Solución 1 · De divitis a landmarks

<span class="fragment"><mark>Exigía:</mark> quitar la divitis sin cambiar una sola palabra del texto</span>

```html
<header>
  <h1>Bienvenido a mi Web</h1>
  <nav><ul><li><a href="#">Inicio</a></li></ul></nav>
</header>
<main><p>Este es el contenido principal de la página.</p></main>
<footer><p>&copy; 2026 Mi Web</p></footer>
```

<span class="fragment">nav se anida en header cuando el menú forma parte de la cabecera</span>

<span class="fragment"><mark>Error típico:</mark> repetir main o dejar el menú como div</span>

Note:
El ejercicio 1 es el más rápido de corregir: se mira si el texto sigue intacto y si hay un único main. nav dentro de header es correcto cuando el menú pertenece a la cabecera de la página. Si queda un div class=menu, el ejercicio sigue empezado.

---

## Solución 2 · Artículo semántico

<span class="fragment"><mark>Exigía:</mark> article con header interno, dos section y footer propio</span>

<span class="fragment">La fecha va con <code>time datetime="2026-06-10"</code> y el texto visible en español</span>

<span class="fragment">«Recetas» sube de h3 a h2: cada section lleva su <mark>encabezado</mark></span>

<span class="fragment">header y footer internos pertenecen al artículo, no a la página</span>

<span class="fragment"><mark>Error típico:</mark> dos h1 por página o un h3 tras el h1</span>

Note:
La fecha es el punto que más se olvida: visible para las personas e ISO para las máquinas. Cada section necesita su encabezado propio, por eso Recetas sube un nivel. header y footer internos delimitan el artículo, no la web entera. Si falta una de las dos section, el artículo pierde sus bloques temáticos.

---

## Solución 3 · Portafolio semántico

<span class="fragment"><mark>Exigía:</mark> un solo main, fragmentos que apunten a ids reales y figure</span>

<span class="fragment">Los id #inicio y #proyectos coinciden con los enlaces del nav</span>

<span class="fragment">alt describe la imagen y figcaption la contextualiza: <mark>nunca el mismo texto</mark></span>

<span class="fragment">Cada proyecto en article con h3, párrafo, enlace e imagen con width y height</span>

<span class="fragment"><mark>Error típico:</mark> target=_blank sin rel=noopener e imágenes sin tamaño</span>

Note:
Comprueba que cada fragmento del menú apunta a un id que exista; si no, el enlace no lleva a ningún sitio. alt y figcaption tienen que aportar información distinta entre sí. rel=noopener es obligatorio en todo target que abra pestaña nueva. Las imágenes con width y height evitan el salto de contenido mientras cargan.

---

## Solución 4 · Noticia con detalles

<span class="fragment"><mark>Exigía:</mark> header con time, figure, abbr, blockquote y tabla completa</span>

<span class="fragment">blockquote con cite marcan la cita y su fuente; abbr evita repetir siglas</span>

<span class="fragment">Tabla con caption, thead scope=col, cabeceras scope=row y tfoot</span>

<span class="fragment">Dos time con <mark>fecha ISO</mark> para el rango del 16 al 18 de junio</span>

<span class="fragment"><mark>Error típico:</mark> tabla de puras td y figcaption idéntico al alt</span>

Note:
La tabla es lo más trabajado del ejercicio: caption, cabeceras de columna y de fila, y pie con el total. La cita necesita blockquote y cite, no comillas sueltas dentro del párrafo. Los dos time del rango llevan fecha ISO cada uno.

---

## Solución 5 · Perfil con formularios

<span class="fragment"><mark>Exigía:</mark> secciones jerarquizadas y dos formularios etiquetados</span>

<span class="fragment">Jerarquía de títulos: h2 global del perfil y h3 por bloque interno</span>

<span class="fragment">Cada label apunta con for al id: el clic en el texto <mark>enfoca el campo</mark></span>

<span class="fragment">ol con time en la actividad; fieldset con legend en ambos formularios</span>

<span class="fragment"><mark>Error típico:</mark> label sin for y casillas sin etiqueta asociada</span>

Note:
La jerarquía de títulos es lo primero que se revisa en este ejercicio. for e id deben coincidir en todos los campos, incluidas las casillas de preferencias. Si el foco no salta al pulsar la etiqueta, falta el for o el id está mal escrito. El mismo criterio se aplica al select y a cualquier control de los dos formularios.

---

## Solución 6 · Vídeo en canvas

<span class="fragment"><mark>Exigía:</mark> vídeo como fuente de píxeles y canvas como render en paralelo</span>

```javascript
for (let i = 0; i < data.length; i += 4) {
  const gris = 0.2126 * data[i] + 0.7152 * data[i+1] + 0.0722 * data[i+2];
  data[i] = gris; data[i+1] = gris; data[i+2] = gris;
}
ctx.putImageData(frame, 0, 0);
requestAnimationFrame(procesarFrame);
```

<span class="fragment">El bucle arranca en el evento play y se corta cuando el vídeo queda en pausa</span>

<span class="fragment"><mark>Error típico:</mark> olvidar crossorigin o recorrer el array de uno en uno</span>

Note:
Aquí está el núcleo del ejercicio 6: luminancia ponderada y avance de cuatro en cuatro. El canal alfa no se toca, porque dejarlo en cero volvería transparente el lienzo. El bucle se dispara en play y se frena solo cuando el vídeo se pausa.

---

## Ejercicio 6 · Las cuatro respuestas

<span class="fragment">El canvas está vacío al cargar: dibuja el primer drawImage al empezar el play</span>

<span class="fragment">Se recorre de 4 en 4 porque ImageData guarda <mark>RGBA</mark> por píxel</span>

<span class="fragment">setInterval pierde sincronía con el refresco y corre en pestañas ocultas</span>

<span class="fragment">Solo con el canal verde los rojos salen negros y los verdes, muy brillantes</span>

Note:
Son las cuatro preguntas escritas del enunciado, y las cuatro puntúan. La de setInterval es la que separa un trabajo completo de uno a medias, porque toca refresco y pestañas ocultas. Repasad también la diferencia entre gris por luminancia y gris por canal verde.

---

## Solución 7 · Formulario de matrícula

<span class="fragment"><mark>Exigía:</mark> validar en cliente con HTML5 y sin una línea de JavaScript</span>

```html
<input type="text" id="nif" name="nif" pattern="[0-9]{8}[A-Za-z]"
       title="Ocho dígitos y una letra" required>
<label for="ciclo">Ciclo</label> <input id="ciclo" list="ciclos" required>
<datalist id="ciclos">
  <option value="DAM"><option value="DAW"><option value="SMR">
</datalist>
```

<span class="fragment">required, email, date y min o max cubren los campos obligatorios</span>

<span class="fragment">datalist <mark>sugiere sin cerrar</mark> la opción; para cerrarla se usa select</span>

Note:
Toda la validación es nativa: required, email, date, min y max, pattern. El datalist se asocia al campo con list y su id debe coincidir. Si queréis impedir valores distintos de los ciclos, entonces toca un select, no un datalist.

---

## Error común: formularios sin etiqueta

<span class="fragment"><code>label</code> sin <code>for</code>: el clic en el texto no llega al campo</span>

<span class="fragment"><code>pattern</code> sin <code>title</code>: el navegador no puede explicar el fallo</span>

<span class="fragment">Obligatorios sin <code>required</code>: se envían correos vacíos y fechas imposibles</span>

<span class="fragment">La validación nativa <mark>complementa</mark> a la etiqueta visible, no la sustituye</span>

Note:
Son los tres fallos que más se repiten en este ejercicio y los tres se ven al probar el formulario. Un label sin for no rompe la página, pero la rúbrica lo castiga en accesibilidad. El pattern sin title deja al usuario sin explicación del error.

---

## Solución 8 · Horario accesible

<span class="fragment"><mark>Exigía:</mark> tabla legible por lector de pantalla y filas cuadradas</span>

```html
<caption>Horario del grupo 1º DAM - Curso 2026/2027</caption>
<thead><tr><th scope="col">Hora</th><th scope="col">Lunes</th></tr></thead>
<tr><th scope="row">08:00-09:00</th><td>LMH</td></tr>
<tr><th scope="row">09:00-10:00</th><td colspan="2">Hora de patrocinio</td></tr>
<tfoot><tr><th scope="row">Total</th><td colspan="2">12 horas</td></tr></tfoot>
```

<span class="fragment">Todas las filas suman el <mark>mismo número de celdas</mark> contando colspan</span>

<span class="fragment">El código completo añade además <code>tbody</code> y <code>colgroup</code> con su <code>col</code></span>

Note:
La tabla se comprueba leyéndola con lector de pantalla: cada celda debe anunciar su columna y su fila. Todas las filas deben cuadrar contando los colspan, incluido el pie. colgroup fija el ancho de la columna de horas sin tocar el CSS.

---

## Error común: tablas sin scope

<span class="fragment"><code>th</code> sin <code>scope</code>: el lector no sabe si describe fila o columna</span>

<span class="fragment">Encabezados escritos como <code>td</code> «en negrita»: no declaran nada</span>

<span class="fragment"><code>colspan</code> mal colocado descuadra el total de celdas de la tabla</span>

<span class="fragment">Sin <code>caption</code>, la tabla carece de <mark>título accesible</mark></span>

Note:
Este error es invisible a simple vista porque la tabla se ve bien: por eso hay que probarla con lector de pantalla. Los th sin scope obligan a adivinar de qué fila o columna habla cada dato. El colspan mal colocado rompe la cuadratura que pide el enunciado.

---

## Solución 9 · Galería accesible

<span class="fragment"><mark>Exigía:</mark> imágenes adaptativas, descarga informada y vídeo con subtítulos</span>

<span class="fragment">figure con figcaption y sin enlaces «ver imagen» redundantes</span>

<span class="fragment">srcset con sizes y versiones de 400, 800 y 1600 px, con width y height</span>

<span class="fragment">El enlace de descarga indica <mark>formato y peso</mark> del fichero</span>

<span class="fragment">Vídeo con poster y dos track: español con default e inglés</span>

<span class="fragment"><mark>Error típico:</mark> vídeos sin track, inaccesibles para personas sordas</span>

Note:
La pareja srcset y sizes es lo que más se olvida, y sin ella el navegador elige a ciegas entre las versiones. El texto del enlace de descarga debe informar de formato y peso, como pide el enunciado. Los dos track convierten el vídeo en contenido accesible. Sin poster, el vídeo arranca en un fotograma arbitrario y pierde contexto.

---

## Solución 10 · Landmarks y skip link

<span class="fragment"><mark>Exigía:</mark> recorrer la web con teclado y anunciar estados, sin librerías</span>

<span class="fragment">El skip link es el <mark>primer elemento</mark> del body, hacia #contenido</span>

<span class="fragment">main con tabindex=-1 para recibir el foco fuera del tabulador</span>

<span class="fragment">Botón con aria-expanded, aria-controls y aria-label que alterna el menú</span>

<span class="fragment">role=status en los avisos: anuncia <mark>sin robar el foco</mark></span>

Note:
Es el ejercicio mejor valorado de la unidad porque junta todos los requisitos de accesibilidad. El skip link debe mover el foco de verdad, no solo desplazar la página. aria-expanded solo tiene sentido si algo alterna su estado realmente.

---

## Error común: botones falsos con div

<span class="fragment">Un <code>div onclick</code> haciendo de botón: no es enfocable ni anuncia estado</span>

<span class="fragment"><code>aria-expanded</code> dejado en false tras abrir el menú: atributo muerto</span>

<span class="fragment">El skip link solo haciendo scroll en vez de <mark>trasladar el foco</mark></span>

<span class="fragment">Avisos en un div normal: los cambios de texto no se anuncian solos</span>

Note:
Un div con onclick no es un botón para el teclado ni para el lector de pantalla. aria-expanded dejado en false no lo detecta el validador, pero sí la prueba con lector. Esta corrección se comprueba con teclado en menos de un minuto.

---

## Claves para el examen

<span class="fragment"><mark>Landmarks</mark>: un solo main; nav en header si forma parte de él</span>

<span class="fragment"><mark>section</mark> con encabezado, time con ISO, abbr y blockquote con cite</span>

<span class="fragment">Tabla: caption, thead y tfoot, th con scope, colspan que <mark>cuadra</mark></span>

<span class="fragment">Formulario: label con for, tipo nativo, required y pattern con title</span>

<span class="fragment">Multimedia: alt ≠ figcaption, srcset con sizes, poster y track</span>

<span class="fragment">Accesibilidad: skip link primero, aria-expanded real y role=status</span>

Note:
Estas seis líneas resumen lo que se espera recordar de los diez ejercicios. Si en el examen os piden una tabla o un formulario, la mitad de la respuesta ya está aquí. Lo demás lo da la práctica con el validador y el teclado. Repasad también los tres errores comunes: son los que más puntos restan en la corrección.

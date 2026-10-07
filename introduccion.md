# HTML5 y CSS

## Apuntes de interfaces

**Módulos 0373 (LMH) · 0488 (DI)**

Lenguajes de marcas y sistemas de gestión de información (DAW) · Desarrollo de Interfaces (DAM)

Curso 2026/2027

Note:
Bienvenidos a los apuntes de interfaces, el material de apoyo de HTML5 y CSS de los módulos de interfaces de DAW y DAM. Todo lo que veréis aquí se explica también en clase: teoría concisa, ejemplos comentados y ejercicios con solución, siempre con el mismo formato para que podáis estudiar con un método fijo. Esta primera presentación es la del curso: qué veremos, con qué módulos se relaciona y cómo leer las diapositivas. Pregunta para empezar: ¿cuántos habéis tocado HTML antes de este curso, y cuántos habéis abiado alguna vez un .html en un editor?

---

## Objetivos de aprendizaje

<span class="fragment">1. Explicar qué es <mark>HTML5</mark> y qué papel cumple <mark>CSS</mark> en una página web</span>

<span class="fragment">2. Situar los tres módulos: <mark>0373, 0615 y 0488</mark> y su ciclo formativo</span>

<span class="fragment">3. Reconocer el mapa del material: <mark>10 unidades de HTML y 16 de CSS</mark></span>

<span class="fragment">4. Interpretar las señales de las diapositivas: <mark>mark, fragment y Note</mark></span>

Note:
Cuatro objetivos: los dos primeros son conceptuales y los dos últimos os sitúan dentro del material. El tercero os da la fotografía completa del curso para que sepáis en todo momento dónde estáis y qué os queda por ver. El cuarto es práctico y urgente: si no entendéis el formato de estas diapositivas, perdéis las notas del profesor, y ahí es donde se indican las preguntas de examen. Al final de la sesión deberíais poder explicar estos cuatro puntos a un compañero que no haya venido a clase.

---

## ¿Por qué HTML5 y CSS?

<div style="font-size: 1em; text-align: left;">

Toda la web que usáis se escribe con estos dos lenguajes.
</div>

<span class="fragment">HTML5 describe la <mark>estructura</mark>: qué hay en la página</span>

<span class="fragment">CSS describe la <mark>presentación</mark>: cómo se ve</span>

<span class="fragment">Separar capas: cambiar el diseño sin tocar el contenido</span>

<span class="fragment">Reutilizable: pantalla, móvil, papel o leída en voz alta</span>

<span class="fragment">Base sobre la que se montan Angular, React o Vue</span>

Note:
La idea fuerza del curso es la separación de capas: el contenido no sabe nada de su aspecto y el estilo no decide el significado. De ahí salen páginas accesibles, imprimibles y fáciles de mantener, que es exactamente lo que se pide en el mundo profesional. Pregunta al grupo: si desactiváis el CSS de una web conocida, ¿sigue siendo utilizable? Si la respuesta es no, el HTML estaba mal construido y dependía del aspecto para tener sentido.

---

## HTML, CSS y JavaScript

| Tecnología | Pregunta | Capa | Archivo |
|---|---|---|---|
| **HTML** | ¿Qué hay? | Estructura | `.html` |
| **CSS** | ¿Cómo se ve? | Presentación | `.css` |
| **JavaScript** | ¿Qué hace? | Comportamiento | `.js` |

<span class="fragment">Los cimientos y las paredes, la pintura y la instalación</span>

<span class="fragment">Tres capas, tres ficheros, tres responsabilidades</span>

<span class="fragment">Así se reparte el trabajo y se cachea cada parte</span>

Note:
Tabla de cabecera del curso y también de examen: HTML no programa, solo declara significado. Lo que debe lucir va en CSS y lo que debe ocurrir va en JavaScript, siempre en ficheros separados. En el módulo 0373 veremos HTML5 entero, en el 0615 el CSS completo y en el 0488 cómo se combinan con un framework. Si os preguntan «¿dónde pongo el color?», la respuesta es siempre: en el CSS.

---

## Los tres módulos y marco normativo

<div style="font-size: 1em; text-align: left;">

Este material alimenta tres módulos de dos ciclos formativos (FP Grado Superior):
</div>

<span class="fragment"><strong>0373 · LMH</strong> — Lenguajes de marcas y SGI (DAW 1.º)</span>

<span class="fragment"><strong>0615 · DIW</strong> — Diseño de interfaces web (DAW 2.º)</span>

<span class="fragment"><strong>0488 · DI</strong> — Desarrollo de interfaces (DAM 2.º)</span>

<span class="fragment">Mismo contenido, distinto énfasis: HTML, CSS, frameworks y accesibilidad</span>

Note:
Los tres módulos comparten material porque comparten tecnología: primero se aprende a escribir el contenido y después a vestirlo y a llevarlo a un framework. En DAW tenéis 0373 y 0615; en DAM, 0488 recoge lo esencial de ambos antes de aterrizar en componentes. Pregunta: ¿alguien sabe ya en qué módulo le tocará evaluar cada una de estas unidades? Vale la pena aclararlo hoy para saber qué os van a preguntar y cuándo.

--

## Marco normativo en Andalucía

| Ámbito | DAW (Web) | DAM (Multiplataforma) |
|---|---|---|
| **Real Decreto (BOE)** | RD 686/2010 | RD 453/2010 |
| **Orden (BOJA)** | Orden 16/06/2011 (BOJA 149) | Orden 16/06/2011 (BOJA 150) |
| **Módulos clave** | 0373 (LMH) · 0615 (DIW) | 0488 (DI) |

<span class="fragment">Nuevo marco FP: <mark>Ley Orgánica 3/2022</mark> y <mark>Real Decreto 659/2023</mark></span>

<span class="fragment">Accesibilidad legal obligatoria: <mark>Real Decreto 1112/2018</mark> (UNE-EN 301549 / WCAG AA)</span>

Note:
Marco normativo que fundamenta la programación didáctica: RD 686/2010 y Orden 16/06/2011 (BOJA 149) para DAW; RD 453/2010 y Orden 16/06/2011 (BOJA 150) para DAM. Ambos bajo la Ley Orgánica 3/2022 y RD 659/2023. Además, el RD 1112/2018 exige accesibilidad obligatoria según la norma UNE-EN 301549 y los estándares WCAG en el desarrollo web y de aplicaciones.

---

## Mapa de contenidos · HTML5

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 0.5rem; font-size: 1em; text-align: left;">

<div class="fragment">
1. Introducción a HTML5<br>
2. Texto y semántica<br>
3. Enlaces y recursos<br>
4. Multimedia<br>
5. Tablas de datos
</div>

<div class="fragment">
6. Formularios HTML5<br>
7. Estructura semántica y ARIA<br>
8. APIs y funcionalidades nativas<br>
9. Ejercicios por niveles<br>
10. Ejercicios: soluciones
</div>

</div>

<span class="fragment">Unidades 1 y 2 esta semana: sintaxis y semántica, la base de todo lo demás</span>

Note:
Diez capítulos que cubren todo lo esencial de HTML5, con una batería de ejercicios por niveles y sus soluciones completas. Las unidades 1 y 2 sientan la sintaxis y la semántica; sin ellas no se entiende nada de las demás, así que dedíquenles tiempo. Las soluciones (unidad 10) se consultan solo después de intentarlo: si las abrís antes, el ejercicio no cuenta para el criterio de evaluación. El capítulo 9 ya lleva los criterios de evaluación de cada reto, así que conviene leerlos antes de empezar a escribir código.

---

## Mapa de contenidos · CSS

<div style="font-size: 1em; text-align: left;">

Dieciséis unidades, de la 00 a la 15, ordenadas en cinco bloques:
</div>

<span class="fragment"><strong>Base</strong>: 00 Normativa · 01 Fundamentos · 02 Selectores · 03 Modelo de caja</span>

<span class="fragment"><strong>Maquetación</strong>: 04 Posicionamiento · 05 Flexbox · 06 Grid · 07 Flujo y display</span>

<span class="fragment"><strong>Estilo</strong>: 08 Unidades y tipografía · 09 Fondos e imágenes</span>

<span class="fragment"><strong>Avanzado</strong>: 10 Responsivo · 11 Transiciones · 12 CSS moderno</span>

<span class="fragment"><strong>Calidad</strong>: 13 Accesibilidad · 14 Rendimiento · 15 Ejercicios y glosario</span>

Note:
El bloque de CSS va de la normativa al CSS moderno, y siempre en este orden: sin modelo de caja no hay Flexbox, y sin Flexbox no hay Grid. Fijaos que la accesibilidad y el rendimiento cierran el recorrido: son la revisión final de todo lo anterior, no un tema aparte. Si venís de 1.º, ya habéis tocado las cuatro primeras unidades; si empezáis de cero, no os asustéis: el bloque arranca sin presupuestos. Cada bloque cierra con ejercicios, y los del bloque de maquetación son los que más tiempo consumen.

---

## Cómo leer estas diapositivas

<div style="font-size: 1em; text-align: left;">

Cada fichero <code>.md</code> es una presentación reveal.js; los guiones crean diapositivas nuevas.
</div>

<span class="fragment"><code>&lt;mark&gt;</code> resalta el <mark>término clave</mark> de la diapositiva</span>

<span class="fragment"><code>&lt;span class="fragment"&gt;</code> hace que el punto aparezca al avanzar</span>

<span class="fragment"><code>Note:</code> al final es la nota del profesor: énfasis, pregunta y truco</span>

<span class="fragment">Las flechas avanzan y retroceden; <code>Esc</code> muestra la vista general</span>

<span class="fragment">El subrayado amarillo es lo que se memoriza; el resto se comprende</span>

Note:
En el examen se pregunta mucho lo que aparece en las notas del profesor, porque ahí indico qué se evalúa de cada concepto y qué es solo ampliación. Los fragmentos os permiten ir despacio: cada tecla revela una idea, así que no leáis la diapositiva entera de golpe. Guardad este hábito desde ya: mark para estudiar, Note para el porqué de las cosas. Si alguien presenta una diapositiva sin Note, seguidamente avisad: es un error de formato.

---

## Estructura de cada unidad

<span class="fragment">Portada con los <strong>objetivos</strong> de aprendizaje de la unidad</span>

<span class="fragment">Conceptos: <strong>una idea por diapositiva</strong> y términos clave marcados</span>

<span class="fragment">Ejemplos de <strong>código comentado</strong> listos para copiar en VS Code</span>

<span class="fragment">Un <strong>diagrama</strong>, un error frecuente y una autoevaluación al cierre</span>

<span class="fragment">Final: <strong>Claves para el examen</strong>, lo mínimo que hay que recordar</span>

<span class="fragment">Repetir patrón: al tercero ya sabéis dónde mirar sin que os lo expliquen</span>

Note:
Todas las unidades siguen la misma plantilla para que podáis estudiar con un método fijo: objetivos, conceptos, código, error común y claves. Cuando conocéis el patrón, el repaso antes del examen se convierte en recorrer las diapositivas tituladas «Claves» y «Error común» en veinte minutos. Os recomiendo subrayar en papel lo que no os suene de cada unidad y volver solo a eso la noche anterior a la prueba. Ese subrayado, sumado a las autoevaluaciones, es lo que os hará falta el día de la prueba.

---

## Requisitos previos

<div style="font-size: 1em; text-align: left;">

Antes de arrancar conviene dominar tres cosas, y ninguna es difícil:
</div>

<span class="fragment">Usar <strong>VS Code</strong> y guardar los archivos con la extensión <code>.html</code></span>

<span class="fragment">Mover rutas relativas dentro de una carpeta: <code>./</code> y <code>../</code></span>

<span class="fragment">Idea general de qué hace un navegador al abrir una URL</span>

<span class="fragment">No hace falta CSS previo: el bloque de CSS empieza desde cero</span>

<span class="fragment">Tampoco hace falta saber programar: HTML no tiene variables ni bucles</span>

Note:
Si domináis los tres primeros puntos vais sobrado; el resto se afina en la primera sesión y con el primer ejercicio. Recordad el recorrido del navegador: pide el archivo, lo analiza, construye el árbol DOM y lo pinta; esa imagen mental explica casi todos los errores de la unidad 1. Pregunta al grupo: ¿qué diferencia hay entre lo que escribe el navegador en la barra de direcciones y lo que veis en pantalla? La respuesta os sorprenderá: no siempre es el archivo que guardasteis.

---

## Herramientas y recursos

<span class="fragment"><strong>VS Code</strong> con previsualización en vivo y un navegador con <code>F12</code></span>

<span class="fragment">Validador del W3C: <code>validator.w3.org</code> antes de entregar cualquier práctica</span>

<span class="fragment"><strong>MDN Web Docs</strong> como referencia oficial de cada etiqueta</span>

<span class="fragment">Los apuntes completos en <code>docs/</code> y los ejercicios con sus soluciones</span>

<span class="fragment">Guardad siempre en <strong>UTF-8</strong>: Archivo → Guardar con codificación</span>

<span class="fragment">Annadid Live Server si queréis que la página se recargue sola al guardar</span>

Note:
El validador es vuestra primera línea de defensa: detecta etiquetas sin cerrar, lang ausente o id duplicados en segundos y os ahorra discusiones con el profesor. MDN es la fuente que se cita en los exámenes prácticos: si dudáis de un atributo, se consulta ahí y no en foros de dudosa fiabilidad. Y el error más frecuente de los primeros días es de codificación: UTF-8, siempre UTF-8, o veréis signos raros que no tienen nada que ver con vuestro código. Guardad este enlace en marcadores: lo vais a usar cada semana.

---

## Autoevaluación inicial

Antes de entrar en materia, comprobemos lo básico del curso:

<span class="fragment">¿Qué lenguaje describe <strong>cómo se ve</strong> una página: HTML o CSS?</span>

<span class="fragment">Respuesta: <strong>CSS</strong>; HTML describe qué hay y el aspecto va en otro fichero</span>

<span class="fragment">¿Se puede escribir HTML en mayúsculas? ¿Y conviene hacerlo?</span>

<span class="fragment">Se puede, pero <strong>no conviene</strong>: se escribe en minúsculas por convención</span>

<span class="fragment">¿Cuántas unidades de CSS y cuántas de HTML tiene este material?</span>

<span class="fragment"><strong>16 de CSS</strong> (de la 00 a la 15) y <strong>10 de HTML</strong></span>

Note:
Estas tres preguntas son el termómetro de la sesión: si las falláis, no pasa nada, pero señalan por dónde hay que empezar. La primera es la que más se confunde fuera del aula, donde todo se llama «HTML5» por costumbre. La segunda aparece literalmente en el examen teórico de la unidad 1. La tercera sirve para que sepáis cuánto material os queda y en qué orden se va a impartir.

---

## Error común: mezclar las capas

⚠ <span class="fragment">Guardar en <code>.txt</code> o ANSI en lugar de <code>.html</code> en UTF-8</span>

⚠ <span class="fragment">Escribir etiquetas en mayúsculas: rompe la convención</span>

⚠ <span class="fragment">Mezclar capas: colores dentro del HTML o texto en el CSS</span>

⚠ <span class="fragment">Rutas absolutas de vuestro equipo en vez de relativas</span>

⚠ <span class="fragment">Copiar código sin leerlo: no aprenderéis a depurarlo</span>

Note:
Los tres primeros son los que más se repiten la primera semana y todos se detectan en cuanto se abre el archivo en el navegador. El cuarto funciona en vuestro equipo y se rompe en cuanto se sube a un servidor, que es justo cuando más cuesta diagnosticarlo. El último no es un error de sintaxis, pero es el que de verdad impide aprender: leed cada línea antes de pegarla. Si detectáis alguno de estos cinco en una entrega, se corrige en clase sin penalización.

---

## Claves para el examen

- HTML dice **qué hay**, CSS **cómo se ve**, JS **qué hace**

- HTML5 es el estándar; **no existe CSS3** como especificación

- Módulos: **0373** (LMH) · **0615** (DIW) · **0488** (DI)

- Formato: **mark** = clave · **fragment** = revela · **Note** = nota

- Mapa: **10 unidades HTML5** y **16 de CSS**, en este orden

- Validad en **validator.w3.org** y guardad en **UTF-8**

Note:
Estas seis líneas resumen la presentación del curso. La primera es la que más se olvida en el primer examen: confundir la capa de estructura con la de estilo invalida ejercicios enteros. La cuarta no es contenido técnico, pero determina cómo estudiáis el resto del curso: si ignoráis las notas del profesor, os dejáis la mitad del temario. Repasad el mapa de unidades también, porque en la práctica se os pedirá localizar material concreto.

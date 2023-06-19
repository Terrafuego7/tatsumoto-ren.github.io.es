---
title: Discución sobre las distintas plantillas de tarjetas
date: 1610646660
tags: [anki]
---

<p align="center"><img alt="flashcards" class="shadow" src="img/bluepilled-flashcards.webp"></p>

Muchos estudiantes coinciden en que la forma más efectiva de adquirir el japonés
es combinar el repaso espaciado (RE) con la inmersión.
Después de terminar de aprender
los [kana](learning-kana-in-two-days.html) y los [kanji](jp1k-anki-deck.html),
seguirás utilizando Anki
en tu tiempo de estudio para memorizar vocabulario.
Al memorizar nuevo vocabulario, existen diferentes plantillas de tarjetas entre las que puedes elegir.

Las plantillas de tarjetas se diferencian por lo que se coloca en el frente de la tarjeta.
Hay dos plantillas principales que la gente tiende a usar: las `tarjetas de oraciones` y las `tarjetas de palabras`.
Ambas tienen sus variaciones dependiendo de la información adicional que contengan.

Este artículo cubre las tarjetas de **reconocimiento**.
Las tarjetas de producción se tratan en [este enlace](writing-japanese.html).

****

## Cómo se crean las tarjetas

En Anki, el usuario crea *notas* que almacenan la información que desea recordar.
Una nota se divide en campos, y cada campo puede almacenar texto.
La nota más simple tiene solo dos campos, "Pregunta" y "Respuesta", o "Frente" y "Dorso".
Anki genera *tarjetas* a partir de las notas que el usuario ha creado utilizando *plantillas de tarjeta*.
Una *plantilla de tarjeta*, o *tipo de tarjeta*, es una plantilla HTML y CSS que define cómo se verá una tarjeta.
Puedes tener varias tarjetas por nota, dependiendo de las plantillas de tarjeta que hayas creado.
Por ejemplo, cada elemento de oración
tendría una tarjeta para evaluar la lectura y otra tarjeta para evaluar la escritura a mano.

## Los varios tipos de plantillas de tarjetas

La división de las plantillas de tarjetas es arbitraria.
La incluimos porque, desde la perspectiva del aprendizaje de idiomas,
es importante en qué nos evaluamos a nosotros mismos.
Aquí, una plantilla de tarjeta se caracteriza por el campo de la nota
que se coloca en el frente.
Los campos en el dorso de la tarjeta son menos significativos.
Su propósito es ayudar a aumentar tu comprensión de lo que está en el frente.

* **Tarjetas de Palabras** evalúan tu comprensión de lectura de una sola palabra.
  * **[Tarjetas de Palabras Simples](#tarjetas-de-palabras-simples)** contienen la información mínima necesaria para entender la palabra.
  * **[Tarjetas de Contexto de Palabras](#tarjetas-de-contexto-de-palabras)** deben tener adicionalmente una oración de ejemplo en el dorso de la tarjeta.
* **[Tarjetas de Oraciones](#tarjetas-de-oraciones)** evalúan tu comprensión de lectura de una oración o parte de una oración.
* **[Tarjetas de Oraciones Objetivo](#tarjetas-de-oraciones-objetivo)** evalúan tu comprensión de lectura de una sola palabra en contexto.
* Otros tipos de tarjetas se utilizan raramente, incluyendo tarjetas con audio en el frente.

Abordamos las plantillas de tarjetas con base en la idea de que
tu práctica en Anki debería imitar situaciones del mundo real.
En otras palabras, debes *practicar de la manera en que se hará en la vida real*.
Y en el mundo real leemos oraciones y escribimos oraciones.
Por lo tanto, se da preferencia a los formatos de tarjetas que contienen oraciones.
Dicho esto, las tarjetas de palabras tienen su lugar en tu RE.
Son muy efectivas para estudiar sustantivos concretos.

Independientemente de la plantilla de tarjeta,
creas tus tarjetas a partir de palabras y oraciones que encuentras mientras consumes japonés.
Los estudiantes utilizan
[GoldenDict](setting-up-goldendict.html)
[Qolibri](setting-up-qolibri.html),
[scripts de mpv](mining-from-movies-and-tv-shows.html#user-scripts-for-mpv),
[Yomichan](setting-up-yomichan.html),
y [otros programas](resources.html#dictionaries)
para agilizar y facilitar la creación de tarjetas.

## Tarjetas de palabras simples

Por tarjetas de palabras simples me refiero a una palabra en el idioma objetivo en el frente de la tarjeta
y una definición y, por lo general, audio e imagen en el dorso.
En este tipo de tarjetas no se presenta contexto.

<p align="center"><img alt="tarjeta-de-palabra" class="shadow" src="img/example-word-card.webp"></p>

<p align="center"><i>Una tarjeta de palabra simple.</i></p>

Las TPS son las más fáciles de crear y las más rápidas de revisar.

### Cómo revisar las TPS

1) Lee la palabra objetivo.
2) Recuerda el significado y la lectura de la palabra.

Pasa la tarjeta si comprendes el significado y la lectura de la palabra objetivo.
De lo contrario, elige "Repetir" para revisar la tarjeta nuevamente más pronto.

### Ventajas y desventajas de las TPS

Como se mencionó al principio de este artículo,
las tarjetas de palabras simples son muy efectivas al aprender sustantivos concretos.
Un *sustantivo concreto* es un sustantivo que puedes ver o tocar.
Los sustantivos "teléfono", "perro", "coche" son sustantivos concretos.
Si una palabra no es un sustantivo concreto,
aprenderla a través de una tarjeta de palabra simple no será efectivo.
Por ejemplo, palabras como <span title="ふっかつ ー restaurar, revivir">復活</span>
o <span title="はしる ー correr">走る</span> requieren contexto para entender su significado y uso.
Sin él, es casi seguro que malentenderás el significado
y no sabrás qué construcciones gramaticales se deben usar con la palabra.

Pero debido a que la mayoría de los sustantivos concretos
tienen significados claros,
se usan de manera similar
y están rodeados de patrones gramaticales similares
que se pueden aprender fácilmente a través de la exposición repetida,
en mi opinión, proporcionar contexto es completamente innecesario.
A menudo puedes entender el significado de un sustantivo concreto incluso sin un diccionario.
Para entender qué significa <span title="ねこ ー un gato">猫</span>,
basta con ver una foto de él.

El tiempo ahorrado al usar TPS para sustantivos supera los beneficios de usar tarjetas de oraciones,
porque se pueden agregar muchas más TPS que tarjetas de oraciones,
y se pueden revisar mucho más rápidamente sin pensar en el contexto.
Al simplemente pensar en la lectura y el significado de una palabra, estás haciendo que las TPS requieran muy poco esfuerzo.

Argumentaría que las tarjetas de palabras deberían representar alrededor del 15% de tu número total de tarjetas.

## Tarjetas de contexto de palabras

Las TCP contienen la palabra objetivo en el frente.
El frente de la tarjeta a veces también contiene pistas
que desambiguan ciertos aspectos de la palabra objetivo.

El dorso de la tarjeta contiene todo lo que necesitas para entender la palabra objetivo:

* Lecturas y acentos de tono
* Oración de ejemplo
* Definiciones
* Audio
* y demás.

<p align="center"><img alt="ejemplo-tcp" class="shadow" src="img/example-word-context-card.webp"></p>

<p align="center"><i>Una tarjeta de contexto de palabra.</i></p>

### Cómo revisar las tarjetas de contexto de palabras

Las TCP evalúan tu comprensión de lectura de una sola palabra.
De manera similar a las TP, 
presiona `Bien` solo si entiendes cómo se lee la palabra y qué significa.

La primera vez que aprendes una nueva tarjeta,
lees la oración en el dorso de la tarjeta y escuchas el audio
para entender el uso de la palabra.
Después de eso, cada vez que la tarjeta aparezca para su revisión,
verás la palabra aislada en el frente,
recordarás el significado,
y si puedes recordar bien el significado,
pasarás a la siguiente tarjeta
sin escuchar el audio
ni leer la oración en el dorso.

Cuando usas esta plantilla de tarjeta, puedes revisar muy rápidamente
porque a menos que olvides la palabra,
no necesitas la oración,
y no te obligas a leerla.
Simplemente puedes omitir la oración y pasar a la siguiente tarjeta.

### Ventajas y desventajas de las TCP

Al igual que las TP, las TCP deberían funcionar muy bien para sustantivos concretos.
Si te encuentras con un sustantivo concreto en contexto,
crear una TCP sería una elección natural.
Las desventajas se presentan al aprender otros tipos de palabras.

Las TCP llevan más tiempo crearlas que las TP.
Se necesita tiempo adicional para agregar el contexto (oración, imagen, audio) a la tarjeta.
Sin embargo, existen herramientas que pueden automatizar este proceso.
Por ejemplo, scripts de mpv.

Las TCP deberían ser tan rápidas de revisar como las TP.
Lo único que necesitas hacer es recordar qué significa la palabra objetivo.
Para palabras que no sean sustantivos concretos, las TCP podrían llevar más tiempo recordar el significado.
Si la palabra es abstracta,
puede ser difícil saber si entiendes el significado o no
sin contexto en el frente.

Las TCP eliminan la información de contexto del frente de la tarjeta,
obligándote a recordar el significado y la lectura sin importar el contexto.
Esto hace que las tarjetas sean más difíciles de aprender y revisar.

* Debido a que las palabras que no son sustantivos concretos rara vez se ven aisladas,
  esta práctica es poco natural.
* Debido a que el conocimiento en el que te estás evaluando es tan pequeño,
  es difícil asociar directamente la palabra con su significado.
* Dedicas más tiempo y esfuerzo a recordar el significado
  en comparación con una tarjeta con contexto en el frente.
  Es más fácil leer una oración de ejemplo y comprender la palabra en una oración.
* Si puedes recordar el significado de una palabra aislada,
eso no significa necesariamente que cuando leas la palabra en una oración
vas a entender la oración.

Debido a que falta el contexto en el frente,
a menudo es necesario confiar en un campo adicional
que sirve para reducir la interferencia de la memoria: el campo de pista.
El campo de pista es necesario cuando una palabra tiene múltiples significados.
Para esa palabra, no puedes recordar el significado correcto sin mirar un ejemplo.
Una TCP con contexto en el frente, en esencia, se convierte en un tipo de tarjeta de oración.
En este caso, definitivamente elegiría crear una tarjeta de oración específica en su lugar.

Si decides usarlas, las Tarjetas de Contexto de Palabras, al igual que las Tarjetas de Palabras Simples, pueden ser útiles,
pero no recomendaría usarlas como tu plantilla principal de tarjeta.

## Tarjetas de oraciones

Una [tarjeta de oración](http://www.antimoon.com/how/usingsm-makeitems-sentence.htm)
es una tarjeta de RE con una oración en el campo de pregunta.
La oración tiene **una** palabra o frase desconocida.

Algunas personas podrían hacer tarjetas con múltiples elementos desconocidos,
pero esto conlleva repasos más difíciles.
Si tienes una tarjeta de oración que evalúa dos (o más) palabras al mismo tiempo,
necesitarás hacer repasos
que sean lo suficientemente frecuentes para mantener la palabra más difícil en la memoria.

En el dorso encontrarás lecturas y definiciones de diccionario.
Idealmente, también querrás agregar audio para toda la oración y/o la palabra objetivo,
información sobre el acento tonal
y una imagen si la oración proviene de un video.

<p align="center"><img alt="ejemplo-tarjeta-de-oracion" class="shadow" src="img/example-sentence-card.webp"></p>

<p align="center"><i>Una tarjeta de oración.</i></p>

### Cómo revisar las tarjetas de oraciones

El algoritmo se explica en el [sitio de AJATT](https://web.archive.org/web/20081122063325/http://www.alljapaneseallthetime.com/blog/10000-sentences-how/).
Lo simplifiqué un poco, a continuación están los pasos principales:

1) Lees la oración completa.
2) Conoces el significado de cada palabra en la oración.
3) Comprendes el significado de la oración completa.

Si se cumplen los requisitos anteriores, presiona `Bien`.
De lo contrario, elige `Repetir` para ver la tarjeta más pronto.

Hay otros pasos y matices descritos en el sitio de AJATT,
pero la mayoría de los usuarios de tarjetas de oraciones los omiten.
En particular, no creo que muchas personas lean las oraciones en voz alta
o las copien a mano en un papel.
Estas acciones no son útiles y solo alargan los repasos.

### Ventajas y desventajas de las tarjetas de oraciones

La primera ventaja de las tarjetas de oraciones es que son fáciles de recordar.
Tienes una oración completa como contexto que se muestra.
El contexto ayuda a tu cerebro a recordar lo que significa la palabra objetivo.
Si solo tienes una palabra en el frente,
especialmente si es una palabra con un significado más abstracto,
puede ser difícil saber si entiendes el significado o no.

Las tarjetas de oraciones son naturales y orgánicas.
Lo que quiero decir con esto es que
la práctica de leer oraciones se parece mucho a situaciones del mundo real.
Es más similar a lo que haces en la vida real al leer un libro.
La palabra objetivo está integrada en un contexto que ayuda a que el significado de la palabra sea claro.

Pero tienen ciertas debilidades, siendo la principal el **tiempo de repaso**.
En una tarjeta de oración, la palabra objetivo no se enfatiza de ninguna manera.
Como resultado, en cada repetición tienes que leer toda la oración
y básicamente evaluarte a ti mismo en cada palabra de la misma.
En promedio, se tarda 20 segundos en responder una tarjeta de oración.
Esto es mucho tiempo en comparación con leer y recordar solo la palabra objetivo.
Afortunadamente, existen algunos trucos para hacer repasos más rápidos, que se describen en la sección de TOO.

Las tarjetas de oraciones reciben muchas críticas
porque pueden crear memorias dependientes del contexto.
Si siempre recuerdas el significado de una palabra
cuando esa palabra está contenida dentro de una determinada oración,
a veces terminas memorizando esa oración en lugar de la palabra objetivo.
Luego, cuando ves esa palabra objetivo fuera de contexto o en un contexto diferente,
no puedes establecer la conexión y recordar qué significa la palabra
o incluso darte cuenta de que aprendiste esa palabra.
En menor medida, esto también ocurre con las tarjetas de palabras
porque no tener contexto es un tipo de contexto en sí mismo.
Cuando ves la palabra en inmersión,
es posible que no puedas establecer la conexión y recordarla.
Es probable que se puedan formar memorias dependientes del contexto al usar cualquier tipo de plantilla de tarjeta.
Para combatir las memorias dependientes del contexto, la inmersión es clave.
El conocimiento de una palabra se internaliza
después de verla varias veces en diferentes contextos en la vida real.

A veces se dice que al revisar oraciones
construirás la gramática interna y recordarás el uso de las palabras,
lo cual es útil para tu producción.
Creo que esto proviene de una falta de comprensión del sitio de AJATT.
Hay una suposición subyacente de que
el RE se puede utilizar para aprender a producir.
En realidad, el papel del RE es ayudar a la comprensión
ayudándote a memorizar los significados y las lecturas de las palabras.
La producción solo puede surgir de una exposición abundante y ver palabras en diferentes contextos.
La lectura de oraciones en el RE solo puede desempeñar un papel menor.

No obstante, hay algo de verdad en esta afirmación.
Aunque según Wozniak, el reconocimiento pasivo no garantiza el recuerdo activo,
leer varias veces la misma pieza tiene un efecto similar al de los comerciales de televisión.
A veces puedes recitarlos de memoria solo por la exposición repetida.
Puedes esperar memorizar muchas oraciones de esta manera,
pero casi seguramente no las memorizarás todas.
Debo señalar que es simplemente un efecto secundario
y no debe considerarse una ventaja del uso de tarjetas de oraciones.

## Tarjetas de oraciones objetivo

Las TOO son similares a las [tarjetas de oraciones](#tarjetas-de-oraciones),
pero siempre te aseguras de resaltar la palabra objetivo.
Esto se hace seleccionando la palabra y presionando <kbd>Ctrl</kbd>+<kbd>B</kbd> en Anki, fácil y sencillo.
Yomichan también puede hacerlo si se ajusta su configuración de cierta manera.

<p align="center"><img alt="ejemplo-tarjeta-de-oracion-objetivo" class="shadow" src="img/example-mpvacious-card.webp"></p>

<p align="center"><i>Una tarjeta de oración específica.</i></p>

Las TOO son muy flexibles y brindan a los usuarios muchas opciones para revisarlas.
Dependiendo de tus preferencias, puedes:

* Repasarlas como tarjetas de oraciones regulares.
  Lees la oración completa
  y decides si entendiste todas las partes.
* Leer toda la oración, pero evaluarte solo en la palabra objetivo.
  Esto tiene el efecto positivo de aliviar la carga mental de evaluarte
  en demasiadas cosas al mismo tiempo.
* Leer solo la palabra objetivo y, probablemente, unas pocas palabras que la rodean.
  Esta forma de revisar las TOO se asemeja a las TCO y las TPS y puede ahorrar mucho tiempo de repaso.
  Si una oración es demasiado larga,
  generalmente comienzo a leer unas pocas palabras detrás de la palabra objetivo
  y paro tan pronto como entiendo la oración.
  Evalúate solo en la palabra objetivo, no te penalices si fallas en otras palabras.

Cuando aprendas una oración por primera vez,
asegúrate de leerla y entenderla por completo,
incluso si no quieres leerla cada vez que aparezca la tarjeta.
Entender el contexto ayuda mucho a comprender la palabra objetivo.

También es importante que ya conozcas todas las palabras además de la palabra objetivo.
No quieres encontrarte con palabras que no has aprendido cada vez que repases la tarjeta.
Este concepto se llama "oraciones con un objetivo" y se discute más adelante en este sitio,
en los artículos sobre cómo crear tus propias tarjetas.

Sigue [este enlace](setting-up-anki.html#import-an-example-mining-deck) para descargar
un mazo con ejemplos de Tarjetas de Oraciones Objetivo.

### Haz que Yomichan resalte la palabra objetivo por ti

Recomiendo configurar Yomichan para que marque automáticamente la palabra objetivo cuando se crea una nueva tarjeta.
Esto te ahorra el paso adicional
que tendrías que realizar cada vez que creas una nueva tarjeta de oración específica.
[mpvacious](https://github.com/Ajatt-Tools/mpvacious)
es consciente de esta configuración y conserva las palabras resaltadas al actualizar las oraciones.

Ve a Configuración de Yomichan > "Anki" > "Configurar formato de tarjeta de Anki...".

<p align="center"><img alt="resaltar-palabra-objetivo" class="shadow" src="img/highlight-target-word.png"></p>

<p align="center"><i>Configuración de Yomichan.</i></p>

**Nota:** Todas las configuraciones de Yomichan se explican en detalle en [Configuración de Yomichan](setting-up-yomichan.html#anki-settings) más adelante.

### ¿Por qué las TOO?

* **Las TOO son libres de estrés.**
  Debido a que no tienes que leer la oración completa en cada tarjeta,
  puedes repasar las TOO mucho más rápido.
  Pero al mismo tiempo, siempre tienes acceso a la oración completa en el frente,
  por lo que puedes leerla si quieres,
  o saltar la lectura si no tienes tiempo para dedicar a tus repasos.
  Libérate rápidamente y vuelve a las cosas divertidas.
* **Las TOO son fáciles de hacer.**
  Puedes usar scripts de mpv como [mpvacious](https://github.com/Ajatt-Tools/mpvacious)
  para crear cada tarjeta en solo unos segundos.
  Cuando estás leyendo una novela, solo Yomichan puede encargarse de todo.
* **El contexto siempre está presente.**
  No te privas de la oración completa, lo que facilita tus repasos.
* **Ves cómo se utiliza la palabra.**
  Debido a que las palabras rara vez se encuentran fuera de las oraciones,
  te aseguras de que tu práctica en Anki se asemeje estrechamente a la lectura en la vida real.
  Incluso si te evalúas solo en la palabra objetivo,
  la información en la tarjeta debería ayudarte a comprender su uso.
* **Elimina la fatiga.**
  No tienes que evaluarte en cada palabra.
  Si crees que las tarjetas de oraciones te evalúan en demasiados elementos al mismo tiempo,
  lo que te agota mentalmente,
  entonces evalúate solo en la palabra objetivo.
  Las TOO te dan libertad de elección.
* **Las TOO son amigables para los principiantes.**
  Cuando recién comencé a aprender elementos de oraciones,
  la capacidad de evaluarme solo en la palabra objetivo me ahorró muchos dolores de cabeza
  porque no tenía que recordar los significados y las lecturas de todas las demás palabras en una oración
  que aún conocía mal o que aún no conocía en absoluto.
* **Ahorra decisiones al crear tarjetas.**
  No necesitas elegir entre varias plantillas de tarjetas porque las TOO
  fusionan las *tarjetas de palabras* y las *tarjetas de oraciones* de una manera única.
* **Cualquier longitud funciona.**
  Las TOO te liberan de la necesidad de extraer oraciones más cortas.
  A menudo, las oraciones cortas carecen de suficiente contexto.
  Los usuarios de tarjetas de oraciones deben buscar oraciones más cortas para acortar los repasos.
  No tienes que mantener las cosas cortas solo para hacer repasos más rápidos.
  Al mismo tiempo, las oraciones largas no te abrumarán porque no estás obligado a leerlas.
* **Mantén el enfoque.**
  Debido al formato de la plantilla de tarjeta y la combinación de los campos de la nota,
  las TOO siempre tienen solo una palabra objetivo por tarjeta,
  pero pueden contener más de una palabra desconocida en total.
  Agregar solo oraciones con un objetivo al RE es una buena práctica,
  garantiza que todas las tarjetas en la colección tengan dificultades intrínsecas similares,
  lo que facilita los repasos.
  Por otro lado,
  si tienes que hacer una TOO con muchas palabras desconocidas,
  no se convierte en una carga
  —al evaluarte, omites todo excepto el objetivo principal.
* **Conserva tus tarjetas.**
  Existe una idea en la comunidad de que las tarjetas deben eliminarse o suspenderse
  después de alcanzar un cierto intervalo.
  La idea se justifica por la suposición de que la inmersión por sí sola es suficiente
  para mantener cualquier palabra en la memoria después de haberla adquirido.
  Creo que es solo una forma de lidiar con el hecho de que las tarjetas de oraciones retardan una eternidad el terminar los repasos diarios.
  Si eres usuario de TOO, tus repasos son rápidos,
  así que no te deshagas de todas tus tarjetas antiguas.

### ¿Las TOO son demasiado fáciles?

Dado que las TOO te permiten ver el contexto, son más fáciles que las tarjetas de palabras, pero eso es algo bueno.

Por el contrario, al repasar palabras de forma aislada, básicamente te creas dificultades innecesarias. También vas en contra del principio de  *practica de la manera en que se hará en la vida real* al evaluarte en algo que rara vez se ve en la vida real.

> Pero, ¿qué pasa si memorizo el significado de la oración en su conjunto y luego no soy capaz de reconocer o entender la palabra objetivo en otros contextos?

En primer lugar, no podrás leer muy bien en absoluto hasta que realmente practiques la lectura y le dediques tiempo. El RE solo puede ayudar un poco. En segundo lugar, eso no ocurre con frecuencia. Sí, a veces formarás memorias dependientes del contexto. Para adquirir completamente una palabra y transferir el conocimiento de depender del contexto a ser independiente del contexto, tienes que verla varias veces en la vida real. La mayoría de las veces eso ocurre rápidamente.

La realidad es que el RE no garantiza que recuerdes una palabra al 100% de todos modos. Podrías hacer una **tarjeta de palabras** para ella y luego no poder recordarla en el momento adecuado debido a un defecto en el algoritmo o porque la memoria de la palabra todavía depende del contexto. Esto incluso puede ocurrir con las tarjetas que aciertas siempre en el RE.

Afortunadamente, la mayoría de las palabras según Krashen se encuentran en **contextos amigables**. En realidad, es menos probable que no puedas entender el significado de una palabra cuando lees contenido en japonés, así que no te preocupes por no poder recordar lo que has aprendido en el RE.

Por último, el mayor problema al aprender a leer en japonés es recordar las lecturas de los kanjis. Para la mayoría de las personas, los intentos fallidos de recordar las lecturas constituyen la mayoría de las fallas en Anki, pero los significados a menudo se obtienen de forma gratuita gracias a los contextos amigables y las **pistas semánticas** que proporcionan los kanjis.

### Mejoras en el rendimiento

En cuanto al tiempo, puedes esperar las siguientes mejoras:

- Cuando leas la oración completa, puedes repasar las TOO hasta 2 veces más rápido en comparación con las tarjetas de oraciones. Esto se logra utilizando el complemento de Anki llamado [Speed Focus Mode](useful-anki-add-ons-for-japanese.html#speed-focus-mode). Incluso puedes evaluar tu conocimiento solo en la palabra objetivo para acelerar aún más las revisiones.
- Cuando repasas las TOO leyendo únicamente la palabra objetivo, puedes hacerlo hasta 4 veces más rápido en comparación con las tarjetas de oraciones. Esto se logra simplemente omitiendo todo excepto la palabra objetivo. Aún escucharás el audio de la oración (si está disponible) o leerás la oración una vez que se revele el reverso de la tarjeta, pero es totalmente opcional.

Durante muchos años estudié con tarjetas de oraciones. Aunque obtuve buenos resultados, invertía mucho tiempo que no era óptimo. Una vez que has visto una tarjeta suficientes veces, no necesitas seguir leyendo la oración completa cada vez que aparece. Puedes saltar a la palabra objetivo si así lo deseas. Sin embargo, con las tarjetas de oraciones regulares, **no sabes cuál es la palabra objetivo hasta que reveles la respuesta**. Con las TOO, resaltas la palabra objetivo cuando creas la tarjeta. Luego, cuando la tarjeta se muestra para repasar, siempre tienes la opción de leer solo la palabra objetivo.

Ten en cuenta que cualquier tiempo que dediques al RE es tiempo que no puedes dedicar a la inmersión. Por lo tanto, el propósito de estos consejos es reducir el tiempo invertido en las revisiones y aprovechar la carga mental del RE. Al aplicarlos, reducirás ligeramente los beneficios de las tarjetas de oraciones, pero creo que en última instancia cualquier técnica que te ayude a mantener el ritmo es un buen equilibrio. Si mantienes una relación poco saludable con el RE, es fácil comenzar a odiarlo y dejarlo por completo, lo cual es el peor resultado en comparación con olvidar algunas palabras de vez en cuando.

Puedes repasar las TOO rápidamente y puedes aprender más tarjetas en la misma cantidad de tiempo o simplemente aprender la misma cantidad de tarjetas en menos tiempo y luego tener más tiempo para la inmersión.

También es importante tener en cuenta que el RE te ayuda a mantener entradas de diccionario mental para las palabras que incluyes. Incluso si no recuerdas el significado exacto de una palabra, tener una entrada de diccionario mental permite que tu cerebro la note más fácilmente en la inmersión y almacene cualquier información nueva sobre esa palabra.

### ¿Puede el campo de pista salvar el día?

Los usuarios de las TCP emplean un campo de "pista" para desambiguar las lecturas correctas y señalar uno de los posibles significados en algunas palabras. No creo que sea una buena idea. La necesidad de crear un campo separado está lejos de ser la mejor solución y parece ser un apoyo. Primero, cada vez que revises una tarjeta, debes identificar que no puedes comprender el significado sin una pista. Luego, debes copiar una parte de la oración al campo de pista. Finalmente, cuando revises la tarjeta, debes leer la palabra objetivo y luego saltar a la pista y leerla también.

Debido a que las TOO colocan las oraciones en primer lugar, se te brindan todas las herramientas para desambiguar tanto las lecturas de los kanji como los múltiples significados de forma gratuita, y no necesitas inventar nada. Leer frases es más fácil que leer palabras separadas con algo de texto al final, y se asemeja más a la forma en que leemos libros reales.

#### Distinguiendo significados

Algunas palabras solo aparecen en ciertas expresiones. Algunas pueden tener múltiples significados. La buena noticia es que no tienes que preocuparte por ello al revisar las TOO. El contexto en el frente te ayuda a identificar el significado correcto. También puedes crear una segunda tarjeta para otro significado si lo deseas.

<p align="center"><img alt="hint-field-replacement" class="shadow" src="img/hint-field-replacement.png"></p>

<p align="center"><i>Las TOO ofrecen una alternativa natural al campo de pista.</i></p>

> ¿Qué pasa si una expresión no tiene una entrada en un diccionario japonés-japonés?

Seguramente la tiene. Si no la encuentras en un diccionario de Yomichan, búscala en [www.weblio.jp](https://www.weblio.jp/) o utiliza la búsqueda en la web. Por ejemplo, [aquí](https://www.weblio.jp/content/%E9%A0%AD%E8%A7%92%28%E3%81%A8%E3%81%86%E3%81%8B%E3%81%8F%29%E3%82%92%E7%8F%BE%28%E3%81%82%E3%82%89%E3%82%8F%29%E3%83%BB%E3%81%99) puedes encontrar una definición para 「頭角を現す」.

> ¿Y si no tiene audio en Yomichan?

No es un gran problema, pero puedes intentar buscarlo en [Forvo](https://forvo.com/word/%E9%A0%AD%E8%A7%92%E3%82%92%E7%8F%BE%E3%81%99/#ja). Si has agregado audio para la oración, no es necesario añadir audio para la expresión objetivo.

#### Distinguiendo lecturas

Si una palabra tiene muchas lecturas, hay dos palabras que se escriben con los mismos kanji pero se pronuncian de manera diferente, o si quieres evitar fracasar en una tarjeta debido a un error común de lectura que tiendes a cometer, las TOO te permiten usar furigana en la parte superior para señalar la correcta.

Asegúrate de que tu plantilla del frente permita mostrar el furigana:
```
{{furigana:SentKanji}}
```
Y para agregar el furigana en el frente, simplemente lo especificas entre corchetes como de costumbre:
```
稀に日蝕の 最中[×さいちゅう]に姿を消す者がある
```
<p align="center"><img alt="reading-1" class="shadow" src="img/doukatsu.png"></p>

<p align="center"><i>Una forma de evitar repetir el mismo error.</i></p>

<p align="center"><img alt="reading-2" class="shadow" src="img/sanaka.png"></p>

<p align="center"><i>Señala la lectura correcta.</i></p>

### Las tarjetas de respaldo

La idea detrás de las tarjetas de respaldo es similar a la de las tarjetas de oraciones objetivo, pero el frente es diferente. Cuando una tarjeta de respaldo aparece para su revisión, se ve como una **tarjeta de palabra** común, pero puedes pasar el cursor sobre la palabra objetivo para revelar la oración completa. Las tarjetas de respaldo básicamente ofrecen a los usuarios todos los beneficios de las tarjetas de oraciones objetivo, pero están diseñadas para personas que se preocupan por formar memorias dependientes del contexto.

<p align="center"><img alt="tarjeta de respaldo" class="shadow" src="img/fallback_card.webp"></p>
<p align="center"><i>Frente de una tarjeta de respaldo.</i></p>

Una desventaja es que esta plantilla de tarjeta es algo complicada de hacer por tu cuenta. Tendrás que jugar con el CSS y HTML de tus tarjetas para hacer que aparezca el contexto al pasar el cursor sobre la palabra.

Un usuario de DJT compartió su plantilla de tarjeta en [Pastebin](https://pastebin.com/pAVvqLPd), échale un vistazo si necesitas ayuda para configurar las tarjetas de respaldo. La plantilla configura la tecla **Shift** para alternar la visibilidad de la oración, es posible que desees instalar la extensión de Anki [Refocus Card when Reviewing](https://ankiweb.net/shared/info/1642550423) para poder utilizarla.

Desde [aquí](https://github.com/Ajatt-Tools/AnkiNoteTypes/tree/main/templates/Japanese%20fallback) puedes descargar el Japanese fallback Note Type (Tipo de Nota de Respaldo Japonés) creado por ﾌｪﾘﾍﾟ.

### Conclusión

La falta de contexto hace que las tarjetas de palabras sean más difíciles de aprender, pero se revisan rápidamente y son efectivas para los sustantivos concretos.

Las tarjetas de oraciones requieren más tiempo para que completes tus revisiones diarias, pero debido a que la palabra objetivo tiene contexto, aclara el significado y el uso de la palabra.

Las tarjetas de oraciones objetivo combinan la rapidez de las tarjetas de palabras con la efectividad del aprendizaje en contexto de las tarjetas de oraciones, lo que las convierte en la mejor plantilla de tarjeta.

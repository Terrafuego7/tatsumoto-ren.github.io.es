---
title: Configuración de Anki
date: 1609127492
tags: [anki]
---

<img alt="anki logo" src="img/anki_logo.webp" float="right">

[Anki](https://wiki.archlinux.org/index.php/Anki) es un sistema de [repaso espaciado](https://es.wikipedia.org/wiki/Repaso_espaciado) (RE) que te permite crear, gestionar y repasar [tarjetas de estudio](https://es.wikipedia.org/wiki/Tarjeta_de_aprendizaje).

Muchos estudiantes de idiomas encuentran útil Anki para memorizar rápidamente el vocabulario básico del idioma objetivo (IO), así como para ayudarles a recordar nuevo material más adelante.

Uno de los inconvenientes de Anki es que puede ser *un poco* difícil de aprender a usar. Dependiendo de cómo lo utilices, puedes reducir considerablemente el tiempo dedicado al estudio o convertir el uso de Anki en un verdadero infierno. Si te sientes confundido acerca de cómo funciona Anki, se recomienda que leas el [manual de Anki](https://docs.ankiweb.net/). Sin embargo, dado que es altamente detallado y técnico, la mayor parte de este artículo se centrará en explicar los ajustes más útiles de Anki para ayudarte a ponerlo en marcha lo más rápido posible.

****

## Instalación

Existen dos formas principales de instalar Anki.

* Utilizando el gestor de paquetes de tu distribución (pacman, apt, dnf, etc.).
* Utilizando pip, un instalador de software para programas de Python.
* Descargando una versión desde el sitio web oficial.

El primer método garantiza que tendrás las dependencias adecuadas instaladas,
pero es posible que obtengas una versión antigua de Anki.
Los mantenedores de las distribuciones no suelen mantener Anki actualizado,
aunque en las distribuciones GNU de lanzamiento continuo esto no se nota tanto.
El segundo método garantiza que obtendrás la última versión,
pero debes asegurarte de tener todas las dependencias instaladas.
Y el tercer método es para sistemas operativos que no tienen gestores de paquetes.

Por favor, no instales Anki mediante **FlatPak**, paquetes Snap u otros gestores de paquetes no nativos.
Se han reportado diversos problemas relacionados con estos métodos de instalación.

Si estás utilizando Wayland, por favor vuelve a [Xorg](https://wiki.archlinux.org/title/xorg)
para evitar posibles problemas.

### Utilizando tu gestor de paquetes

* En Arch Linux y otras distribuciones basadas en pacman, puedes obtener el binario oficial de
  [GitHub](https://github.com/ankitects/anki/releases/)
  instalando
  [anki-official-binary-bundle](https://aur.archlinux.org/packages/anki-official-binary-bundle/)
  desde AUR.

  Anki también está disponible en repositorios de terceros:
  [Chaotic](https://aur.chaotic.cx/) y
  [archlinuxcn](https://github.com/archlinuxcn/repo).
  Estos son repositorios que proporcionan paquetes precompilados de AUR
  para que los usuarios no tengan que compilar esos paquetes ellos mismos.
  Después de habilitar un repositorio de terceros,
  instala Anki con `sudo pacman -S anki` como cualquier otro paquete.
* Si no eres usuario de Arch Linux,
  seguramente encontrarás Anki en los repositorios de tu distribución.
  Para encontrar Anki para tu sistema operativo, puedes utilizar [pkgs.org](https://pkgs.org/search/?q=Anki).
* Los usuarios de Debian y otras distribuciones *estables* deben tener en cuenta que
  las versiones desactualizadas de Anki no funcionan bien con la mayoría de los complementos, especialmente los nuevos.
  Utiliza una versión lanzada hace al menos 6 meses o más reciente.

### Uso de pip

La última versión se puede instalar con el paquete [aqt](https://pypi.org/project/aqt/).

```
$ pip install --upgrade aqt
```

<details>
<summary>Notas</summary>

* `pip` coloca los archivos ejecutables en `~/.local/bin/` de forma predeterminada.
  No olvides agregar este directorio a la
  [ruta](how-do-i-add-a-directory-to-the-path.html).
* Para ejecutar Anki, escribe `anki` en la terminal y presiona Enter.
  Sin embargo, tener una
  [entrada de escritorio](https://wiki.archlinux.org/title/Desktop_entries)
  es más conveniente.
  Descarga
  [este archivo](https://github.com/tatsumoto-ren/dotfiles/blob/main/.local/share/applications/anki.desktop)
  y guárdalo en `~/.local/share/applications`.
* Si después de instalar Anki con `pip`
  [Fcitx](https://wiki.archlinux.org/title/Fcitx)
  no funciona,
  agrega `export QT_PLUGIN_PATH=/usr/lib/qt/plugins`
  a la lista de [variables de entorno](how-do-i-change-an-environment-variable.html).
* Anki depende de [mpv](https://mpv.io/) para reproducir audio.
  Debes instalarlo por separado.
* Es posible que también debas instalar [PyQt5](https://pypi.org/project/PyQt5/).
* Anki `2.1.50` y versiones posteriores requieren adicionalmente la instalación de
  [PyQtWebEngine](https://pypi.org/project/PyQtWebEngine/)
  y
  [PyQt5-stubs](https://pypi.org/project/PyQt5-stubs/)
  desde PyPI.
* `PyQt5` y `PyQtWebEngine` también se pueden obtener de los repositorios oficiales de Arch Linux.

Puedes indicarle a `pip` que instale una versión específica.
Esto es útil cuando la última versión presenta fallas.

```
pip3 install --upgrade --pre "aqt==2.1.49"
```

Hay dos versiones,
dependiendo de la interfaz gráfica que se utilice,
`Qt6` y `Qt5`.
Puedes cambiar la interfaz de la siguiente manera:

```
$ pip install --upgrade 'aqt[qt5]'
$ pip install --upgrade 'aqt[qt6]'
```

Normalmente, esto no es necesario.

</details>

### Desde el sitio web oficial

Si tu sistema operativo cuenta con un gestor de paquetes, como la mayoría de las distribuciones GNU+Linux, no se recomienda instalar directamente desde el sitio web oficial, ya que un gestor de paquetes puede automatizar la descarga, instalación, desinstalación y actualización.

Pero algunos sistemas operativos, especialmente los similares a Windows como [ReactOS](https://reactos.org/), no tienen esta característica.
En este caso, dirígete a [apps.ankiweb.net](https://apps.ankiweb.net/) y lee las instrucciones ahí.

### Solución de problemas

* Si aún no puedes instalar o ejecutar Anki, consulta el [Manual de Anki](https://docs.ankiweb.net/platform/linux/installing.html) y la [guía de Anki Betas](https://betas.ankiweb.net/).
* Algunas personas informan que ven una pantalla en negro al iniciar y que deberías ejecutar Anki con el parámetro sin sandbox: `anki --no-sandbox` para evitarlo.

## Sincroniza tu dispositivo móvil

Al [registrarte](https://ankiweb.net/account/register) en AnkiWeb,
puedes mantener tus tarjetas sincronizadas en varios dispositivos.
También puedes sincronizar entre dispositivos.
Instala [AnkiDroid](https://f-droid.org/en/packages/com.ichi2.anki/)
en tu dispositivo Android y sincroniza tu colección.
Esto te permitirá repasar tus tarjetas cuando estés fuera
y no tengas acceso a tu computadora.
Prefiero descargar la última versión alfa desde
[GitHub](https://github.com/ankidroid/Anki-Android/releases)
porque las versiones de AnkiDroid son lentas.

Para sincronizar tu colección en el escritorio, presiona `Y` o haz clic en "Sincronizar" en la barra de herramientas.

## Importa un mazo de ejemplos de extracción

Después de instalar Anki, necesitas configurar un `Tipo de nota`
para mantener tus tarjetas de memoria formateadas como desees.
Anki viene con algunos Tipos de nota básicos, pero no son adecuados para aprender japonés.

Dado que crear tu propio `Tipo de nota` es un proceso tedioso
que consiste básicamente en agregar los campos que necesitas y copiar y pegar HTML y CSS,
te recomiendo importar un mazo de ejemplos de extracción prehecho.

Puedes encontrar un mazo de ejemplos de extracción de muestra aquí:

* [AnkiWeb](https://ankiweb.net/shared/info/1557722832)
* [Espejo](https://disk.yandex.com/d/BSmZ2mCRgMZHgQ)

## Soporte para el idioma japonés

Presiona "Herramientas" > "Complementos" > "Obtener complementos" para descargar e instalar el complemento
[AJT Japanese](https://ankiweb.net/shared/info/1344485230).
Luego reinicia.
El complemento está incluido con
[Mecab](https://aur.archlinux.org/packages/mecab),
por lo que no necesitas instalar dependencias adicionales.

## Configuraciones de Anki

En Anki puedes aprender idiomas, biología, matemáticas, física, etc.,
y Anki no está optimizado específicamente para ninguno de ellos.

Para optimizar Anki para el aprendizaje de idiomas,
recomiendo las siguientes configuraciones.

## Preferencias

Las preferencias controlan el comportamiento de tu colección de Anki.
Se aplican a todos los mazos.
Puedes acceder a las preferencias yendo a `Herramientas > Preferencias...` en la ventana principal de Anki.

* **Límite de estudio por adelantado.**
  Recomiendo mantener el valor cerca del valor predeterminado de 20 minutos.
  El mío es de `35` minutos.
  Cuando termines tus repasos diarios y las tarjetas nuevas,
  Anki comenzará a ignorar los intervalos de las tarjetas en la cola de aprendizaje `menores` que
  este valor y te mostrará las tarjetas de inmediato.
  Esto es bueno para las tarjetas con intervalos pequeños porque te permite terminar tus repasos
  sin interrupciones y esperar a que tus tarjetas estén listas para ser revisadas.
  Pero si estableces un `Límite de estudio por adelantado` demasiado alto,
  las tarjetas con pasos de aprendizaje más largos se mostrarán demasiado pronto.
  Mantener el valor en el lado más bajo refuerza el tiempo de espera de tus pasos.
  Si estableces esto en `0`, Anki siempre esperará el retraso completo, por lo que tampoco es óptimo.
* **Mostrar tarjetas nuevas antes de los repasos.**
  Siempre quieres terminar tus repasos primero,
  y no quieres que las tarjetas nuevas te retrasen.
  Puedes elegir `Mostrar tarjetas nuevas antes de los repasos`
  si eres constante y te sientes seguro de que nunca tendrás un retraso en las repasos de Anki.
  Mezclarlas es probablemente la peor opción y te confundirá cuando
  aparezca una tarjeta nueva después de una racha de tarjetas maduras.

  **Nota:** Esta opción se ha movido en las versiones más recientes.
* **Planificador de Anki 2021.**
  Este es un
  [nuevo planificador](https://faqs.ankiweb.net/the-2021-scheduler.html)
  que viene con Anki 2.1.45+.
  Si tu versión de Anki no muestra esta opción, ya ha sido habilitada de forma predeterminada.
  De lo contrario, asegúrate de habilitarla.
  El antiguo planificador `V1` tenía errores y era torpe.
  El nuevo soluciona sus problemas.

  Características principales:

  * Puedes tener submazos y revisarlos todos juntos,
    las tarjetas se mezclarán correctamente durante el repaso.
  * Puedes aprender tarjetas nuevas en mazos filtrados.
    Los mazos filtrados ya no reinician los pasos de aprendizaje cuando se reconstruyen o vacían.
* **Modo minimalista.**
  Las versiones más recientes de Anki vienen con una interfaz de usuario absolutamente horrible.
  El modo minimalista se agregó después de una amplia crítica por parte de los usuarios.
* **Estilo: Nativo.**
  Igual que antes.
  Al habilitar los estilos nativos, el usuario puede aplicar su tema [kvantum](#kvantum) preferido
  y desactiva el tema infantil al estilo de Apple que está establecido

## Grupos de opciones

Cada mazo tiene un Grupo de opciones asociado.
Los Grupos de opciones definen configuraciones específicas para cada mazo.
Cada mazo puede tener configuraciones diferentes según su Grupo de opciones.
Las opciones de los sub-mazos anulan las opciones del mazo principal.
Haz clic en `Mazo > Opciones` para acceder a la configuración de Grupos de opciones.
Puedes hacer clic en "Gestionar" para crear Grupos de opciones adicionales.

**Advertencia:** Si estás utilizando Anki 2.1.45+,
se te mostrará un nuevo diálogo de configuración "Grupos de opciones".
Como de costumbre, los desarrolladores de Anki empeoran la aplicación con cada actualización.
El nuevo diseño no coincidirá con las capturas de pantalla mostradas en esta página.
Si deseas acceder a la versión antigua del diálogo,
haz clic en "Opciones del mazo" mientras mantienes presionada la tecla `Shift`.

Considera crear Grupos de opciones separados para *cada tipo de material* que aprendas.
Puedes asignar cada Grupo de opciones a múltiples mazos.
Esto es útil para realizar pequeños ajustes en mazos individuales en función de las tarjetas que contienen.

<details>

<summary>Nuevo menú</summary>

El nuevo menú de configuración de Grupos de opciones
se puede ver en Anki a partir de la versión 2.1.45.
Las opciones se describen más adelante en este artículo.

<p align="center"><img alt="grupos de opciones" src="img/anki-options-groups.webp"></p>
<p align="center"><i>Configuración.</i></p>

</details>

A continuación se muestran las opciones que recomiendo utilizar.

### Tarjetas nuevas

#### Pasos de aprendizaje

Este es el número de veces que debes responder "bien" en la tarjeta antes de que se gradúe.
Recomiendo a los principiantes que sigan los pasos de aprendizaje predeterminados de `1 10`.
Cuando te familiarices más con Anki, puedes agregar tus propios pasos personalizados y experimentar con ellos.
Pero no exageres: demasiados pasos harán que pases demasiado tiempo en Anki sin obtener una retención sustancial.
La opción "aprender por adelantado" configurada en la sección anterior se asegurará de que no se te muestren tarjetas con pasos grandes demasiado pronto.

Puedes experimentar con los llamados micro pasos
si ves que recordar las tarjetas nuevas es más difícil de lo que pensabas.
Esto significa especificar un intervalo en segundos en lugar de minutos.
Para el nuevo menú de configuración, simplemente escribe `30s` para 30 segundos.
Para el menú antiguo, necesitas especificar un decimal de esta manera: `0.5`.

#### Tarjetas nuevas por día

Controla la cantidad de tarjetas que aprendes cada día en general,
aunque siempre puedes aprender más si quieres.
El valor predeterminado de `20` tarjetas es muy razonable y manejable para la mayoría de los usuarios.
Sin embargo, si te sientes abrumado por la cantidad de repasos que debes hacer, puedes reducirlo a unas `10` tarjetas nuevas al día.
También es posible hacer más tarjetas si puedes manejar la carga de repasos,
pero generalmente en la comunidad AJATT se recomienda aprender no más de `30` tarjetas nuevas al día.

Yo mantengo mi configuración en `0`.
Esto se debe a que uso [Learn Now Button](https://ankiweb.net/shared/info/1021636467) para **seleccionar** y aprender tarjetas manualmente de mi Banco de Frases.
Personalmente, me resulta mejor que dejar que Anki decida por mí.

#### Dificultad inicial

Cada tarjeta tiene una propiedad llamada *Factor de dificultad*.
Con el tiempo, el factor de dificultad puede cambiar y causar efectos secundarios negativos.
Establece la Dificultad inicial en `131%` para evitar los efectos secundarios.
Más información al respecto [más adelante](#infierno-de-dificultad).

<p align="center"><img alt="tarjetas nuevas" class="shadow" src="img/options-groups-new-cards.webp"></p>

### Repasos

#### Máximo de repasos al día

Este valor establece un límite arbitrario en la cantidad de repasos que puedes hacer cada día.
Si el límite es bajo, tus tarjetas pendientes no desaparecerán mágicamente después de hacer los repasos.
En su lugar, formarán un acumulado de tarjetas probablemente olvidadas.
Como quieres repasar todas tus tarjetas pendientes cada día,
ajusta este valor a uno alto.

#### Modificador de intervalo

Aquí es donde se pone interesante.
Cuando respondes **Bien** en una tarjeta, se recalcula su intervalo:

```
Nuevo intervalo = intervalo actual * Facilidad de la tarjeta * Modificador de intervalo
```

De manera predeterminada, el nuevo intervalo es `2.5 * último intervalo`.
Con su valor predeterminado del 100%, el `Modificador de intervalo` no hace nada.
Sin embargo, esto no es lo que deseas,
ya que acabas de reducir la `Dificultad inicial` al 131% en la sección anterior.
Para restaurar el equilibrio, aumenta el `Modificador de intervalo` al 192%.
`1.92 * 1.31` es aproximadamente igual a `2.5`.

Más adelante, después de usar Anki durante unos meses y tener una alta *tasa de retención*,
puedes aumentar aún más el valor y hacer menos repasos.
Si olvidas demasiadas tarjetas, se recomienda reducirlo un poco.

#### Bonificación por fácil e intervalo por difícil

Ignora estas configuraciones, ya que nunca debes usar los botones "Difícil" y "Fácil".

<p align="center"><img alt="dificil-facil" class="shadow" src="img/anki-buttons.webp"></p>

Los botones "Difícil" y "Fácil" tienen efectos contraproducentes en el algoritmo de Anki,
lo que causa problemas a largo plazo con la Facilidad de tus tarjetas.

[AJT Flexible Grading](https://ankiweb.net/shared/info/1715096333) puede ocultar los botones no deseados.
Se explicará con más detalle más adelante.

Una forma alternativa de hacer que los botones "Difícil", "Bien" y "Fácil" se comporten de la misma manera sería
[utilizar el mecanismo de programación personalizada del planificador V3](https://forums.ankiweb.net/t/low-key-anki-with-v3-scheduler-s-custom-scheduling/19707).

#### Intervalo máximo

Los intervalos de tus tarjetas nunca pueden aumentar más allá de este límite.
Recomiendo establecerlo lo más alto posible.
El valor predeterminado es `36500` días, que es igual a `100` años.
Sin embargo, puedes disminuir este número si deseas asegurar una retención a largo plazo.

<p align="center"><img alt="repasos" class="shadow" src="img/options-groups-reviews.webp"></p>

### Olvidos

#### Pasos (en minutos)

Funciona de manera similar a la configuración en la pestaña "Tarjetas Nuevas",
excepto que se aplica a las tarjetas en las que has presionado "Volver a mostrar".
Esto afecta la forma en que volverás a aprender tus tarjetas olvidadas.
Los principiantes deben establecer un único paso de aprendizaje y observar su experiencia.
El valor predeterminado de `10` minutos está bien, pero yo prefiero uno ligeramente mayor.
Más adelante, puedes experimentar con más pasos de aprendizaje.

#### Nuevo intervalo

A menudo, aún recuerdas un palabra en japonés aunque la falles.
Un contexto diferente, otra palabra o estudiarla en otro día pueden ayudar a refrescar tu memoria.
Por lo tanto, no es necesario penalizar completamente un fallo aquí.

Por ejemplo, si usas un nuevo intervalo del 50%,
cuando olvidas una tarjeta y la vuelves a aprender,
el intervalo no se reiniciará a 1 día,
sino que será la mitad del intervalo anterior.
El rango recomendado en la comunidad AJATT está entre el 50% y el 75%.

Para una baraja de `tarjetas de palabras`, puedes establecerlo en aproximadamente el 30-40%,
ya que las tarjetas de palabras son notablemente más difíciles que las `tarjetas de oraciones`.
Explicaré las diferencias entre las plantillas de tarjetas más adelante.

#### Umbral de repeticiones fallidas y Acción para repeticiones fallidas

*Leeches* son tarjetas que sigues olvidando y volviendo a aprender una y otra vez.
Mantén el umbral de repeticiones fallidas bajo (4-6 olvidos) y suspende las tarjetas cuando se conviertan en leeches.
Debes ocuparte adecuadamente de las leeches en lugar de permitir que se sigan rotando en tu baraja y te ralenticen.

Formas posibles de lidiar con las leeches:

* **Eliminarlas:** Para esa pequeña minoría de tarjetas que simplemente no se quedan en tu memoria,
  es mejor deshacerte de ellas. En lugar de perder mucho tiempo en una única leech,
  es más productivo aprender 5 tarjetas normales en su lugar.

* **Dejarlas para más tarde:** Si no puedes recordar una palabra después de 4-5 olvidos,
  significa que tu cerebro aún no ha sido preparado para adquirirla.
  Espera uno o dos meses y vuelve a intentarlo.
  A menudo, descubrirás que las tarjetas que antes no se quedaban, se vuelven muy fáciles.

* **Crear una nueva tarjeta para la misma palabra objetivo:** Si una palabra es de gran valor para ti,
  puedes intentar memorizar una
  [representación diferente](https://www.supermemo.com/de/archives1990-2015/articles/20rules)
  de ella.
  Encuentra una oración de ejemplo diferente en tu Banco de Oraciones
  o [en línea](resources.html#examples-and-pronunciations).
  Por ejemplo, en [Weblio](https://ejje.weblio.jp/sentence/).

<p align="center"><img alt="olvidos" class="shadow" src="img/options-groups-lapses.webp"></p>

### Orden de visualización

Aquí la mayoría de las configuraciones no son tan significativas.
Siéntete libre de experimentar por ti mismo.

**Orden de tarjetas nuevas/repaso** parece ser el equivalente actual
de la configuración **Mostrar tarjetas nuevas después de repasar** que antes se encontraba en [Preferencias](#preferences).
Para mantener el mismo comportamiento, establece esta opción en "Mostrar después de repasar".

Si has establecido [Tarjetas nuevas/día](#new-cards) en 0, esta configuración no debería tener efecto.

## Sincronización de colecciones grandes

No sincronices tu colección con AnkiWeb
si almacenas archivos grandes en ella
o si eres un usuario intensivo de [subs2srs](our-immersion-learning-toolset.html#subs2srs).
Las barajas de `subs2srs` ocupan mucho espacio en el disco.
Utiliza un perfil de Anki diferente para almacenarlos.
El perfil adicional no debe sincronizarse.

Para crear varios perfiles, haz clic en "Archivo" > "Cambiar de perfil".

Como alternativa, utiliza un servidor de sincronización personal de Anki.
[anki-sync-server](https://aur.archlinux.org/packages/anki-sync-server-git)
es un servidor de sincronización para Anki con el que puedes sincronizar en lugar de usar AnkiWeb.

El Infierno de la Facilidad

El Infierno de la Facilidad es cuando Anki disminuye gradualmente los factores de facilidad de tus tarjetas, asumiendo que son más difíciles de lo que realmente son. Una tarjeta con un factor de facilidad bajo debe ser revisada con más frecuencia. Como resultado, te ves obligado/a a revisar demasiadas tarjetas cada día.

Anki disminuye el factor de facilidad de una tarjeta cada vez que la respondes incorrectamente o seleccionas "Difícil". Esto hace que los intervalos de tiempo crezcan más lentamente y, eventualmente, la mayoría de tus tarjetas acaben teniendo un factor de facilidad bajo. Esto es lo que se conoce como estar en el **Infierno de la Facilidad**.

De manera similar, al seleccionar "Fácil", el factor de facilidad aumenta. Los intervalos de tiempo de esas tarjetas crecen más rápidamente que lo normal, lo que lleva a olvidarlas en el futuro.

Efectos secundarios de cada botón de respuesta:

- Nuevamente: el factor de facilidad disminuye un 20%.
- Difícil: el factor de facilidad disminuye un 15%.
- Bien: sin efectos secundarios.
- Fácil: el factor de facilidad aumenta un 15%.

La razón por la que recomiendo nunca seleccionar "Difícil" y "Fácil" es evitar los efectos secundarios. Sin embargo, esto no soluciona el problema con el botón "Nuevamente". El valor más bajo posible para el factor de facilidad inicial en Anki es del `131%`. Al establecer el **Factor de Facilidad Inicial** en el valor más bajo posible y, al mismo tiempo, aumentar el **Modificador de Intervalo**, te aseguras de que los factores de facilidad de tus tarjetas no puedan disminuir más, solucionando así el problema.

Existe la posibilidad legítima de que algunas tarjetas de tu colección sean más difíciles que otras. Para tener esto en cuenta, recomiendo establecer un umbral bajo para las **Tarjetas Problemáticas**. Las tarjetas difíciles serán suspendidas más rápidamente. Una vez que una tarjeta se convierta en una tarjeta problemática, debes investigar por qué sucede.

> Abre el Navegador de Anki y escribe `tag:leech` para mostrar tus tarjetas problemáticas.

Si has estado utilizando Anki durante un tiempo antes de leer esta página, es posible que necesites actualizar tu colección para restablecer el factor de facilidad de las tarjetas más antiguas. Para actualizar las tarjetas antiguas, utiliza el complemento [RefoldEase](https://ankiweb.net/shared/info/819023663).

Más sobre el Infierno de la Facilidad:

- [Guía de Intervalos y Pasos de Aprendizaje en Anki](https://redirect.invidious.io/watch?v=1XaJjbCSXT0)
- [El Problema del Factor de Facilidad](https://web.archive.org/web/20200926103540/https://massimmersionapproach.com/table-of-contents/anki/low-key-anki/the-ease-factor-problem/)
- [El Infierno de la Facilidad en Anki](https://readbroca

Tema GTK

Anki utiliza la biblioteca de herramientas [Qt](https://wiki.archlinux.org/title/Qt). Si no estás utilizando Plasma (o posiblemente otro entorno de escritorio basado en Qt), las aplicaciones Qt no se mostrarán con el estilo del tema GTK que hayas seleccionado.

Existen varias formas de indicarle a Anki que utilice tu tema GTK. Pero antes de continuar, ve a "Preferencias" > "Apariencia" y asegúrate de que el "Estilo" esté configurado en "Nativo".

### qt5-styleplugins

1) Si tu versión de Anki utiliza `Qt5`, instala [qt5-styleplugins](https://aur.archlinux.org/packages/qt5-styleplugins/). Si tu versión de Anki utiliza `Qt6`, instala [qt6gtk2](https://aur.archlinux.org/packages/qt6gtk2).
2) Configura la siguiente [variable de entorno](how-do-i-change-an-environment-variable.html):

   ```
   export QT_QPA_PLATFORMTHEME=gtk2
   ```

Luego, cierra sesión o reinicia el sistema.

### kvantum

Instala los requisitos: `kvantum`, `qt5ct`, `qt6ct`.

```
$ sudo pacman -S kvantum qt5ct qt6ct
```

1) Ejecuta `kvantummanager`, selecciona "Cambiar/Eliminar Tema" y elige tu tema en el cuadro de selección.
2) Presiona "Usar este tema" y luego "Salir".
3) Abre `qt5ct` y `qt6ct`. Selecciona `kvantum` como motor de temas. Aplica los cambios.
4) Configura la siguiente [variable de entorno](how-do-i-change-an-environment-variable.html):

   * Si tu versión de Anki utiliza `Qt6`: `export QT_QPA_PLATFORMTHEME=qt6ct`
   * Si tu versión de Anki utiliza `Qt5`: `export QT_QPA_PLATFORMTHEME=qt5ct`

Luego, cierra sesión o reinicia el sistema.

Este método funciona de manera consistente si Anki utiliza `Qt5`. Actualmente, hay problemas con `Qt6`. Para solucionarlo, instala la versión de Anki para `Qt5` (y/o [desinstala](https://pip.pypa.io/en/stable/cli/pip_uninstall/) los paquetes `PyQt6-*` con `pip` si los has instalado) y, en lugar de establecer la variable de entorno a nivel del sistema, configúrala localmente. Puedes lograrlo ejecutando Anki de la siguiente manera:

```
QT_QPA_PLATFORMTHEME=qt5ct anki
```

Para que la configuración sea persistente, en el archivo `.desktop` (consulta las [notas de instalación](setting-up-anki.html#using-pip) de `pip`) cambia `Exec=` por:

```
Exec=env QT_QPA_PLATFORMTHEME=qt5ct anki %f
```

Si deseas instalar y probar múltiples versiones de Anki al mismo tiempo, puedes utilizar las siguientes funciones. Agrégalas a tu archivo `~/.bashrc` o `~/.zshrc`.

Para instalar una versión específica, por ejemplo, ejecuta `anki_test_install 45` para instalar Anki 2.1.45.

```bash
anki_test_install() {
	local -r version=${1:?No se proporcionó ninguna versión.}
	local -r dir=~/.local/share/anki_builds/"anki_$version"
	(
		mkdir -p -- "$dir" && cd -- "$dir" || exit
		python -m venv --system-site-packages pyenv
		./pyenv/bin/pip3 install --upgrade pip
		./pyenv/bin/pip3 install --upgrade --pre "aqt==2.1.$version"
	)
}
```

Para ejecutar una versión específica, este script utiliza [dmenu](https://wiki.archlinux.org/title/Dmenu) para preguntar qué versión quieres ejecutar.

```bash
anki_test_run() {
	local -r dir=~/.local/share/anki_builds
	if [[ $* ]]; then
		local -r choice=$*
	else
		local -r choice=$(ls -1 "$dir" | dmenu)
	fi
	if [[ -n $choice ]]; then
		(cd -- "$dir/$choice" && ./pyenv/bin/anki)
	fi
}
```

Estas funciones están disponibles en [mi GitHub](https://github.com/tatsumoto-ren/dotfiles/blob/main/.config/shell/functionrc).

Si estás estudiando ciertos caracteres de la "旧字体" (kanji tradicionales utilizados en Japón antes de 1946), es posible que hayas notado que cuando los agregas en Anki, se [convierten automáticamente](https://docs.ankiweb.net/editing.html?highlight=norma#unicode-normalization) a sus versiones de "新字体" (forma simplificada de kanji utilizada en Japón desde 1946). Por ejemplo, si creas una tarjeta con el carácter 「禎」, al abrir la tarjeta nuevamente, el kanji se reemplaza por 「禎」.

Si estás estudiando caracteres de "旧字体", incluyendo ciertos kanji utilizados para nombres, y deseas evitar que se conviertan en equivalentes modernos, abre la consola de depuración presionando <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>;</kbd> y pega lo siguiente. Presiona <kbd>Ctrl</kbd>+<kbd>Enter</kbd> para aplicar los cambios.

```
mw.col.conf["normalize_note_text"] = False
```

Esta configuración debe aplicarse **a cada colección** (perfil de Anki) de forma individual.

Lee este [post del foro de Anki](https://forums.ankiweb.net/t/inconsistent-unicode-normalization/22634) como referencia.

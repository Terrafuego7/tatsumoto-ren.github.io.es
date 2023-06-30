---
title: Guía rápida de Matrix
date: 1655322524
tags: [matrix]
---

Este artículo es una guía de usuario de Matrix.
También cubre el programa cliente de Matrix más popular, Element.

****

## ¿Qué es Matrix?

Matrix es un protocolo de chat en Internet.
Puedes enviar mensajes a personas de manera personal o en chats grupales,
enviar archivos
y utilizar cifrado de extremo a extremo para asegurar tus comunicaciones.
A diferencia de Discord o Telegram, Matrix es federado.
Está compuesto por muchos servidores,
cada servidor aloja cuentas y chats de Matrix.
Creas una cuenta en un servidor de Matrix,
este se comunica con otros servidores de Matrix en tu nombre y te envía los datos.
El correo electrónico es un ejemplo de un protocolo federado.

En Matrix, los nombres de usuario se conocen como `MXID`s (Matrix IDs),
los chats como `room`s
y los servidores como `homeserver`s.
También puedes agrupar salas para formar `space`s.
Los espacios en Matrix se comportan como los "servidores" de Discord.

## Por qué usar Matrix

Existen varias ventajas importantes en Matrix que atraen a nuevos usuarios.

1) Protección contra moderadores.
   Si eliges un `homeserver` confiable o alojas uno tú mismo,
   no perderás tu cuenta ni tus chats.
   En Discord, no es raro que se prohíban "servidores".
   Como resultado, tienes que crear uno nuevo e invitar de nuevo a los antiguos miembros.
   Nadie te garantiza que no te prohibirán el acceso nuevamente.

   Aunque los `homeservers` de Matrix pueden prohibir salas,
   no pueden ordenar a otros `homeservers` hacer lo mismo.
   Una sala existe siempre y cuando haya al menos un `homeserver` que no la haya prohibido.
2) Tanta libertad.
   Cada componente del ecosistema de Matrix es
   [software libre](https://www.gnu.org/philosophy/free-sw.html).
   Esto garantiza que no estás ejecutando
   [software malicioso](https://www.gnu.org/proprietary/)
   en tu computadora,
   y sabes lo que el software está haciendo.
3) Cifrado.
   El cifrado asegura que solo tú y las personas con las que estás hablando
   puedan leer el contenido de los mensajes.
   El cifrado es compatible con muchos servicios de mensajería,
   pero en Matrix es confiable y fácil de usar.
   El sistema de cifrado de mensajes utilizado en Matrix ha sido auditado de forma independiente.

   Ten en cuenta que el cifrado puede estar activado o desactivado de forma predeterminada
   según la aplicación cliente y el `homeserver` que utilices.
   Se recomienda habilitarlo al crear salas privadas,
   pero dejarlo desactivado al crear salas públicas.
   Las salas públicas de todos modos pueden ser leídas por cualquier persona.
   Las salas grandes comienzan a tener retrasos si están cifradas.
4) Todas las funciones habituales de un software de mensajería.
   Chats grupales,
   mensajes directos,
   mensajes de voz,
   llamadas de voz y video,
   emojis y stickers,
   compartir archivos y medios, etc.

## Salas en Matrix

Todas las comunicaciones en Matrix ocurren a través de las salas de Matrix.
Cuando le envías un mensaje a alguien directamente, también creas una sala,
excepto que se etiqueta como directa en la configuración de tu cuenta.

Cuando un nuevo usuario se une a una sala,
la sala se copia en su `homeserver`.
Esta acción puede tomar algo de tiempo en completarse.
Si el servidor ya tiene una copia de la sala,
el usuario se une de inmediato.

Los `homeservers` participan en las salas en nombre de sus usuarios.
Dado que cada servidor tiene una copia de la sala, esto crea redundancia.
Mientras al menos dos `homeservers` diferentes participen en una sala,
la sala se mantiene activa incluso si uno de los servidores se desconecta.
Cuando el último participante en un `homeserver` en particular abandona una sala,
*se supone que la sala será eliminada del `homeserver`*.
Cuando el último participante abandona la sala,
esta se vuelve inaccesible y nadie puede unirse a ella nuevamente.

Los `homeservers` pueden cerrar (prohibir) salas.
Si intentas unirte a una sala prohibida, recibirás un mensaje de error que dice:
"Esta sala ha sido bloqueada en este servidor."
Esto indica que deberías abandonar tu `homeserver` actual porque está controlado por fanáticos del control.

Los administradores de salas pueden bloquear `homeservers`.
Si intentas unirte a una sala que ha bloqueado tu `homeserver`,
recibirás un mensaje de error que dice:
"El servidor está prohibido en esta sala."
Esto indica que necesitas una nueva cuenta en otro `homeserver` para unirte a la sala.

Las salas tienen [versiones](https://spec.matrix.org/unstable/rooms/).
Al crear una sala nueva, debes elegir la última versión para obtener todas las características posibles.
La versión de la sala no se puede cambiar en el futuro,
pero la sala se puede actualizar a una versión más reciente.
La actualización crea una nueva sala con el mismo nombre y vincula la sala antigua a la nueva sala.

## Espacios en Matrix

Un espacio en Matrix es una sala especial que contiene referencias a otras salas.
Cuando un usuario ingresa a un espacio, ve su descripción y una lista de salas para unirse.
Los espacios pueden residir dentro de otros espacios.
Una sala puede pertenecer a más de un espacio.

* Piezas de automóviles (espacio)
	* Ruedas
	* Motor
	* Asientos
	* Ventanas

Normalmente, no envías mensajes a un espacio.
Los espacios solo actúan como colecciones de otras salas.

## Cuentas en Matrix

Creas tu cuenta en un servidor.
El servidor almacena todos los datos de tu cuenta.
También almacena todas tus salas y el historial de mensajes.

Cuando registras una cuenta nueva,
un `homeserver` puede solicitar tu dirección de correo electrónico y/o número de teléfono.
El administrador del servidor puede ver estos datos,
por lo que si deseas tener mayor privacidad, debes encontrar un `homeserver` que no los solicite.

A diferencia de las salas en Matrix, las cuentas en Matrix no tienen redundancia.
Si crees que tu `homeserver` podría desconectarse en algún momento o prohibirte,
mantén una segunda cuenta (un alias) registrada en un `homeserver` diferente.

En algún momento, Matrix puede volverse más independiente de los `homeservers`
y permitir a los usuarios mantener sus datos de cuenta localmente.
Hasta entonces, ten en cuenta que los `homeservers` pueden cerrar inesperadamente y llevarse las cuentas consigo.

## Instalar un programa cliente

Para comunicarte en Matrix, necesitas cualquier cliente de Matrix.

* Todos los clientes de Matrix están listados en [Arch Wiki](https://wiki.archlinux.org/title/List_of_applications/Internet#Matrix_clients).
* Si utilizas un teléfono, abre [F-droid](https://f-droid.org/) y busca clientes de Matrix.
  Por lo general, la gente instala `Element` o `Fluffychat`.
* [Nheko](https://github.com/Nheko-Reborn/nheko)
  a menudo requiere
  [esta solución](https://github.com/Nheko-Reborn/nheko/issues/1187#issuecomment-1255831124).

## Elegir un homeserver

Consulta la [Lista de servidores de Matrix](list-of-matrix-servers.html).

Si tienes tu propio sitio,
puedes [alojar un servidor de Matrix](https://redirect.invidious.io/watch?v=dDddKmdLEdg) en él.
Si no, elige un servidor que tenga registro abierto.

Nunca uses `matrix.org` para nada más que para molestar,
y ten en cuenta que los administradores de `matrix.org` venderán tus datos a Israel.

## Ejecutar Element localmente

Element-Desktop se construye con Electron.
Es posible que no te guste porque se ejecuta en una instancia separada del navegador,
tarda mucho en iniciarse y consume mucha memoria RAM.
Si no puedes soportarlo, puedes cambiar a
[otro cliente popular](https://write.midov.pl/midek/software-list#matrix-client).
Como alternativa, puedes ejecutar Element en tu navegador.
La forma más sencilla de hacerlo es abrir [una instancia que alguien más haya configurado](list-of-matrix-servers.html#with-element).

Sin embargo, es posible que tampoco quieras hacer eso, porque:

* Tu `homeserver` no tiene Element integrado.
* La conexión a una instancia remota es lenta.
* No confías en otro tercero.

La solución es servir Element localmente con un servidor web y acceder a él en un navegador web.

Necesitarás:

* Cualquier servidor web, como `nginx`.
  Yo uso [darkhttpd](https://archlinux.org/packages/community/x86_64/darkhttpd/).
* [element-web](https://archlinux.org/packages/community/x86_64/element-web/).
  Si ya tienes instalado `element-desktop`, automáticamente tienes `element-web`.

La parte final es ejecutar el servidor y abrir Element en tu navegador web.

```
darkhttpd /usr/share/webapps/element --port 8000 --addr 127.0.0.1 --daemon --log /dev/null
```

Ahora ve a http://127.0.0.1:8000/ e inicia sesión en tu cuenta.

He escrito
[un pequeño script](https://aur.archlinux.org/cgit/aur.git/tree/element-web.sh?h=element-desktop-git-greentext)
para **iniciar** y **detener** rápidamente una instancia local de element-web.
Es parte de
[mi versión de Element](https://aur.archlinux.org/packages/element-web-greentext/).

**Consideraciones.**

* element-web no funciona bien con
  [uMatrix](https://addons.mozilla.org/en-US/firefox/addon/umatrix/).
  uMatrix bloquea conexiones de terceros,
  por lo que debes desbloquear la URL de tu `homeserver`.
  Ni siquiera se iniciará a menos que bloquees el `homeserver` predeterminado (establecido en `/etc/element/config.json`).
  Si te gusta probar diferentes `homeservers`, esto se vuelve molesto rápidamente.
* Ciertas funciones de Element dependen de la capacidad
  de copiar o pegar contenido en el portapapeles del sistema con JavaScript.
  Si usas Firefox o una derivada,
  es posible que debas establecer `dom.event.clipboardevents.enabled` en `true`
  para cargar imágenes y archivos multimedia almacenados en el portapapeles
  y `dom.allow_cut_copy` en `true` para copiar enlaces de salas al portapapeles.

## Configurando Element

Element tiene un menú de Configuración.
Desafortunadamente, hay algunas configuraciones a las que no se puede acceder sin modificar el archivo de configuración.
Si estás ejecutando `element-web` localmente, edita `/etc/element/config.json`.
Si estás ejecutando `element-desktop` (la aplicación electron), crea o edita `~/.config/Element/config.json`.
Crea el archivo si aún no existe.

En el archivo de configuración, habilita "Labs" para acceder a las configuraciones ocultas.

```
{
	"showLabsSettings": true
}
```

Después de reiniciar Element,
los Labs aparecerán en Configuración.

<p align="center"><img alt="Configuración" src="img/element-labs.webp"></p>
<p align="center"><i>Labs en Configuración.</i></p>

Dentro de Labs,
recomiendo habilitar lo siguiente.

1) Anclar mensajes. Permite ver los mensajes anclados en las salas.
2) Mensajes en hilos. Permite acceder a hilos dentro de las salas.
Un hilo es una sublínea de tiempo donde las personas pueden conversar de forma independiente a la línea principal.
3) Modo de desarrollador. Facilita el acceso a ciertas funciones.
4) Mostrar eventos ocultos en la línea de tiempo.

Configuración adicional.

* Puedes encontrar una documentación de las características de Labs
  [aquí](https://github.com/vector-im/element-web/blob/develop/docs/labs.md).
* Hay muchas más cosas que puedes modificar en `config.json`, consulta
  [esta página](https://github.com/vector-im/element-web/blob/develop/docs/config.md) para ver la lista de configuraciones.

También puedes obtener un archivo de configuración de una instancia existente.
Por ejemplo, de esta manera.

```
# curl 'https://element.midov.pl/element/config.json' -o '/etc/element/config.json'
```

Cada instancia pública de Element tiene su propio archivo de configuración.

## Uso de múltiples cuentas

Si deseas utilizar varias cuentas diferentes al mismo tiempo,
puedes probar las siguientes opciones.

* Element-desktop admite múltiples perfiles.
  Así es como puedes iniciar un nuevo perfil.

  ```
  $ element-desktop --profile "nombre-de-perfil"
  ```
* Puedes tener múltiples pestañas de contenedor en Firefox, cada una ejecutando Element.
* [Ferdium](https://aur.archlinux.org/packages?O=0&K=ferdium).
  Una aplicación de escritorio que te ayuda a combinar varios servicios en una sola aplicación.
  Está basado en Chromium y es bastante pesado (más de 300 MiB después de la instalación).

## Unirse a salas

Para unirte a una sala, puedes
hacer clic en un enlace de sala si alguien te lo ha compartido
o aceptar una invitación si alguien te ha invitado.

## Encontrar salas y espacios

* Existe una forma integrada de encontrar salas públicas.
  Abre Element y presiona "Explorar salas".
  Algunos espacios también se enumeran allí.
* El directorio público de matrix.org se puede acceder sin registro aquí
  https://view.matrix.org/
* Para encontrar más salas de Matrix, puedes buscar enlaces `matrix.to/#/` en 4chan.
  1) [4chan find](https://find.4chan.org/?q=matrix.to%2F)
  1) [archived.moe](https://archived.moe/_/search/text/%22https%3A%2F%2Fmatrix.to%2F%23%2F%22/)
  1) [desuarchive](https://desuarchive.org/_/search/text/%22https%3A%2F%2Fmatrix.to%2F%23%2F%22/)
  1) [arch.b4k.co](https://arch.b4k.co/_/search/text/%22https%3A%2F%2Fmatrix.to%2F%22/)
  1) y otros índices similares.

## Se produjo un error al unirse a la sala

Si estás intentando unirte a una nueva sala
y sigues obteniendo constantemente el mensaje "Se produjo un error al unirse a la sala",
debes esperar hasta que tu servidor descargue la sala.
Este error ocurre en `homeservers` de mala calidad.
Crea una nueva cuenta en otro `homeserver` si el error no desaparece.

## Privacidad

Tu `homeserver` almacena copias de todas las salas a las que te has unido.
Esto significa que el operador de tu `homeserver` sabe con quién estás hablando,
incluso si no puede leer los mensajes.
Dado que aún no tenemos mensajería de igual a igual en Matrix,
esto puede considerarse como una preocupación de privacidad.
Elige un `homeserver` en el que puedas confiar o configura el tuyo propio.

Aún así, esto no es tan malo como en Telegram o Discord donde entregas todos tus datos.

## Crear una sala con la última versión

En Element,
puedes crear una nueva sala presionando el botón "Agregar".

Cuando creas una nueva sala a través de Element,
elige la versión de la sala por ti.
A menudo esto no es lo que deseas
porque la versión que elige es más antigua que la última versión disponible.
Puedes solucionarlo creando salas con
[curl](https://wiki.archlinux.org/title/CURL).
La
[API cliente-servidor](https://matrix.org/docs/spec/client_server/r0.6.1#creation)
proporciona una forma de hacerlo.

```
#!/usr/bin/env bash

readonly SERVER=matrix-server.com
readonly TOKEN=my_access_token

curl -X POST -H "Authorization: Bearer $TOKEN" -H "Content-Type: application/json" "https://$SERVER/_matrix/client/r0/createRoom" --data-binary '{
	"room_version": "10",
	"name": "Mi chat",
	"preset": "public_chat",
	"topic": "Bienvenido a mi chat"
}'
```

En el momento de escribir esto, `10` era la última versión.
`SERVER` y `TOKEN` son la URL de tu `homeserver` y el token de acceso de tu cuenta.
En Element, puedes obtenerlos yendo a "Configuración" > "Ayuda y acerca de" > "Avanzado".

## Actualizar a una nueva versión de sala

Cuando hay una nueva versión de sala disponible,
puedes optar por actualizar a la última versión de sala.

```
#!/usr/bin/env bash

readonly ID='!id_de_sala:servidor.com'
readonly SERVER=servidor.com
readonly TOKEN=mi_token_de_acceso

curl -X POST -H "Authorization: Bearer $TOKEN" -H "Content-Type: application/json" "https://$SERVER/_matrix/client/r0/rooms/$ID/upgrade" --data-binary '{
    "new_version": "10"
}'
```

Si esto no funciona, puedes intentar [actualizar manualmente](https://gist.github.com/turt2live/a99c8e794d6115d4ddfaadb72aabf063),
paso a paso.

Cuando actualizas una sala, se crea una nueva sala que reemplaza a la anterior,
por lo tanto, el `ID` de la sala cambia.
En Element, para obtener el `ID` de la sala anterior, ve a "Configuración de sala" > "Avanzado".
No olvides obtener `TOKEN` y `SERVER` siguiendo la sección anterior.

Durante una actualización, se envía un [evento de lápida](https://spec.matrix.org/v1.1/client-server-api/#mroomtombstone) a la sala anterior.
El evento de lápida cierra la sala anterior y la enlaza a la nueva sala.

## Publicar tu sala

Si eliges publicar tu sala, esta aparecerá en el directorio público de tu `homeserver`.
Otros usuarios en tu `homeserver` podrán encontrarla en la página "Explorar salas".

Para publicar una sala, ve a la configuración de la sala y haz clic en
"Publicar esta sala en el directorio público del servidor".

## Publicar tu espacio

Element te permite publicar salas regulares en el directorio público de tu `homeserver`,
pero por alguna razón no hay una opción similar en la configuración de Espacios.
Para publicar tu espacio y facilitar que los nuevos usuarios lo encuentren, ejecuta el siguiente script.

```
#!/usr/bin/env bash

readonly ID='!id_de_sala:servidor.com'
readonly SERVER=servidor.com
readonly TOKEN=mi_token_de_acceso

curl -X PUT -H "Authorization: Bearer $TOKEN" -H "Content-Type: application/json" "https://$SERVER/_matrix/client/r0/directory/list/room/$ID" --data-binary '{
  "visibility": "public"
}'
```

Alternativamente, puedes habilitar las herramientas para desarrolladores,
hacer clic derecho en el espacio,
presionar "Ver línea de tiempo de la sala",
y luego "Configuración".
Esto abrirá la configuración para salas regulares.

## Habilitar invitaciones

Por alguna razón, las salas y espacios recién creados solo permiten a los administradores invitar a nuevos usuarios.
A menudo, esto no es deseable.
Cámbialo yendo a Configuración de la sala > "Roles y permisos" > "Invitar usuarios".

## Enlazar a tu sala

Normalmente puedes compartir tu sala utilizando un enlace que se ve así:
`https://matrix.to/#/#sala:servidor.dominio`.
El inconveniente de usar esos enlaces es que los nuevos usuarios que aún no han registrado una cuenta de Matrix
serán enviados a `app.element.io` y se les sugerirá crear una cuenta en `matrix.org`.
Esto nunca es lo que queremos.
Para solucionarlo, podemos enlazar una instancia específica de Element.

Si estás utilizando una instancia de la versión web de Element,
abre la sala y copia la URL de la barra de direcciones de tu navegador web.
Por lo general, el enlace se verá así: `https://element.anontier.nl/#/room/#g-rust:matrix.org`.
La URL puede no funcionar dependiendo de la configuración de Element establecida por el operador de la instancia,
pruébala primero en una pestaña privada del navegador.

Consulta [Servidores que admiten enlaces a salas](list-of-matrix-servers.html#servers-that-support-links-to-rooms)
para obtener una lista de instancias de Element que pueden reemplazar a `app.element.io`.

## ¿Cómo puedo utilizar el formato de texto verde (greentext)?

Puedes utilizar el formato de texto verde [de esta manera](https://glowers.club/wiki/doku.php?id=wiki:newfriends#how_do_i_greentext),
o puedes instalar [element-web-greentext](https://aur.archlinux.org/packages/element-web-greentext)
con el comando `/greentext` incorporado.
[QuickMedia](https://git.dec05eba.com/QuickMedia/about/) admite el formato de texto verde de forma predeterminada.

<p align="center"><img src="img/element-greentext.webp"></p>
<p align="center"><i>Cómo la gente utiliza el formato de texto verde.</i></p>

## Consejos para administradores de salas

Si decides crear y gestionar una sala pública grande,
es muy importante que no pierdas acceso a ella.
Incluso los grandes homeservers a veces desaparecen sin regresar.
Siempre mantén al menos dos cuentas de administrador en la sala, cada una alojada en un homeserver **diferente**.
Si un homeserver se desconecta o decide bloquearte o *cerrar* tu sala,
aún podrás controlar la sala a través de la otra cuenta de administrador.

Lo más importante que debes tener en cuenta como administrador de una sala son las
[clausuras de sala](https://github.com/matrix-org/synapse/blob/develop/docs/admin_api/rooms.md#delete-room-api).
Una clausura de sala ocurre cuando un administrador de homeserver
expulsa a todos los miembros registrados en el homeserver
de tu sala
y evita futuras incorporaciones.
Una clausura de sala solo afecta a los usuarios en el servidor que inició la clausura.
Para minimizar el posible daño que una clausura pueda causar a tu sala,
siempre indica a tus miembros que utilicen homeservers en los que confíes.

Elige un servidor que ejecute la última versión de
[Synapse](https://github.com/matrix-org/synapse).
Las versiones más nuevas te dan acceso a versiones de sala más avanzadas.
Para verificar la versión de Synapse de un servidor, ejecuta el siguiente comando en la terminal.
Reemplaza `homeserver.name` con la URL de tu homeserver, por ejemplo, `midov.pl`.

```
curl -s 'https://homeserver.name/_matrix/federation/v1/version'
```

Alternativamente, puedes pegar la URL del servidor en
[probador de federación](https://federationtester.matrix.org/).

Es una buena idea bloquear completamente la participación de ciertos servidores en tu sala, utilizando
[ACLs del servidor](https://matrix.org/docs/guides/moderation#banning-servers-from-rooms-server-acls).
Las ACLs del servidor te permiten bloquear todas las cuentas registradas en homeservers no deseados
para que no puedan unirse a tu sala.
El homeserver que se bloquea con más frecuencia es, como ya te imaginarás, `matrix.org`.

## Lecturas adicionales

* [https://glowers.club/wiki/doku.php?id=wiki:newfriends](https://glowers.club/wiki/doku.php?id=wiki:newfriends)
* [https://www.schotty.com/Services/Matrix/](https://www.schotty.com/Services/Matrix/)
* [https://community.kde.org/Matrix](https://community.kde.org/Matrix)
* [https://calcuode.com/matrix/](https://calcuode.com/matrix/)

---
title: Lista de servidores de Matrix
date: 1611943875
tags: ['matrix']
---

[Matrix](https://wiki.archlinux.org/index.php/Matrix) es un protocolo de código abierto y federado para mensajería instantánea. El ecosistema de Matrix consiste en muchos servidores que se pueden utilizar para el registro. Esta es una lista de servidores de Matrix para aquellos que preguntan qué servidor elegir para registrarse.

Para usar Matrix, primero instala un [cliente](https://wiki.archlinux.org/index.php/List_of_applications#Matrix_clients). Uno de los clientes más populares es [Element](https://archlinux.org/packages/?name=element-desktop).

Si eres nuevo en Matrix, lee la [guía de inicio rápido de Matrix](matrix-quickstart-guide.html).

****

## Usuarios de Matrix.org

Si ya tienes una cuenta alojada en Matrix.org, por favor desactiva tu cuenta y crea una nueva cuenta en otro servidor de inmediato. Matrix.org es el servidor de Matrix más grande y la mayoría de las aplicaciones de Matrix lo sugieren por defecto. Muchos usuarios nuevos en Matrix terminan usando este servidor porque no saben que existen otros servidores. Desafortunadamente, Matrix.org está lejos de ser la mejor opción. Debido a sus reglas absurdamente estrictas, el servidor es conocido por los frecuentes bloqueos de salas y cuentas de usuario, y lo hace sin previo aviso. Básicamente, Matrix.org utiliza su tamaño y estatus especial para imponer la censura.

Afortunadamente, cambiar de servidor de Matrix es tan fácil como cambiar de proveedor de correo electrónico. A continuación, tengo una lista de servidores con términos de servicio menos estrictos.

<p align="center"><img class="shadow" alt="registration" src="img/element_registration.webp"></p>
<p align="center"><i>Haz clic en "Editar".</i></p>

## Cómo elegir

Elige un servidor que no participe en purgas caóticas de cuentas o salas. Estar en un servidor así no es diferente a estar en Discord. Si un servidor tiene reglas, léelas para comprobar si son excesivamente estrictas. Mantente alerta ante las señales de comportamientos problemáticos. Por ejemplo, si un servidor intenta suprimir ciertas opiniones políticas, restringirte de publicar ciertos tipos de contenido o [imponer un entorno autoritario](https://glowers.club/wiki/doku.php?id=jannies).

## Recomendaciones

Idealmente, alojarías tu propio servidor en tu propio hardware, pero no todos pueden hacerlo. Esta sección contiene servidores seleccionados por mí y terceros de confianza. Con el símbolo 🏆 he marcado los servidores que han recibido un <span title="bloqueo ACL">premio de reconocimiento</span> del equipo de Matrix HQ.

No todos los servidores pueden estar abiertos para registrarse en cualquier momento. Es posible que debas enviar un correo electrónico a un administrador para obtener una cuenta.

### Servidores recomendados por [#d:anontier.nl](https://matrix.to/#/#d:anontier.nl):

| Servidor                | Cliente web                                      | Extra                 |
| :---                    | :---                                             | :---                  |
| `community.rs`          | [element](https://element.community.rs)          |                       |
| `matrix.im`             | [element](https://element.matrix.im)             |                       |
| `sibnsk.net`            | [element](https://element.sibnsk.net)            |                       |
| `matrix.unredacted.org` | [element](https://element.unredacted.org)        | última verificación - cerrado |
| `zelchat.de`            | [chat.zelchat.de](https://chat.zelchat.de/)      |                       |

### Mi selección

| Servidor            | Cliente web                                                      | Extra                                                |
| :---                | :---                                                             | :---                                                 |
| `cutefunny.art`     | [cutefunny.art](https://matrixclient.cutefunny.art/)              | 🏆                                                   |
| `sakura.ci`         | [web.sakura.ci](https://web.sakura.ci/)                            |                                                      |
| `iddqd.chat`        | [iddqd.chat](https://iddqd.chat/)                                  | última verificación - cerrado                                |
| `trygve.me`         | [trygve.me](https://element.trygve.me/)                            |                                                      |
| `nitro.chat`        | [nitro.chat](https://app.nitro.chat/)                              |                                                      |
| `midov.pl`          | [midov.pl](https://element.midov.pl/element/)                      | [Regístrate aquí](https://midov.pl/registerform.sh) 🏆 |
| `koneko.chat`       | [element.koneko.chat](https://element.koneko.chat/)                |                                                      |
### Selecciones inteligentes sobre confianza de cuentas, listadas

Igual que algunos mencionados anteriormente.

| Servidor        | Cliente web                                              | Extra |
| :---            | :---                                                     | :---  |
| `eientei.org`   | [matrix.eientei.org](https://matrix.eientei.org/)        |       |

### Servidores gestionados por personas japonesas

| Servidor              | Cliente web                                              | Extra |
| :---                  | :---                                                     | :---  |
| `matrix.fedibird.com` | [fedibird.com](https://element.fedibird.com/)             | 🏆    |
| `matrix.juggler.jp`   | [juggler.jp](https://matrix-element.juggler.jp/)          |       |

Fuente: [matrix-room-list-jp](https://matrix-room-list-jp.netlify.app/)

### Una lista de homeservers recomendados por [Glowers Club](https://web.archive.org/web/20221208070442/https://glowers.club/wiki/doku.php?id=start)

| Servidor                  | Cliente web                                              | Extra                    |
| :---                      | :---                                                     | :---                     |
| `matrix.thisisjoes.site`  | [thisisjoes.site](https://element.thisisjoes.site/)      | última verificación - cerrado    |
| `nerdsin.space`           | [nerdsin.space](https://nerdsin.space/)                  | última verificación - cerrado 🏆 |

## No utilizar

Esta lista contiene servidores populares que han demostrado ser poco confiables. Se añade un servidor a esta lista si se ha descubierto que bloquea cuentas de usuario o salas sin previo aviso.

| Servidor                         | Información                                                                                                                                   |
| :---                             | :---                                                                                                                                          |
| `waifuhunter.club`               | El administrador desactivó las cuentas de los usuarios sin previo aviso.                                                                       |
| `matrix.org`                     | Se explicó anteriormente.                                                                                                                     |
| `*.modular.im` o `*.ems.host`     | Afiliados a matrix.org.                                                                                                                       |
| `tchncs.de`                      | El administrador bloqueó salas en busca de censura.                                                                                            |
| `asra.gr`                        | El administrador desactivó las cuentas de los usuarios después de recibir informes falsos.                                                    |
| `3000.chat`                      | El administrador desactivó las cuentas de los usuarios después de recibir informes falsos.                                                    |
| `lolisho.chat`                   | El administrador desactivó las cuentas de los usuarios sin motivo aparente. El administrador filtró direcciones IP de algunos usuarios.         |
| `synod.im`                       | El administrador desactivó las cuentas de los usuarios sin motivo aparente.                                                                   |
| `utwente.io`                     | El administrador desactivó las cuentas de los usuarios sin motivo aparente.                                                                   |
| `envs.net`                       | El administrador bloqueó salas en busca de censura.                                                                                            |
| `halogen.city`                   | Solía recomendar este servidor, pero nuestros miembros se quejaban constantemente de tener problemas al unirse a salas. Además, el servidor es lento. |

Una lista completa que incluye servidores menos populares está disponible [aquí](https://tatsumoto-ren.github.io/matrix/#blocklist).

## Otros servidores

### Lista ordenada

Tengo una lista ordenada que se actualiza automáticamente cada 12 horas [aquí](https://tatsumoto-ren.github.io/matrix/).

Criterios de selección.

* Registro abierto
* Longitud de dominio
* Versión actualizada de Synapse

La lista es útil para obtener servidores nuevos y actualizados,
pero no hay garantía de que los resultados sean buenos.

### Servidores que admiten enlaces a salas

Una lista separada de servidores que se pueden utilizar para enlazar salas.
Esto es muy útil si deseas compartir una sala con alguien
pero no quieres usar `element.io` o `matrix.to` porque están detrás de Cloudflare
o porque tu sala no se puede alcanzar a través de `matrix.to`.

Para enlazar una sala, agrega `#/room/#tu_sala:ejemplo.com`
a la dirección de Element de la instancia,
como esto: `https://c.wfr.moe/#/room/#djtspace.midov.pl`.

* https://element.fablabchemnitz.de/
* https://riot.ukvly.org/
* https://riot.tzchat.org/
* https://crystal-temple.flak.is/
* https://im.tetaneutral.net/
* https://nerdsin.space/ 🏆
* https://matrix.mlp.chat/
* https://matrix.eientei.org/
* https://im.tetaneutral.net/
* https://element.arcticfoxes.net/

### Con Element

Estos servidores tienen [Element](https://web.archive.org/https://element.io/). Es una aplicación web que puedes usar para chatear sin necesidad de utilizar un cliente de escritorio.

* https://chat.darkcloud.ca/
* https://element.georgefloyd.link/
* https://chat.cfx.re/ 🏆
* https://matrix.dpin.de/ 🏆
* https://chat.vscape.tk/ 🏆
* https://matrix.radu.at/ 🏆
* https://matrix.3dns.eu/ 🏆
* https://fsoc.lol/matrix/ 🏆
* https://riot.shendai.rip/ 🏆
* https://matrix.okoyono.de/ 🏆
* https://element.avlikos.gr/ 🏆
* https://matrix.pittamitz.at/ 🏆
* https://matrix.dandl.bayern/ 🏆
* https://chat.dresden.network/ 🏆
* https://element.crossbach.de/ 🏆
* https://element.schaeferit.de/ 🏆
* https://matrix.patricknour.de/ 🏆
* https://element.tinternet.net/ 🏆
* https://www.schotty.com/matrix/ 🏆
* https://matrix.pancrypticon.net/ 🏆
* https://element.radiowarnerd.org/ 🏆
* https://element.fablabchemnitz.de/ 🏆
* https://comf.chat/
* https://web.yuri.im/
* https://matrix.base8.org/
* https://unita.online/
* https://chat.zelchat.de/
* https://chat.peek-a-boo.at/
* https://element.cccgoe.de/
* https://mx.aire.ml/
* https://matrix.therealblue.de/
* https://element.internet-portal.cz/
* https://element.w1l.duckdns.org/
* https://chat.leon.wtf/
* https://matrix.club-tech.fr/
* https://chat.joinpoint.org/
* https://www.schotty.com/
* https://matrix.riotcat.org/
* https://chat.thorko.de/
* https://chat.cambsac.org.uk/
* https://cell.linuxbrujo.net/
* https://matrix.n2n.io/
* https://chat.das-labor.org/
* https://element.lion.fm/
* https://okaris.de/
* https://element.juniorjpdj.pl/
* https://chat.greensteps.cn/
* https://element.matrix4ulm.de/
* https://c.a2sc.eu/
* https://c.wfr.moe/
* https://uddu.chat/
* https://mx.aire.ml/
* https://chat.usr.nz/
* https://ngonbay.com/
* https://chat.leel.ch/
* https://im.skytel.ee/
* https://talk.comm.cx/
* https://chat.gould.cx/
* https://chat.vyas.net/
* https://gnome.riot.im/
* https://nerdsin.space/
* https://riot.kudos.im/
* https://riot.pcg.life/
* https://riot.zorc.xyz/
* https://salty.riot.im/
* https://app.nitro.chat/
* https://chat.eforah.nl/
* https://element.42l.fr/
* https://chat.thorko.de/
* https://my.m4tr1x.chat/
* https://riot.ukvly.org/
* https://matrix.mlp.chat/
* https://el.aria-net.org/
* https://element.1984.cz/
* https://element.asra.gr/
* https://im.solokeys.com/
* https://matrix.nwca.xyz/
* https://riot.tzchat.org/
* https://webchat.kde.org/
* https://element.fff.chat/
* https://matrix.boba.chat/
* https://riot.backstop.it/
* https://element.kif.rocks/
* https://3000.chat/element/
* https://chat.oscillas.com/
* https://element.eclabs.de/
* https://element.myserv.me/
* https://element.pwoss.org/
* https://element.trygve.me/
* https://chat.freakachu.org/
* https://element.avlikos.gr/
* https://riot.scamdemic.wtf/
* https://webchat.freitrix.de/
* https://mailstation.de/riot/
* https://the-apothecary.club/
* https://chat.fairydust.space/
* https://riot.qonfucius.social/
* https://crystal-temple.flak.is/
* https://element.privacytools.io/
* https://element.thisisjoes.site/
* https://element.midov.pl/element/
* https://grid.rrze.fau.de/riotweb/

### Sin Element

Estos servidores de Matrix no ofrecen la interfaz web, pero aún puedes registrar una cuenta. Instala uno de los clientes que se enumeran en [Arch Wiki](https://wiki.archlinux.org/index.php/List_of_applications#Matrix_clients), haz clic en "crear cuenta", luego busca opciones avanzadas y cambia el servidor por defecto por el que desees.

* https://l12c.eu/ 🏆
* https://fick.es/ 🏆
* https://javil.eu/ 🏆
* https://bmw12.nl/ 🏆
* https://cisek.ca/ 🏆
* https://group.lt/ 🏆
* https://whyc.dev/ 🏆
* https://kleph.eu/ 🏆
* https://linkor.io/ 🏆
* https://lodere.es/ 🏆
* https://faelix.im/ 🏆
* https://ruzik.xyz/ 🏆
* https://denshi.org/ 🏆
* https://obermui.de/ 🏆
* https://kssler.win/ 🏆
* https://priv8.chat/ 🏆
* https://www.hellug.gr/
* https://citadel7.org/ 🏆
* https://lukas.studio/ 🏆
* https://curved.space/ 🏆
* https://lolison.chat/ 🏆
* https://ellipsys.xyz/ 🏆
* https://cl0secall.net/ 🏆
* https://matrix.47q.de/ 🏆
* https://mittelwind.de/ 🏆
* https://tricuties.com/ 🏆
* https://matrix.fuz.re/ 🏆
* https://matrix.fuz.re/ 🏆
* https://matrix.lorf.io 🏆
* https://matrix.dnix.de/ 🏆
* https://chat.thorko.de/ 🏆
* https://matrix.jrop.me/ 🏆
* https://kansanvalta.org/ 🏆
* https://matrix.rptc.bid/ 🏆
* https://matrix.cirk2.de/ 🏆
* https://matrix.wfrei.de/ 🏆
* https://matrix.knax.xyz/ 🏆
* https://schaffarzik.net/ 🏆
* https://tetaneutral.net/ 🏆
* https://plus-sensible.me/ 🏆
* https://skylinetv.stream/ 🏆
* https://matrix.ladiv.org/ 🏆
* https://matrix.ravc.tech/ 🏆
* https://matrix.vleij.com/ 🏆
* https://vanderwarker.dev/ 🏆
* https://matrix.rakozy.us/ 🏆
* https://matrix.glargh.fr/ 🏆
* https://matrix.nesven.eu/ 🏆
* https://matrix.jibby.org/ 🏆
* https://matrix.nesven.eu/ 🏆
* https://pancrypticon.net/ 🏆
* https://matrix.neaweb.ch/ 🏆
* https://matrix.dificen.to/ 🏆
* https://matrix.binwang.me/ 🏆
* https://matrix.huneck.net/ 🏆
* https://matrix.cabaal.net/ 🏆
* https://matrix.prof-x.net/ 🏆
* https://matrix.codenic.de/ 🏆
* https://matrix.poweron.dk/ 🏆
* https://matrix.lazzurs.ie/ 🏆
* https://definitionhub.com/ 🏆
* https://matrix.sumill.com/ 🏆
* https://matrix.grusbv.com/ 🏆
* https://matrix.emri.online/ 🏆
* https://matrix.hofra.rocks/ 🏆
* https://matrix.troback.com/ 🏆
* https://matrix.flick-it.de/ 🏆
* https://neuland.technology/ 🏆
* https://matrix.pangrand.fr/ 🏆
* https://matrix.net4sec.com/ 🏆
* https://chatencriptado.com/ 🏆
* https://matrix.dabbill.com/ 🏆
* https://netrunner-vault.de/ 🏆
* https://matrix.net4sec.com/ 🏆
* https://matrix.nord.digital/ 🏆
* https://chat.deprecated.org/ 🏆
* https://matrix.dunkklar.org/ 🏆
* https://matrix.googboog.com/ 🏆
* https://matrix.heiming.info/ 🏆
* https://gottliebtfreitag.de/ 🏆
* https://matrix.solonari.net/ 🏆
* https://matrix.petrutoni.nl/ 🏆
* https://matrix.zoz-serv.org/ 🏆
* https://matrix.csrichter.com/ 🏆
* https://matrix.jerrycrazy.be/ 🏆
* https://matrix.foreskin.tips/ 🏆
* https://matrix.danyocean.com/ 🏆
* https://matrix.linuxbrujo.net/ 🏆
* https://matrix.thecovrigs.net/ 🏆
* https://matrix.familyhainz.de/ 🏆
* https://matrix.muensterhack.de/ 🏆
* https://matrix.otonokizaka.moe/ 🏆
* https://riot.markshorten.co.uk/ 🏆
* https://matrix.budem.de/_matrix/ 🏆
* https://matrix.leipzigesports.de/ 🏆
* https://matrix.gears-gadgets.com/ 🏆
* https://slipstream.thebell.house/ 🏆
* https://matrix.niveau-keller.com/ 🏆
* https://synapse.mateuszreszka.xyz/ 🏆
* https://llllllllllllllllllllllllllllllllllllllllllllllll.space/ 🏆
* https://mcl.gg/
* https://brad.li/
* https://jn2p.de/
* https://kvbx.de/
* https://stop.pe/
* https://zoit.net/
* https://pcg.life/
* https://oblak.be/
* https://kuvio.de/
* https://m.edw.ai/
* http://rthome.me/
* https://bau-ha.us/
* http://kanik0.wtf/
* https://furry.lol/
* https://koehn.com/
* https://nibbana.jp/
* https://willy.club/
* https://home55.net/
* https://m.webgo.de/
* https://kahakai.de/
* https://tusooa.xyz/
* https://chatmud.com/
* https://secureim.de/
* https://cakeboss.it/
* https://malooma.bzh/
* https://xentonix.net/
* https://xentonix.net/
* https://lolifan.club/
* https://kotilo.dy.fi/
* https://calcuode.com/
* https://converser.eu/
* https://dunstkreis.ch/
* https://chat.filik.eu/
* https://im.su.cvut.cz/
* http://matrix.lod.com/
* https://shirokumo.net/
* https://vanpetegem.me/
* https://matrix.pi2.dev/
* https://drastical.tech/riot/
* https://matrix.phcn.de/
* https://matrix.dhp.com/
* https://matrix.nikel.me/
* https://matrix.ohea.xyz/
* https://matrix.goe.land/
* https://chat.avlikos.gr/
* https://matrix.neko.dev/
* https://matrix.cirr.com/
* https://matrix.altay.fr/
* https://matrix.jarno.ca/
* https://matrix.nx-pod.de/
* https://matrix.sensin.eu/
* https://matrix.privex.io/
* https://matrix.puhoy.net/
* https://matrix.lukamb.de/
* https://matrix.jling.dev/
* https://matrix.bda.space/
* https://matrix.radres.xyz/
* https://matrix.sibnsk.net/
* https://matrix.sykorp.com/
* https://matrix.thegolem.cz/
* https://nekomimi.solutions/
* https://matrix.unknown.place/
* https://matrix.danyocean.com/
* https://matrix.get-racing.de/
* https://matrix.intahnet.co.uk/

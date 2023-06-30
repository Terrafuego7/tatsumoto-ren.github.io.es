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

### Homeservers recommended by [#d:anontier.nl](https://matrix.to/#/#d:anontier.nl):

| Server                  | Web client                                  | Extra                 |
| :---                    | :---                                        | :---                  |
| `community.rs`          | [element](https://element.community.rs)     |                       |
| `matrix.im`             | [element](https://element.matrix.im)        |                       |
| `sibnsk.net`            | [element](https://element.sibnsk.net)       |                       |
| `matrix.unredacted.org` | [element](https://element.unredacted.org)   | last checked - closed |
| `zelchat.de`            | [chat.zelchat.de](https://chat.zelchat.de/) |                       |

### My selection

| Server            | Web client                                           | Extra                                                |
| :---              | :---                                                 | :---                                                 |
| `cutefunny.art`   | [cutefunny.art](https://matrixclient.cutefunny.art/) | 🏆                                                   |
| `sakura.ci`       | [web.sakura.ci](https://web.sakura.ci/)              |                                                      |
| `iddqd.chat`      | [iddqd.chat](https://iddqd.chat/)                    | last checked - closed                                |
| `trygve.me`       | [trygve.me](https://element.trygve.me/)              |                                                      |
| `nitro.chat`      | [nitro.chat](https://app.nitro.chat/)                |                                                      |
| `midov.pl`        | [midov.pl](https://element.midov.pl/element/)        | [Register here](https://midov.pl/registerform.sh) 🏆 |
| `koneko.chat`     | [element.koneko.chat](https://element.koneko.chat/)  |                                                      |

### [Intelligent Selections Regarding Account Entrustment, Listed](https://plan9.rocks/israel/)

Same as some above.

| Server        | Web client                                        | Extra |
| :---          | :---                                              | :---  |
| `eientei.org` | [matrix.eientei.org](https://matrix.eientei.org/) |       |

### Servers run by Japanese people

| Server                | Web client                                       | Extra |
| :---                  | :---                                             | :---  |
| `matrix.fedibird.com` | [fedibird.com](https://element.fedibird.com/)    | 🏆    |
| `matrix.juggler.jp`   | [juggler.jp](https://matrix-element.juggler.jp/) |       |

Source: [matrix-room-list-jp](https://matrix-room-list-jp.netlify.app/)

### [A list of homeservers](https://web.archive.org/web/20230227042902/https://glowers.club/wiki/doku.php?id=wiki:homeservers) recommended by [Glowers Club](https://web.archive.org/web/20221208070442/https://glowers.club/wiki/doku.php?id=start)
| Server                   | Web client                                          | Extra                    |
| :---                     | :---                                                | :---                     |
| `matrix.thisisjoes.site` | [thisisjoes.site](https://element.thisisjoes.site/) | last checked - closed    |
| `nerdsin.space`          | [nerdsin.space](https://nerdsin.space/)             | last checked - closed 🏆 |

## Do not use

The list contains popular servers that have proven themselves unreliable.
A server is added to this list if it has been caught banning user accounts
or rooms without prior notice.

| Server                         | Information                                                                                                                                   |
| :---                           | :---                                                                                                                                          |
| `waifuhunter.club`             | Admin deactivated users' accounts without prior notice.                                                                                       |
| `matrix.org`                   | Explained above.                                                                                                                              |
| `*.modular.im` or `*.ems.host` | Affiliated with matrix.org.                                                                                                                   |
| `tchncs.de`                    | Admin blocked rooms in pursuit of censorship.                                                                                                 |
| `asra.gr`                      | Admin deactivated users' accounts after receiving fake reports.                                                                               |
| `3000.chat`                    | Admin deactivated users' accounts after receiving fake reports.                                                                               |
| `lolisho.chat`                 | Admin deactivated users' accounts for no apparent reason. Admin leaked IP addresses of some users.                                            |
| `synod.im`                     | Admin deactivated users' accounts for no apparent reason.                                                                                     |
| `utwente.io`                   | Admin deactivated users' accounts for no apparent reason.                                                                                     |
| `envs.net`                     | Admin blocked rooms in pursuit of censorship.                                                                                                 |
| `halogen.city`                 | I used to recommend this server, but our members constantly complained about having trouble joining rooms. On top of that the server is slow. |

A full list that includes less popular servers is available
[here](https://tatsumoto-ren.github.io/matrix/#blocklist).

## Other servers

### Sorted list

I have a sorted list that updates automatically every 12 hours
[here](https://tatsumoto-ren.github.io/matrix/).

Selection criteria.

* Open registration
* Domain length
* Up-to-date version of Synapse

The list is good for fetching new and updated servers,
but there are no guarantees that the results are good.

### Servers that support links to rooms

A separate list for servers that can be used to link rooms.
This is very useful if you want to share a room with someone
but don't want to use `element.io` or `matrix.to` because they are behind cloudflare
or because your room can't be reached via `matrix.to`.

To link a room append `#/room/#your_room:example.com`
to the instance's Element address,
like this: `https://c.wfr.moe/#/room/#djtspace.midov.pl`.

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

### With Element

These servers have
[Element](https://web.archive.org/https://element.io/).
It's a web application that you can use to chat
without having to use a desktop client.

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

### Without Element

These Matrix servers don't offer the web interface,
but you can still register an account.
Install one of the clients listed on
[Arch Wiki](https://wiki.archlinux.org/index.php/List_of_applications#Matrix_clients),
press "create account", then find advanced options
and change the server from the default to the one you want.

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

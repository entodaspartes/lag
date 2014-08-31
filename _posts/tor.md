---
title: ¿Que es Tor?
categories: [navegacion, anonimato]
---

¿Qué es Tor?
============

Tor es un programa que puedes ejecutar en tu computador y te ayuda a mantenerte a salvo en Internet. Tor te protege haciendo "saltar" tu comunicación a través de una red distribuida de retransmisores (relays) que funcionan como túneles virtuales y son ejecutados por voluntarios alrededor del mundo (el set de relays voluntarios es llamado Red Tor). De esta forma, cuando estás dentro de la red, tus datos son enviados a través de estos relays aleatoriamente, haciendo que tu tráfico no pueda ser rastreado en caso de que alguien esté monitoreando tu conexión y a la vez previene que los sitios que visitas conozcan tu ubicación física.

Todo esto también permite que si te encuentras en una región donde la censura prima, puedas librarte de ella en cuanto a la visita de sitios web se refiere. 

**En términos simples, ¿qué es y para qué sirve Tor? ¿quiénes lo utilizan?**  
Es un software que permite “saltar” bloqueos de sitios web y servicios a través de internet. Es fuertemente utilizado en países con estrictas políticas respecto a libertad de expresión, de modo que bloquean cualquier posibilidad de acceder a medios de información que muestra una realidad y opiniones que no quieren que se hagan públicas. También es utilizado por quienes no quieran ser rastreados a través de su conexión tradicional bajo los ojos de su ISP (Proveedor de Servicios de Internet) o simplemente para mantener el anonimato a la hora de navegar por distintos sitios de internet.

**¿Qué es el Tor Browser Bundle?**  
Es un navegador basado en el popular Firefox que viene preconfigurado con utilidades y configuraciones para conectarse automáticamente a la red Tor. Antes de iniciarlo verás otro pequeño programa llamado Vidalia que es quien realmente hace tu conexión hacia la red Tor y luego verás la ventana del navegador.

**¿Mi proveedor de internet puede saber qué estoy buscando y qué sitios he visitado con Tor?**  
No. Tu proveedor tendrá conocimiento hasta que te conectas a la red Tor. Una vez dentro de ella, tu tráfico viaja encriptado (es decir, ilegible para un tercero no involucrado en la comunicación) “y saltando” entre distintos puntos (relays o nodos) de dicha red para que no seas rastreadx.

**¿La empresa que me provee de internet sabrá que estoy usando Tor?**  
Sí. Si tu proveedor de servicios de internet quisiera verificar, podría saberlo haciendo una inspección profunda de paquetes (DPI en inglés) pero es bastante poco probable que lo hagan a no ser que te encuentres en una región como China donde hay altos niveles de censura y control por parte del gobierno. Es decir, díficil, pero lo pueden hacer.. [Acá](https://lists.torproject.org/pipermail/tor-talk/2011-June/020655.html) puedes leer, en inglés, las respuestas de varixs usuarixs sobre el tema. Clickea donde dice "Next message" para leerlas. 

_Nota_: Para evitar que tu proveedor sepa que estás usando Tor, puedes utilizar [obfsproxy](https://www.torproject.org/projects/obfsproxy.html.en). 

**¿Cómo funciona Tor?**  
Como dijimos, Tor se puede entender como una serie de túneles virtuales a través de los cuales viaja la información. A continuación lo explicamos mejor de acuerdo al diagrama que verás abajo: 

![tor](https://github.com/nicht/lag/blob/master/media/tor.png)

Tú eres alicia desde tu computador y accedes a la red Tor a través del Tor-Browser-Bundle que mediante Vidalia te conecta propiamente a la red. Luego, una vez dentro de la red quieres acceder al sitio google.com, como muestra el ejemplo, pero en vez de conectarte directamente (Alicia <-> google.com), pasarás a través de distintos computadores llamados relays  que servirán como túneles por los cuales tu información viaja cifrada (ilegible para terceros). La ventaja de "saltar" entre distintos computadores que corran Tor es que una vez llegando a google.com, éste no podrá conocer tu dirección IP original, pues solo tendrá acceso a la del último punto de la red, conocido como "nodo de salida". Lo anterior permite que tu conexión sea anónima en todo su trayecto.  
Es importante notar cuándo tu información viaja cifrada y cuándo no, y este último punto es crítico. Desde que sale la información de tu computador y pasa por los distintos relays la información está encriptada, sin embargo, entre el último relay y el servidor de destino (google.com) la comunicación es legible y por tanto vulnerable. Para suplir este riesgo es recomendable que siempre utilices HTTPS en los sitios que visites de modo que quede protegida la información en el último punto del trayecto.

**Todo suena muy bien respecto a mi privacidad pero me han dicho que no puedo navegar de la misma forma que sin él, ¿cómo es eso?**  
* Es probable que tu navegación sea un poco más lenta que la que tienes contratada directamente con tu ISP. Tor funciona gracias a la donación de ancho de banda de sus usuarios, así que la velocidad es directamente proporcional con los donantes →["cómo configurar un relay" en caso de que quieras colaborar](https://www.torproject.org/docs/tor-relay-debian.html.en).  
* Tampoco podrás ver vídeos o animaciones en flash.  
* Seguramente si visitas tus cuentas como la de Google o Facebook, te llegarán correos o se te mostrará por pantalla alguna notificación de que alguien en cierto lugar del mundo está intentando acceder a tu cuenta y te pide una verificación de identidad. Cuando ocurre esto te das cuenta que las grandes compañías sí almacenan tu dirección IP desde la que te conectas frecuentemente y cualquier cambio es notado por ellos en seguida.

_Ejemplo_: Supongamos que te conectas a tu cuenta de Facebook desde tu  casa a las 12:00, y luego desde tu lugar de trabajo a las 13:30.  Facebook no detectará nada raro en ello. Sin embargo, supongamos que a  las 14:00 te conectas desde Tor, y Tor te asigna una dirección IP en  Alemania: es físicamente imposible que en media hora hayas viajado a  Alemania. Por lo tanto, Facebook te hará una prueba de reconocimiento  algo engorrosa para asegurarse que quien se conecta eres tú. Facebook es  un ejemplo, pero esto también ocurre con Google, Yahoo! y una serie de  otros servicios corporativos.

**Me queda claro. ¿Algún otro consejo?**  
- No le cambies la configuración por defecto al Navegador Tor ni le agregues plugins (complementos). Tor viene configurado y listo para usar.  
- Descargar torrents a través de algún software como BitTorrent, µTorrent, Deluge, etc. a través de Tor no es una buena idea. Clientes como uTorrent pueden exponer información personal o tu dirección IP y de esto último te puedes dar cuenta que cuando descargas un torrent puedes ver la dirección IP desde donde lo estás bajando. Más info [acá](https://blog.torproject.org/blog/bittorrent-over-tor-isnt-good-idea)  
- No descargues documentos de internet mientras estés navegando en Tor.  Debes tener mucho cuidado si lo haces  (especialmente archivos .DOC y .PDF), ya que estos documentos pueden  contener trampas para revelar tu dirección IP. Si tienes que trabajar  con estos documentos, es muy recomendable usar un ordenador  desconectado, descargando VirtualBox y usándola una imagen de máquina virtual  o usando Tails.
 


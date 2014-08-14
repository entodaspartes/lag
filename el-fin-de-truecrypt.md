
#El fin de TrueCrypt

Hace un par de días la página de TrueCrypt anunciaba sin mayores reparos el fin del desarrollo del proyecto. TrueCrypt era un software de código abierto ampliamente usado para cifrar contenido en unidades de almacenamiento (discos duros, pendrives, tarjetas SD, etc) con la característica de ser multiplataforma. En su mensaje de despedida, recomendaron utilizar las alternativas propias de cada sistema: BitLocker para Windows, FileVault para OS X y cualquier cosa que diga “encryption” y “crypt” en GNU/Linux (como Tomb o LUKS).

El mensaje de inmediato despertó suspicacias y teorías conspirativas alrededor del globo. No es tan raro, porque además de mostrar un sitio web muy simple con letras en rojo, esgrimiendo como excusa el fin del soporte de Windows XP por parte de Microsoft, y además recomendando usar BitLocker (donde existen motivos para creer que tiene fallos de seguridad encargados por la NSA), parecía más el producto de un deface (hackeo) del sitio web.

Aún así, entregaron la versión 7.2 de TrueCrypt. Los ficheros estaban firmados con la misma llave OpenPGP que los anteriores, lo que hizo pensar que, de ser un hackeo, era uno extremadamente bien elaborado.

**Algunos Datos**

TrueCrypt ha estado disponible en internet desde hace unos 10 años, no estando exento de polémicas dentro de los círculos de seguridad. Entre sus principales gracias estaban:

    - Facilidad de uso.
    - Multiplataforma (funciona en Windows, OS X y Linux).
    - Cifrado de disco completo.
    - Al parecer, no hubieron reportes de problemas de seguridad graves con él.
    - Gratis.

**Y sus principales problemas eran:**

    - Anonimato de quienes lo desarrollan. Este problema va desde una cosa tan “simple” como tener a quién consultarle si el mensaje de despedida es real, hasta saber las intenciones que hay detrás de un software.
    - Su seguridad no era puesta a prueba (cosa que estaba cambiando en este tiempo).
    - Si bien el código fuente estaba disponible, era bastante tedioso el crear un ejecutable de él.
    - El desarrollo era a puertas cerradas, lo que ampliaba el desconocimiento de qué había detrás de TrueCrypt.
    - No era software libre.

**Ya, ya, ya, mucha info… Entonces, ¿qué pasó?**

No hay grandes motivos para dudar la veracidad del mensaje: el desconocimiento de quienes estaban detrás de TrueCrypt, como sus intenciones, invalidan cualquier intento de deslegitimarlo al recomendar BitLocker (no, nadie ha dicho que TrueCrypt se creó para enfrentar a la NSA). La firma de los binarios con su llave OpenPGP común solo reafirma la veracidad del mensaje.

TrueCryt lleva 10 años dando vueltas, 10 años de largo trabajo hecho por una o más personas, al parecer sin paga alguna. Es entendible el posible agotamiento de quienes estaban a cargo, hace 2 años que no habían actualizaciones y con pruebas de seguridad al software. Si encontraban fallos, estos debían ser arreglados, lo que significa tiempo y más trabajo. Si no hay ánimos, lo correcto en estos casos es cortar con el programa.

Pero que TrueCrypt deje de desarrollarse no significa que del día a la mañana sea inseguro -o al menos más inseguro que ayer-, pero sí que dejará de tener mantenimiento y que, por ende, hay que buscar nuevas alternativas pensando en el mañana y no en el hoy.

**Resumiendo:**

**¿Está TrueCrypt muerto?**
Sí, el software dejó de ser desarrrollado.

**¿Hay fallas graves de seguridad en TrueCrypt?**
No que se conozcan.

**Si yo uso Windows, ¿debo ahora usar BitLocker?**
Si quieres proteger tu información de un ladrón, probablemente funcione. Si quieres proteger tu información de una institución como el Estado o una corporación, no suena tan buena idea. Lo mejor es usar otro sistema operativo, como Linux, que contiene programas de encriptado más recomendables como Tomb o LUKS.

**¿Entonces?**
TrueCrypt aún funciona, pero llegará un momento en donde la versión actual sea tan antigua, que no será muy segura. Si necesitas proteger información sensible, lo más lógico es usar Linux. Si no deseas instalarlo puedes usar una distribución como Tails (sistema operativo que puede ser usado conectando un CD o un pendrive), con soporte de cifrado en pendrives y otros. Si esta no es tu opción, puedes seguir utilizando la versión 7.1 de TrueCrypt y estar pendiente de las noticias, en especial porque se seguirá haciendo el análisis de su seguridad aún cuando el proyecto haya sido abandonado.

**¿Puede alguien retomar TrueCrypt?**
Sí y no. Sí porque, si bien la licencia de TrueCrypt no lo permite, es difícil que alguien vaya a salir de su anonimato para entablarle una demanda a alguien que decida continuar desarrollando TrueCrypt, así que es factible. No, porque como  quienes desarrollaron el proyecto han expresado por contacto, sólo ellxs entienden el código, por lo que retomarlo puede generar más problemas que hacerlo de 0.

**Ufff, qué terrible todo esto…**
No, es más una buena oportunidad para hacer las cosas bien. TrueCrypt no era perfecto, tenía varios problemas y ahora es la ocasión de solucionarlos.

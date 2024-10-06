El propósito de este complemento consiste en proporcionar una solución que permita revisar el funcionamiento de diversas tablas braille con rapidez en NVDA, sin necesidad de sobrescribir las que ya vienen incluidas en el núcleo. De esta forma, se pueden hacer modificaciones en una tabla, probar de manera sencilla el resultado, y proponer cambios en el [repositorio de Liblouis](https://github.com/liblouis/liblouis), llegado el caso.

## Modo de uso

El complemento no dispone de atajos de teclado ni interfaz gráfica. Una vez instalado, ve al menú NVDA, Preferencias, Opciones, Braille, y elige una de las tablas experimentales en los cuadros combinados "Tabla de salida" y "Tabla de entrada". A continuación, trabaja con el braille como lo harías normalmente y evalúa el comportamiento de la tabla elegida. A menos que se indique lo contrario, todas las tablas proporcionadas soportan entrada y salida.

Desde la carpeta de instalación del complemento, puedes editar cualquiera de las tablas con un editor de texto plano, como Notepad++, reiniciar NVDA y probar los cambios en tiempo de ejecución. Si NVDA está instalado en tu equipo, no necesitarás privilegios de administrador, como ocurriría al reemplazar los archivos de tabla en el núcleo del programa.

Si has hecho un cambio que quieres compartir con otros usuarios, contacta con nosotros por la <a href="mailto:nvda-es@googlegroups.com">lista de correo de NVDA en español</a> o abriendo un <a href="mailto:soporte@nvda.es">ticket de soporte</a>, y publicaremos una nueva versión. También admitimos incidencias y pull requests.

## Evaluación de tablas sin una pantalla braille

Las pantallas braille, y especialmente aquellas con teclado, no tienen un precio que se pueda considerar adecuado para todos los bolsillos. No obstante, existen un par de complementos con los que no las echaremos de menos, y que se pueden descargar desde la tienda integrada en NVDA:

* [Entrada braille a través del teclado del pc](https://nvda.es/2017/10/19/entrada-braille-traves-del-teclado-del-pc-nvda/): en su configuración por defecto, las teclas f, d, s y a actuarán como los puntos 1, 2, 3 y 7, mientras que las teclas j, k, l y ñ serán los puntos 4, 5, 6 y 8. Configura el complemento a tu gusto, activa el teclado braille con los atajos disponibles, y escribe. El complemento transcribirá tus pulsaciones usando la tabla de entrada que hayas seleccionado.
* [Unicode Braille Input](https://nvda.es/2017/10/18/unicode-braille-input/): este es el complemento que necesitas para convertir texto a braille. Ve al menú NVDA, Herramientas, y elige Unicode Braille Input. Teclea el texto que deseas transcribir, elige en los botones de opción que hay a continuación tu tabla, y pulsa Aceptar. El resultado se copiará al portapapeles. Puedes pegarlo, o simplemente escucharlo pulsando NVDA+c. Cada uno de los caracteres devueltos se leerá como una secuencia de puntos en braille.

## Tablas braille incluidas

Inicialmente, este complemento ha sido diseñado para ayudar en el mantenimiento de las tablas braille en español. Por ese motivo, se ha elegido el español como su idioma base, y sólo se incluyen las siguientes tablas:

* Español computerizado de 8 puntos.
* Español grado 1 (6 puntos).
* Español grado 2 (braille contraído).
* Español para textos en griego clásico.
* Catalán grado 1.

## Registro de cambios

Se espera que este complemento tenga un ciclo de publicación de versiones bastante dinámico, por lo que no incluiremos un registro de cambios aquí. Puedes consultar los cambios de todas las versiones desde la [página de releases](https://github.com/nvda-es/experimentalBrailleTables/releases). Si instalas el complemento [Display Addons Changelog](https://github.com/javidominguez/displayAddonsChangelog), de Javi Domínguez, recibirás un mensaje con los cambios de cada actualización justo mientras se instala.

## Notas a tener en cuenta

* Para evitar un solapamiento entre las tablas incluidas en NVDA y las que aporta este complemento, estas últimas se han renombrado añadiendo el sufijo "experimental" antes de la extensión del archivo. En algunos casos ha sido necesario modificarlas internamente para que las sentencias `include` coincidan.
* En las opciones de braille de NVDA, las tablas experimentales se encuentran justo al final de la lista, y no se ordenan alfabéticamente junto a las demás.
* Si usas Braille Extender, deberás deshabilitarlo antes de elegir las tablas de este complemento. De lo contrario, la línea braille se quedará en blanco y el teclado dejará de funcionar. Es posible que el autor resuelva este conflicto en próximas versiones.

### Hi there 👋

###Trabajo a realizar
1. Este debe tener una pequeña descripción tuya tipo CV.
Añade una tabla en Markdown (Obviamente) con al menos 5 comandos de la
Terminal que hayas aprendido, de forma que tenga nombre del comando y
descripción en columnas separadas.
2.
Añade una sección con al menos 2 comandos alias que te parezcan útiles
incluyendo columna de descripción.
3.
4. (Opcional) Clona tu repositorio y ejecuta 11ty como en la practica.
---

## Acerca de Mí
---
¡Hola! Soy Ulises Argueta, un apasionado de la tecnología, la realidad virtual y aumentada. Mi objetivo es aprender y explorar el emocionante mundo de la tecnología y las posibilidades que ofrece.

En el ámbito de las artes marciales, soy un cinturón azul en taekwondo y desempeño un papel como instructor de apoyo. Además, soy un principiante en BJJ (Brazilian Jiu-Jitsu) y tengo un gran interés en las artes marciales mixtas.

Me fascina la convergencia de la tecnología y la creatividad para dar vida a proyectos sorprendentes y hermosos. Actualmente, estoy participando en el bootcamp de Undefined Academy, dirigido por Guillermo Rodas, para desafiarme a aprender aún más.

¡Vamos juntos en este viaje de aprendizaje y exploración tecnológica!

## Comandos de la Terminal de Linux
---
| Comandos | Descripcion                     |
|----------|---------------------------------|
| cp -r    | sirve para copiar recursivamente|
|touch     |Crea un archivo nuevo segun ruta |
|cat       |Imprime el contenido de una ruta.|
|mv        |mover archivo o carpeta y cambiar nombre|

> Cuando utilizas mv para cambiar la ubicación o el nombre de un archivo o directorio, estás modificando estos metadatos. No modificando  El contenido real del archivo o directorio (los datos en sí) no se altera; solo se actualiza la información que el sistema de archivos utiliza para localizar y gestionar ese elemento.

## Alias utiles
| Alias                | Funcion                         |
|----------------------|---------------------------------|
|alias rm= "trashh"    | Todo lo que se elimina entra en papelera|
|alias cl = "Clear"    |Limpia la terminal               |
#### guardar alias permanente
> **Bash** se hace en el archivo **.bashrc**
> **~Shell** debe hacerse en **.zshrc**
>
> `` Echo $SHEELL`` para saber que *SHELL* se tiene

# 40 Comandos de linux mas utilizados
<details>
<summary>Click para desplegar la lista</summary>
 1. Comando sudo
Abreviatura de superusuario do, sudo es uno de los comandos básicos más populares de Linux que te permite realizar tareas que requieren permisos administrativos o de root.

Al utilizar sudo, el sistema pedirá a los usuarios que se autentiquen con una contraseña. A continuación, el sistema Linux registrará una marca de tiempo como seguimiento. Por defecto, cada usuario root puede ejecutar comandos sudo durante 15 minutos por sesión.

Si intentas ejecutar sudo en la línea de comandos sin autenticarte, el sistema registrará la actividad como un evento de seguridad.

Esta es la sintaxis general:

sudo (comando)

También puedes añadir una opción, por ejemplo:

-k o -reset-timestamp invalida el archivo timestamp.
-g o -group=group ejecuta comandos como un nombre o ID de grupo especificado.
-h o -host=host ejecuta comandos en el host.
2. Comando pwd
Utiliza el comando pwd para encontrar la ruta de tu directorio de trabajo actual. Simplemente introduciendo pwd te devolverá la ruta actual completa, una ruta de todos los directorios que comienza con una barra oblicua (/). Por ejemplo, /inicio/nombredeusuario.

El comando pwd utiliza la siguiente sintaxis:

pwd [opción]

Tiene dos opciones aceptables:

-L o -logical imprime el contenido de las variables de entorno, incluidos los enlaces simbólicos.
-P o -physical imprime la ruta real del directorio actual.
3. Comando cd
Para navegar por los archivos y directorios de Linux, usa el comando cd. Te pedirá la ruta completa o el nombre del directorio, dependiendo del directorio de trabajo actual en el que te encuentres.

Supongamos que estás en /home/nombredeusuario/Documentos y deseas ir a Fotos, un subdirectorio de Documentos. Para hacerlo, simplemente escribe el siguiente comando:

cd Fotos.

Otro escenario es si deseas ir a un directorio completamente nuevo, por ejemplo, /home/nombredeusuario/Peliculas. En este caso, debes escribir cd seguido de la ruta absoluta del directorio:

cd /home/nombredeusuario/Peliculas.

Hay algunos atajos para ayudarte a navegar rápidamente:

cd ~[nombredeusuario] para ir directamente a la carpeta de inicio.
cd .. para ir un directorio hacia arriba.
cd- para ir al directorio anterior.
4. Comando ls
El comando ls se usa para ver el contenido de un directorio. Por defecto, este comando mostrará el contenido de tu directorio de trabajo actual.

Si deseas ver el contenido de otros directorios, escribe ls y luego la ruta del directorio. Por ejemplo, para ver el contenido de la carpeta Documentos ingresa:

ls/inicio/nombredeusuario/Documentos

Hay variaciones que puedes usar con el comando ls:

ls -R también listará todos los archivos en los subdirectorios.
ls -a mostrará los archivos ocultos.
ls -al listará los archivos y directorios con información detallada como los permisos, el tamaño, el propietario, etc.
5. Comando cat
cat (abreviatura de concatenate, en inglés) es uno de los comandos más utilizados en Linux. Este lista, combina y escribe el contenido de los archivos en la salida estándar. Para ejecutar este comando, escribe cat seguido del nombre del archivo y su extensión. Por ejemplo:

cat archivo.txt.

Aquí hay otras formas de usar el comando cat:

cat > nombredearchivo.txt crea un nuevo archivo.
cat nombredearchivo1.txt nombredearchivo2.txt>nombredearchivo3.txt fusiona nombrearchivo1.txt y nombrearchivo2.txt y almacena el resultado en nombrearchivo3.txt.
tac nombrearchivo.txt muestra el contenido en orden inverso.
6. Comando cp
Utiliza el comando cp para copiar archivos o directorios y su contenido. Echa un vistazo a los siguientes casos de uso.

Para copiar un archivo del directorio actual a otro, introduce cp seguido del nombre del archivo y del directorio de destino. Por ejemplo:

cp nombrearchivo.txt /inicio/nombredeusuario/Documentos

Para copiar archivos en un directorio, introduce los nombres de los archivos seguidos del directorio de destino:

cp nombrearchivo1.txt nombrearchivo2.txt nombrearchivo3.txt /inicio/nombredeusuario/Documentos

Para copiar el contenido de un fichero a otro nuevo en el mismo directorio, introduce cp seguido del fichero de origen y del fichero de destino:

cp nombrearchivo1.txt nombrearchivo2.txt

Para copiar un directorio completo, pasa el indicador -R antes de escribir el directorio de origen, seguido del directorio de destino:

cp -R /inicio/nombredeusuario/Documentos /inicio/nombredeusuario/Documentos_backup

# 7. Comando mv
El uso principal del comando mv es mover archivos, aunque también se puede usar para cambiar el nombre de los archivos. Además, no produce ninguna salida al ejecutarlo.

Simplemente escribe mv seguido del nombre del archivo y el directorio de destino. Por ejemplo, si quieres mover nombredearchivo.txt al directorio /inicio/nombredeusuario/Documentos:

mv nombrearchivo.txt /inicio/nombredeusuario/Documentos.

También puedes utilizar el comando mv para renombrar un archivo:

mv nombre_archivo_antiguo.txt nombre_archivo_nuevo.txt

# 8. Comando mkdir
Utiliza el comando mkdir para crear uno o varios directorios a la vez y establecer los permisos para cada uno de ellos. El usuario que ejecuta este comando debe tener el privilegio de crear una nueva carpeta en el directorio principal o puede recibir un error de permiso denegado.

Esta es la sintaxis básica:

mkdir [opción] nombre_directorio

Por ejemplo, si deseas crear un directorio llamado Música:

mkdir Musica

Para crear un nuevo directorio llamado Canciones dentro de Música, utiliza este comando:

mkdir Musica/Canciones

El comando mkdir acepta muchas opciones, como:

-p o -parents crean un directorio entre dos carpetas existentes. Por ejemplo, mkdir -p Musica/2020/Canciones creará el nuevo directorio «2020».
-m establece los permisos del archivo. Por ejemplo, para crear un directorio con todos los permisos de lectura, escritura y ejecución para todos los usuarios, introduce mkdir -m777 nombre_directorio.
-v imprime un mensaje para cada directorio creado.
9. Comando rmdir
Para eliminar permanentemente un directorio vacío, utiliza el comando rmdir. Recuerda que el usuario que ejecuta este comando debe tener privilegios sudo en el directorio padre.

Por ejemplo, si deseas eliminar un subdirectorio vacío llamado personal1 y su carpeta principal mydir:

rmdir -p mydir/personal1

# 10. Comando rm
El comando rm se utiliza para borrar archivos dentro de un directorio. Asegúrate de que el usuario que ejecuta este comando tiene permisos de escritura.

Recuerda la ubicación del directorio ya que esto eliminará el/los archivo(s) y no podrás deshacerlo.

Esta es la sintaxis general:

rm nombredearchivo

Para eliminar varios archivos, introduce el siguiente comando:

rm nombredearchivo1 nombredearchivo2 nombredearchivo3

Aquí tienes algunas opciones aceptables que puedes añadir:

-i pide confirmación al sistema antes de borrar un archivo.
-f permite al sistema eliminar sin confirmación.
-r borra archivos y directorios de forma recursiva.
11. Comando touch
El comando touch permite crear un archivo vacío o generar y modificar una marca de tiempo en la línea de comandos de Linux.

Por ejemplo, introduce el siguiente comando para crear un archivo HTML llamado Web en el directorio Documentos:

touch /inicio/nombredeusuario/Documentos/Web.html

# 12. Comando locate
El comando locate puedes encontrar un archivo en el sistema de base de datos.

Además, si añades el argumento -i, desactivará la distinción entre mayúsculas y minúsculas, por lo que podrás buscar un archivo aunque no recuerdes su nombre exacto.

Para buscar contenidos que contengan dos o más palabras, utiliza un asterisco (*). Por ejemplo:

locate -i escuela*nota

El comando buscará los archivos que contengan las palabras escuela y nota, tanto si utilizan mayúsculas como minúsculas.

# 13. Comando find
Utiliza el comando find para buscar archivos dentro de un directorio específico y realizar operaciones posteriores. Ésta es la sintaxis general:

find [opción] [ruta] [expresión]

Por ejemplo, quieres buscar un archivo llamado notas.txt dentro del directorio inicio y sus subcarpetas:

find /inicio -name notas.txt

Aquí tienes otras variaciones al utilizar find:

find -name nombredearchivo.txt para buscar archivos en el directorio actual.
find ./ -type d -name nombredeldirectorio para buscar directorios.
14. Comando grep
Otro comando básico de Linux en la lista es grep o impresión global de expresiones regulares. Te permite encontrar una palabra buscando entre todos los textos de un archivo específico.

Una vez que el comando grep encuentra una coincidencia, imprime todas las líneas que contienen el patrón específico. Este comando ayuda a filtrar archivos de registro de gran tamaño.

Por ejemplo, si deseas buscar la palabra azul en el archivo notepad.txt:

grep azul notepad.txt

La salida del comando mostrará las líneas que contengan azul.

# 15. Comando df
Utiliza el comando df para informar sobre el uso del espacio en disco del sistema, mostrado en porcentaje y en kilobytes (KB). Esta es la sintaxis general:

df [opciones] [archivo]

Por ejemplo, introduce el siguiente comando si deseas ver el uso del espacio en disco del sistema del directorio actual en un formato legible para personas:

df -h

Estas son algunas variaciones:

df -m muestra información sobre el uso del sistema de archivos en MBs.
df -k muestra el uso del sistema de archivos en KBs.
df -T muestra el tipo de sistema de archivos en una nueva columna.
16. Comando du
Si quieres comprobar cuánto espacio ocupa un archivo o un directorio, utiliza el comando du. Gracias a este comando puedes identificar qué parte del sistema utiliza excesivamente el almacenamiento.

Recuerda que debes especificar la ruta del directorio cuando utilices el comando du. Por ejemplo, para comprobar /inicio/usuario/Documentos introduce:

du /inicio/usuario/Documentos

Añadiendo una bandera al comando du se modificará la operación, como por ejemplo:

-s ofrece el tamaño total de una carpeta especificada.
-m proporciona información sobre carpetas y archivos en MB.
k muestra la información en KB.
-h informa de la última fecha de modificación de las carpetas y archivos mostrados.
17. Comando head
El comando head permite ver las diez primeras líneas de un texto. Añadiendo una opción se puede cambiar el número de líneas mostradas. El comando head también se utiliza para dar salida a datos canalizados a la CLI.

Esta es la sintaxis general:

head [opción] [archivo]

Por ejemplo, si quieres ver las diez primeras líneas de nota.txt, situado en el directorio actual:

head nota.txt

A continuación te indicamos algunas opciones que puedes añadir:

-n o -lines imprime el primer número personalizado de líneas. Por ejemplo, introduce head -n 5 nombredearchivo.txt para mostrar las cinco primeras líneas de nombredearchivo.txt.
-c o -bytes imprime el primer número personalizado de bytes de cada archivo.
-q o -quiet no imprimirán cabeceras que especifiquen el nombre del archivo.
18. Comando tail
El comando tail muestra las diez últimas líneas de un archivo. Permite a los usuarios comprobar si un archivo tiene datos nuevos o leer mensajes de error.

Este es el formato general:

tail [opción] [archivo]

Por ejemplo, si deseas ver las diez últimas líneas del archivo colores.txt:

tail -n colores.txt

19. Comando diff
Abreviatura de diferencia, el comando diff compara dos contenidos de un archivo línea por línea. Tras analizarlos, mostrará las partes que no coincidan.

Los programadores suelen utilizar el comando diff para modificar un programa en lugar de reescribir todo el código fuente.

Este es el formato general:

diff [opción] archivo1 archivo2

Por ejemplo, si deseas comparar dos archivos de texto: nota.txt y actualización_nota.txt:

diff nota.txt actualizacion_nota.txt

Aquí algunas opciones aceptables para añadir:

-c muestra la diferencia entre dos archivos en un formulario contextual.
-u muestra la salida sin información redundante.
-i hace que el comando diff no distinga entre mayúsculas y minúsculas.
20. Comando tar
El comando tar archiva múltiples ficheros en un fichero TAR, un formato común de Linux similar a ZIP, con compresión opcional.

Esta es la sintaxis básica:

tar [opciones] [fichero_archivo] [fichero o directorio a archivar]

Por ejemplo, si deseas crear un nuevo archivo TAR llamado nuevoarchivo.tar en el directorio /Inicio/nombredeusuario/Documentos:

tar -cvf nuevoarchivo.tar /inicio/nombredeusuario/Documentos

El comando tar acepta muchas opciones, como:

-x extrae un archivo.
-t lista el contenido de un archivo.
-u archiva y añade a un fichero de archivo existente.
21. Comando chmod
chmod es un comando común que modifica los permisos de lectura, escritura y ejecución de un archivo o directorio. En Linux, cada archivo está asociado a tres clases de usuarios: propietario, miembro de grupo y otros.

Esta es la sintaxis básica:

chmod [opción] [permiso] [nombre_archivo]

Por ejemplo, el propietario es actualmente el único con permisos completos para modificar nota.txt. Para permitir que los miembros del grupo y otras personas lean, escriban y ejecuten el archivo, cámbialo al tipo de permiso -rwxrwxrwx, cuyo valor numérico es 777:

chmod 777 nota.txt

Este comando permite muchas opciones, entre ellas

-c o -changes muestra información cuando se realiza un cambio.
-f o -silent suprimen los mensajes de error.
-v o -verbose muestra un diagnóstico para cada archivo procesado.
22. Comando chown
El comando chown permite cambiar la propiedad de un archivo, directorio o enlace simbólico a un nombre de usuario específico.

Este es el formato básico:

chown [opción] propietario[:grupo] archivo(s)

Por ejemplo, si quieres que usuariodelinux2 sea el propietario de nombredearchivo.txt:

chown usuariodelinux2 nombredearchivo.txt

# 23. Comando jobs
Un job es un proceso que el shell inicia. El comando jobs mostrará todos los procesos en ejecución junto con sus estados. Recuerda que este comando sólo está disponible en los shells csh, bash, tcsh y ksh.

Esta es la sintaxis básica:

jobs [opciones] jobID

Para comprobar el estado de los trabajos en el shell actual, basta con introducir jobs en la CLI.

Aquí tienes algunas opciones que puedes utilizar:

-l lista los ID de proceso junto con su información.
-n enumera los trabajos cuyo estado ha cambiado desde la última notificación.
-p lista sólo los ID de proceso.
24. Comando kill
Utiliza el comando kill para terminar manualmente un programa que no responde. Este señalará a las aplicaciones que se comporten mal y les indicará que cierren sus procesos.

Para acabar un programa, debes conocer su número de identificación de proceso (PID). Si no conoces el PID, ejecuta el siguiente comando:

ps ux

Después de saber qué señal utilizar y el PID del programa, introduce la siguiente sintaxis:

kill [opcion_señal] pid

Hay 64 señales que puedes utilizar, pero estas dos son de las más utilizadas:

SIGTERM solicita a un programa que deje de ejecutarse y le da algo de tiempo para guardar todo su progreso. El sistema lo utilizará por defecto si no se especifica la señal al introducir el comando kill.
SIGKILL fuerza a los programas a detenerse y perderás el progreso no guardado.
Por ejemplo, el PID del programa es 63773 y quieres forzarlo a detenerse:

kill SIGKILL 63773

25. Comando ping
El comando ping es uno de los comandos esenciales de Linux más utilizados para comprobar si se puede acceder a una red o a un servidor. Además, se utiliza para solucionar diversos problemas de conectividad.

Este es el formato general:

ping [opción] [nombre_de_host_o_dirección_IP]

Por ejemplo, si quieres saber si puedes conectarte a Google y medir su tiempo de respuesta:

ping google.com

26. Comando wget
La línea de comandos de Linux te permite descargar archivos de Internet mediante el comando wget. Este funciona en segundo plano sin entorpecer otros procesos en ejecución.

El comando wget recupera archivos utilizando los protocolos HTTP, HTTPS y FTP. También puede realizar descargas recursivas, que transfieren partes de sitios web siguiendo estructuras de directorios y enlaces, creando versiones locales de las páginas web.

Para utilizarlo, introduce el siguiente comando:

wget [opción] [url]

Por ejemplo, si introduces el siguiente comando para descargar la última versión de WordPress:

wget https://wordpress.org/latest.zip

27. Comando uname
El comando uname o unix name imprimirá información detallada sobre tu sistema Linux y tu hardware. Esto incluye el nombre de la máquina, el sistema operativo y el kernel. Para ejecutar este comando, simplemente introduce uname en tu CLI.

Esta es la sintaxis básica:

uname [opción]

Estas son las opciones aceptables:

-a imprime toda la información del sistema.
-s imprime el nombre del núcleo.
-n imprime el nombre de host del nodo del sistema.
28. Comando top
El comando top en el Terminal de Linux mostrará todos los procesos en ejecución y una vista dinámica en tiempo real del sistema actual. Este resume la utilización de recursos, desde la CPU hasta el uso de memoria.

El comando top también puede ayudarte a identificar y terminar un proceso que pueda utilizar demasiados recursos del sistema.

Para ejecutar el comando, basta con introducir top en la CLI.

29. Comando history
Con history, el sistema listará hasta 500 comandos ejecutados previamente, permitiéndote reutilizarlos sin necesidad de volver a entrar. Ten en cuenta que sólo los usuarios con privilegios sudo pueden ejecutar este comando. La ejecución de esta utilidad también depende del shell de Linux que utilices.

Para ejecutarlo, introduce el siguiente comando:

history [opción]

Este comando admite muchas opciones, como:

-c borra toda la lista del historial.
-d offset borra la entrada del historial en la posición OFFSET.
-a añade líneas de historial.
30. Comando man
El comando man proporciona un manual de usuario de cualquier comando o utilidad que pueda ejecutar en Terminal, incluyendo el nombre, la descripción y las opciones.

Consta de nueve secciones:

Programas ejecutables o comandos de shell
Llamadas al sistema
Llamadas a la biblioteca
Juegos
Expedientes especiales
Formatos de archivo y convenciones
Comandos de administración del sistema
Rutinas del núcleo
Varios
Para visualizar el manual completo, introduce:

man [nombre_comando]

Por ejemplo, si quieres acceder al manual del comando ls:

man ls

Introduce este comando si deseas especificar la sección mostrada:

man [opción] [número_sección] [nombre_comando]

Por ejemplo, si quieres ver la sección 2 del manual del comando ls:

man 2 ls

31. Comando echo
El comando echo es una utilidad integrada que muestra una línea de texto o cadena utilizando la salida estándar. Esta es la sintaxis básica:

echo [opción] [cadena]

Por ejemplo, puede mostrar el texto Tutoriales Hostinger introduciendo:

echo «Tutoriales Hostinger»

Este comando admite muchas opciones, como:

-n muestra la salida sin la línea final.
-e permite la interpretación de las siguientes barras invertidas:
\a reproduce la alerta sonora.
\b elimina los espacios entre un texto.
\c no produce más salida.
-E muestra la opción por defecto y desactiva la interpretación de las barras invertidas.
32. Comandos zip y unzip
Utiliza el comando zip para comprimir tus archivos en un archivo ZIP, un formato universal de uso común en Linux. Puedes elegir automáticamente la mejor proporción de compresión.

El comando zip también es útil para archivar ficheros y directorios, y reducir el uso del disco.

Para utilizarlo, introduce la siguiente sintaxis:

zip [opciones] archivozip archivo1 archivo2….

Por ejemplo, si tienes un archivo llamado nota.txt que deseas comprimir en archivo.zip en el directorio actual:

zip archivo.zip nota.txt

Por otro lado, el comando unzip extrae los ficheros comprimidos de un archivo. Este es el formato general:

unzip [opción] nombre_archivo.zip

Así, para descomprimir un archivo llamado archivo.zip en el directorio actual, introduce:

unzip archivo.zip

33. Comando hostname
Ejecuta el comando hostname para conocer el nombre de host del sistema. Puedes ejecutarlo con o sin opción. Esta es la sintaxis general:

hostname [opción]

Hay muchas banderas opcionales para usar, incluyendo:

-a o -alias muestra el alias del nombre de host.
-A o -all-fqdns muestra el nombre de dominio completo de la máquina (FQDN).
-i o -ip-address muestra la dirección IP de la máquina.
Por ejemplo, introduce el siguiente comando para conocer la dirección IP de tu ordenador:

hostname -i

34. Comando useradd y userdel
Linux es un sistema multiusuario, lo que significa que más de una persona puede utilizarlo simultáneamente. useradd se utiliza para crear una nueva cuenta, mientras que el comando passwd permite añadir una contraseña. Sólo aquellos con privilegios de root o sudo pueden ejecutar el comando useradd.

Cuando utilizas el comando useradd, este realiza algunos cambios importantes:

Edita los archivos /etc/passwd, /etc/shadow, /etc/group y /etc/gshadow para las cuentas recién creadas.
Crea y rellena un directorio personal para el usuario.
Establece los permisos y la propiedad de los archivos en el directorio personal.
Esta es la sintaxis básica:

useradd [opcion] nombredeusuario

Para establecer la contraseña:

passwd la_combinación_contraseña

Por ejemplo, para añadir una nueva persona llamada Juan, introduce simultáneamente el siguiente comando:

useradd Juan

passwd 123456789

Para eliminar una cuenta de usuario, utiliza el comando userdel:

userdel nombredeusuario

35. Comando apt-get
apt-get es una herramienta de línea de comandos de Linux para gestionar las bibliotecas de Advanced Package Tool (APT) en Linux. Permite recuperar información y paquetes de fuentes autenticadas para gestionar, actualizar, eliminar e instalar software y sus dependencias.

Para ejecutar el comando apt-get es necesario utilizar privilegios sudo o de root.

Esta es la sintaxis principal:

apt-get [opciones] (comando)

Estos son los comandos más comunes que puedes añadir a apt-get:

update sincroniza los archivos del paquete desde sus fuentes.
upgrade instala la última versión de todos los paquetes instalados.
check actualiza la caché de paquetes y comprueba las dependencias rotas.
36. Comandos nano, vi y jed
Linux permite a los usuarios editar y gestionar archivos mediante un editor de texto, como nano, vi o jed. nano y vi vienen con el sistema operativo, mientras que jed hay que instalarlo.

El comando nano denota palabras clave y puede funcionar con la mayoría de los idiomas. Para utilizarlo, introduce el siguiente comando:

nano [nombredearchivo]

vi utiliza dos modos de funcionamiento para trabajar: insertar y comando. insertar se utiliza para editar y crear un archivo de texto. Por otro lado, comando realiza operaciones, como guardar, abrir, copiar y pegar un archivo.

Para utilizar vi en un archivo, introduce:

vi [nombredearchivo]

jed tiene una interfaz de menús desplegables que permite a los usuarios realizar acciones sin necesidad de introducir combinaciones o comandos de teclado. Al igual que vi, dispone de modos para cargar módulos o plugins para escribir textos específicos.

Para abrir el programa, basta con introducir jed en la línea de comandos.

37. Comandos alias y unalias
alias te permite crear un acceso directo con la misma funcionalidad que un comando, nombre de archivo o texto. Cuando se ejecuta, indica al shell que sustituya una cadena por otra.

Para utilizar el comando alias, introduce esta sintaxis:

alias Nombre=Cadena

Por ejemplo, si quieres hacer k el alias para el comando kill:

alias k=’kill’

Por otro lado, el comando unalias borra un alias existente.

La sintaxis general es la siguiente:

unalias [nombre_alias]

38. Comando su
El comando switch user o su permite ejecutar un programa como un usuario diferente. Este cambia la cuenta administrativa en la sesión de inicio de sesión actual. Este comando es especialmente beneficioso para acceder al sistema a través de SSH o utilizando el gestor de pantalla GUI cuando el usuario root no está disponible.

Esta es la sintaxis general del comando:

su [opciones] [nombredeusuario [argumento]]

Cuando se ejecuta sin ninguna opción o argumento, el comando su se ejecuta con privilegios de root. Te pedirá que te autentiques y utilices los privilegios sudo temporalmente.

Aquí algunas opciones aceptables:

-p o -preserve-environment mantiene el mismo entorno de shell, formado por HOME, SHELL, USER y LOGNAME.
-s o -shell te permite especificar un entorno shell diferente para ejecutar.
-l o -login ejecuta un script de inicio de sesión para cambiar a un nombre de usuario diferente. Ejecutarlo requiere que introduzcas la contraseña del usuario.
39. Comando htop
El comando htop es un programa interactivo que monitoriza los recursos del sistema y los procesos del servidor en tiempo real. Está disponible en la mayoría de las distribuciones de Linux y puedes instalarlo con el gestor de paquetes predeterminado.

Comparado con el comando top, htop tiene muchas mejoras y funciones adicionales, como el manejo con ratón e indicadores visuales.

Para utilizarlo, ejecuta el siguiente comando:

htop [opciones]

También puedes añadir opciones, como:

-d o -delay muestra el retardo entre actualizaciones en décimas de segundo.
-C o -no-color activa el modo monocromo.
-h o -help muestra el mensaje de ayuda y la salida.
40. Comando ps
El comando de estado de procesos o ps produce una instantánea de todos los procesos en ejecución en tu sistema. Los resultados estáticos se toman de los archivos virtuales del sistema de archivos /proc.

Ejecutando el comando ps sin una opción o argumento listará los procesos en ejecución en el shell junto con:

El identificador único del proceso (PID).
El tipo de terminal (TTY).
El tiempo de funcionamiento (TIME).
El comando que lanza el proceso (CMD).
Aquí tienes algunas opciones aceptables que puedes utilizar:

-T muestra todos los procesos asociados a la sesión de shell actual.
-u nombredeusuario lista los procesos asociados a un usuario específico.
-A o -e muestra todos los procesos en ejecución.
</details>
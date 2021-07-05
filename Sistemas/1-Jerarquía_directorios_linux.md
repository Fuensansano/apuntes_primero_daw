# Estructura de directorios de GNU/linux
Sigue el estándar FHS. Se completo en 1995.

![estrucura de directorios](https://i2.wp.com/nexolinux.com/wp-content/uploads/2013/04/fhs1-e1365160570150.png)

## /
**Carpeta raíz**, de esta parten todas las demás.

## bin/
Aquí se guardan los ficheros binarios/ejecutables de los programas. Los pueden ejecutar todos los usuarios del sistema

## boot/
archivos que se encargan del arranque del ordenador, es el que se encarga de decirle al equipo cual es la partición que tiene que arrancar. Los kernal se suelen almacenar en este directorio.

## sbin/
Los binarios que se encuentran en este drectorio solo los puede ejecutar el super usuario.

## lib/
un conjunto de operaciones o instrucciones que permiten al programa poder ejecutar unas características. Aquí también se guardan los módulos de kernel.

## usr/
Guarda las mayoría de los datos de programa de una aplicación.

## usr/local/
subdirectorio de usr/ guarda ficheros de aplicaciones que se instalan de forma local.

## opt/
Almacena aplicaiones que son de software de terceros. ajenos a la distribución.

## home/
carpeta descarga, imagenes, personalización de cada usuario. (Más de cada usuario).

## root/
Es el home del superusuario.

## var/
Contiene **datos variables**, datos vivos, como un log de sistemas o log de servicios. Por ejemplo, un servidor web apache, quien se conecta a él, etc.

## tmp/
Se almacenan datos temporales y se limpian cada vez que se apaga el ordenador.

## mnt/
alberga el montaje de los dispositivos. Aquí aparecen las aplicaciones de los periféricos.

## media/
Aqui se montan los dispositivos  específicos tales como discos extraibles, usbs...

**Diferencia entre media/ y mnt/**
Ambos se encargan del montaje del dispositivo pero media se emplea para el montajende dispositivos físicos y mnt para los montajes de unidades en red.

## dev/
Contiene punteros de memoria que van asociados a los dispositivos físicos que tenemos en el equipo y que necesita el sistema operativo para trabajar.

## proc/
Contiene un sistema de ficheros virtual que proporciona acceso a ciertos tipos de información del hardware dinamicamente.
Ejemplo: estado CPU, estado de la RAM, etc.

## srv/
datos para los servicios provistos por este sistema.




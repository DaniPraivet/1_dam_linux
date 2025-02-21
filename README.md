# 1_dam_linux


### Particiones
`cfdisk` -> editor + visualizador de particiones <br>
<br>
`fdisk` -> visualizar particiones <br>
`fdisk -l` -> lista de las particiones <br>
`fdisk -l /dev/sda` -> ver datos del primer disco <br> 
`fdisk -l /dev/sda2` -> ver datos del primer disco, segunda partición <br>
<br>
### Mostrar información
`who` -> quien está conectado al sistema <br>
`who -a` -> muestra la fecha de arranque del sistema<br>
<br>
`whoami` -> muestra el nombre de usuario<br>
<br>
`uname`<br>
`uname --all`<br>
`uname --nodename`<br>
`uname -r`<br>
`uname -v`<br>
<br>
`lsb_release`<br>
`lsb_release -i` -> id del distribuidor<br>
`lsb_release -d` -> descripción<br>
`lsb_release -r` -> numero de version<br>
`lsb_release -c` -> nombre de la versión<br>
`lsb_release -idrc` -> todo lo anterior<br>
<br>
### Usuarios 
`useradd` -> añadir usuarios via terminal <br>
`useradd -m <nombre de usuaro>` -> crear un `/home` para el usuario `<nombre de usuario>`<br>
`useradd -e 2025-03-22 <nombre de usuario>` <br> <br>

`sudo cat /etc/passwd | grep "<nombre de usuario>"` -> para mostrar el usuario que quieras <br><br>
`passwd <nombre de usuario>` -> cambiar contraseña del usuario <br>
`passwd <nombre de usuario> -d` -> Eliminar la contraseña<br>
`passwd <nombre de usuario> -l` -> Bloquear cuenta<br>
`passwd <nombre de usuario> -u` -> Desbloquear cuenta<br>
`passwd <nombre de usuario> -e` -> Fecha de expirar cuenta <br><br>
`exit` -> cerrar sesión o salir de la terminal<br><br>
`reboot` -> reiniciar<br><br>
`shutdown` -> apagar o pausar el equipo<br>
`shutdown -H` -> pausar el sistema
`shutdown -p` -> por defecto
`shutdown -r` -> lo mismo que reboot
`shutdown -c` -> cancelar
 ### Gestión de archivos y ficheros
`adduser` -> crear usuario al sistema
`adduser --system usuariosistema` -> crear usuario del sistema
`adduser --uid 1010 usuario2` -> crear usuario con un uid específico
`adduser --home <ruta de la carpeta /home>` -> crear usuario con una carpeta /home en una ruta específica

`deluser` -> eliminar usuario del sistema
`deluser --remove-home` -> eliminar carpeta del usuario
`deluser --remove-all-files` -> eliminar todos los archivos pertenecientes al usuario

`usermod` -> modificar cuenta de usuario
`usermod -d` -> cambiar directorio personal del usuario 
`usermod -m` -> mueve los contenidos del directorio
``

`addgroup` -> añadir un grupo al sistema
`addgroup --system` -> añade grupo al sistema
`addgroup --gid` -> le pone un id específico

`delgroup` -> eliminar grupo del sistema
`delgroup --only-if-empty` -> lo elimina solo si no tiene ningún usuario

`groupmod` -> modifica el grupo de usuarios
`groupmod -g` -> cambias el id del grupo
`groupmod -n` -> modifica el nombre del grupo


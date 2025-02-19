# 1_dam_linux


### Particiones
`cfdisk` -> editor + visualizador de particiones <br>
<br>
`fdisk` -> visualizar particiones <br>
`fdisk -l` -> lista de las particiones <br>
`fdisk -l /dev/sda` -> ver datos del primer disco <br> 
`fdisk -l /dev/sda2` -> ver datos del primer disco, segunda partición <br>
<br>
### Usuarios
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

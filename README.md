# script_docker

Para ejecutar script debe situarse en la ubicación donde se encuentra y ejecutar la siguiente línea:

$ ./dockeer.sh

En caso de no funcionar por falta de permisos, ejecutar la siguiente línea:

$ chmod +x dockeer.sh

En caso de no tener instalado Curl, ejecutar la siguiente línea:

$ sudo apt install curl

#####################################################

Para comprobar si el usuario es miembro de docker debe volver a loguear, utilice la siguiente línea:

$ su -l $USER
#Luego utilizar $id para comprobar los grupos
#Deberia obtener algo asi: "uid=1000(punkblock) gid=1000(punkblock) groups=1000(punkblock),4(adm),24(cdrom),27(sudo),30(dip),46(plugdev),116(lpadmin),126(sambashare),999(docker)"

Para checkear version de Docker y Docker-compose instaladas, ejecutar las siguientes líneas:

docker -v
#Deberia obtener algo asi: "Docker version 18.09.6, build 481bc77"
docker-compose -v
#Deberia obtener algo asi: "docker-compose version 1.24.0, build 0aa59064"

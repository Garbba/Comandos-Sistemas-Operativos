# Comandos Sistemas Operativos 💻

Jeremy García Baltodano

Universidad Latinoamericana de Ciencia y Tecnología

ULACIT

2022

**Comandos**

ps ⮕ Estático.
ps -aux ⮕ Procesos de mi usuario.
ps -e ⮕ Procesos de mi sistema operativo.
htop ⮕ Dinámico, va cambiando, mejor interfaz gráfica.
top ⮕ Dinámico, va cambiando.
pstree ⮕ Muestra árbol y rutas de procesos.
ip addr --> ip 
ls --> listar contenido de una carpeta o directorio
ls -l --> modo lista
| --> concatenar los comandos
grep --> busquedas de texto
ps -aux | grep "firefox"
mkdir --> crear carpetas
pwd --> saber donde estoy
sudo adduser <name miniscula>--> crear un nuevo usuario 
sudo passwd --> cambiar la contraseña a un usuario.
sudo userdel <nombre usuario> --> borrar un usuario
su <nombre usuario> --> me cambio a otro usuario
whoami --> que usuario soy
exit --> salgo de la sesion
nano <archivo> --> ver y editar archivos
cat --> ver contenido de un archivo
history --> ver comandos
history > <name archivo> -->  me guarda todo en ese archivo nuevo
head/tail -n <numero de lineas> <nombre del arhcivo> --> me muestra el numero de lineas que quiera
cat <archivo name> | more --> scroll down el archivo
cp <archivo a copiar> <lugar donde vamos a copiar> --> copiar archivo
mv <archivo a moverr> <lugar donde vamos a mover> --> mover archivo
rm o mv -R <archivo a borrar> --> borrar archivos
mv -R o mv -Rf (f es de forzado) <directorio a borrar> --> borrar directorio
du -h <archivo> --> ver los metadatos
du -h <archivo> --> ver los metadatos
stat <archivo> --> ver metados
file <archivo> --> de que formato es un archivo
df - h --> ver archivos montados
gparted --> administrar particiones
gnome-disk-utility --> info sobre el disco duro
testdisk --> para recuperar archivos borrados!
export var="valor" --> para crear una variable
docker image rm <nombre>
docker ps -a --> los contenedores que yo cree y estan corriendo
docker pull <aplicacion o image a instalar>
Una vez instalado usamos el comando: 
sudo docker run -it <archivo> --> crea un nuevo contenedor
sudo docker start<container id> --> va a iniciar un contenedor que esta detenido
sudo docker attach <container id>
docker stats --> me enseña cuanta memoria esta consumiendo el container 
El -d es modo detached, voy a crear un contenedor pero no voy a entrar a la terminal del ubuntu, solo dejar un servicio corriendo.
docker run -d -p 80:80 -p 3306:3306 tutum/lamp
El -p es para abrir un puerto del contenedor en nuestra maquina virtual
Crear otro contenedor de ubuntu
sudo docker run -it -p 9090:80 --name mi_ubuntu ubuntu
cp -rv <ubicacion>[letras]* <nueva direccion> -->copiar archivos que inicien con cierta letra de forma recursiva

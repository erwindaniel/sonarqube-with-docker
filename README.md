# sonarqube-with-docker
# how run sonarqube in a docker container - Como ejecutar sonarqube en un contenedor docker

Laejecucion se realiza con docker compose en un servidor linux con docker engine instalado.

1. Instalar docker compose:

 **sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose**

 cambiar por la version mas reciente
 
 permisos de ejecucion :
 
 **sudo chmod +x /usr/local/bin/docker-compose**
 
2. Ejecutar:

**sudo sysctl -w vm.max_map_count=262144**
**sudo chown $USER /var/run/docker.sock**

3. Copiar el archivo docker-compose.yml en un directorio de eleccion y ejecutar
   
   **docker-compose up**
4. Abrir en un navegador la url:
   **http://ipDeMiServidorLinux:9000**
   
6. Cambiar la contraseña por defecto
   
   Al ingresar por primera vez pedirá cambio de contraseña
   
   **El usuario y contraseña por defecto es admin, cambiarlo por otro de eleccion y listo ya queda nuestro Sonarqube para hacer analisis estático**



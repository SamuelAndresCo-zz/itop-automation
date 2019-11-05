# itop-automation
En este espacio de trabajo se subiran las memorias del trabajo de grado de la automatización de la instación de la herramienta de gestión IT Itop

# Acerca de este Repositorio
Este es un repositorio de Git para la imagen de Docker con la herramienta de gestión Itil Itop. 

# Requisitos 
1. Instalación de Docker. Para obtenerlo dirigirse al link https://hub.docker.com/. Docker puede ejecutarse sobre distintos Sistemas Operativos (Mac, Windows, Linux). Para el caso de Windows es necesario tener la versión Enterprise (No funcionara con la versión HOME).
2. Es necesario crear un usuario (Ejemplo: itopudistrital)

3. Instalación de Docker en Ubuntu

   1. Antes de iniciar la instalación ejecutar el comando
      sudo apt-get update
   2. Asegurarse de remover versión anteriores
      sudo apt-get remove docker docker-engine docker.io
   3. Instalar Docker
      sudo apt install docker.io
   4. Iniciar Docker
      sudo systemctl start docker
   5. Probar que Docker quedo bien instalado
      docker --version 
      Debe salir en consola la versión de Docker instalada    
4. Posterior a la instalación de Docker. Se debe agregar el 
    1. Para ejecutar comandos en docker sin necesidad de utilizar "Sudo" se debe dar permisos al usuario para ejecutar Docker
       sudo groupadd docker
    2. Agregar el usuario 
       sudo usermod -aG docker $USER
    3. Activar los cambios sobre el usuario
        newgrp docker 
    4. Comando para verificar que podemos ejecutar  
       docker run hello-world

# Ejecución de Docker itop
   1. Descargar el repositorio: git clone git@github.com:SamuelAndresCo/itop-automation.git
   2. Abrir la terminal de comandos y ejecutar el "docker build -t udistrital/itop ." Este comando ejecutara el archivo dockerfile y           creara la imagen llamada udistrital/itop. **El nombre udistrital/itop puede ser reemplazado por cualquier otro
   3. Ejecutar el comando docker images ps y verificar que se liste la imagen udistrital/itop
   4.
   
   
      

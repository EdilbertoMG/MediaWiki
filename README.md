## Diseño
<img src="https://raw.githubusercontent.com/edil-gutierrez/MediaWiki/master/MediaWiki%20Diagrama.png" />

## Preliminares
Para realizar las prácticas debes tener instalado en el equipo o servidor de pruebas:
  - Docker
  - Python

#### Instalación de Ansible

        pip install ansible

### Construcción de la imagen personalizada
Ingresa a la carpeta ```Dockerfile``` y sigue los pasos indicados.

-------------------------------------------

### Luego de hacer los pasos en la carpeta Dockerfile haga lo siguiente: 
Ejecute los siguiente comandos:
``` 
ansible-playbook -i hosts Mysql.yml
```
```
ansible-playbook -i hosts Apache.yml
```
```
ansible-playbook -i hosts MediaWiki.yml
```
NOTA: en el Diseño se muestra que el servidor web sera nginx pero en la practica se opto por utilizar apache2
-------------------------------------------

Documentación de lo que se hizo
-------------------------------------------
En acuerdo a como se solicitó en la actividad de instalación de Mediawiki en su última versión, se plantearon las siguientes dudas.

### ¿Cómo crear los contenedores de Docker? 
Para poder crear los contenedores se optó por hacer un ```Dockerfile```, para crear la imagen que es la que nos permitirá hacer los contenedores y un archivo de autorización.

### ¿Cómo realizar la instalación automatizando mediante Ansible? 
Dentro de los contenedores los cuales llamaremos ```web_server``` y ```mysql_server```.

Dentro de estos 2 contenedores se instalarán los roles dado de la siguiente manera: 
```-	Apache y MediaWiki dentro del contenedor web_server.
   -	MySql dentro del contenedor mysql_server.
```
Luego de haber realizado toda esta guía paso a paso ya se podrá ingresar al puerto que quedo abierto para ingresar por el navegador que es el 8080.


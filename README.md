## Diseño
<img src="https://raw.githubusercontent.com/edil-gutierrez/MediaWiki/master/MediaWiki%20Diagrama.pngf" />

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
Ejecute los siguiente comandos
``` 
ansible-playbook -i hosts Mysql.yml
```
```
ansible-playbook -i hosts Apache.yml
```
```
ansible-playbook -i hosts MediaWiki.yml
```

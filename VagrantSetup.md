# Setup de la máquina virtual

## Pasos previos
Comprobamos que tenemos instalados los paquetes necesarios ejecutando los siguientes comandos:
```bash
$ gh --version
$ vagrat --version
$ autojump --version
$ tree --version
```
Creamos la estructura de directorios necesaria.
```bash
~/Documentos/
├── RLO    
    └── VM
```
Copiamos el fichero _Vagrantfile_ de la carpeta compartida a nuestra carpeta VM.

Vamos a la carpeta _VM_ y editamos con el editor de textos _SublimeText_ el fichero _Vagrantfile_
```bash
subl Vagrantfile
```
Modificamos las líneas 48 y 49 adaptándolas a nuestro caso:
```bash
      :bridge => "xxx",
      :ip => "192.168.xx.xxx"    
```
## Clonar repositorio
Clonamos el repositorio necesario para iniciar la máquina virtual. Nos vamos a la carpeta _VM_ y ejecutamos el comando 
```bash
$ gh repo clone SMR-RAL/vm-init
```
Si es la primera vez que utilizamos la aplicación _gh_ deberemos autenticarnos en _github_. utiliza el comando 
```bash
$ gh auth login
```
## Autojump
Autojump es una 

## Servicios Internos
### Simple ServerMail con Docker

### Pre-requisitos 📋

_Opcional tener instalado make para automatizar algunos comandos_
```
$ sudo apt install make
$ sudo apt install build-essential 
```
_Se debe tener instalado docker_

[https://linuxconfig.org/how-to-install-docker-on-ubuntu-18-04-bionic-beaver][https://linuxconfig.org/how-to-install-docker-on-ubuntu-18-04-bionic-beaver]

Es opcional dry, pero sirve para ver algunas cosas de docker ya funcionando

[https://github.com/moncho/dry][https://github.com/moncho/dry]

Para usuarios de Windows 10 estos son los enlaces para instalar Docker.
Es importante tener la versión 2004.
Se puede actualizar desde:

[https://www.microsoft.com/es-es/software-download/windows10][https://www.microsoft.com/es-es/software-download/windows10]


Esta es el enlace con las instrucciones:

[https://medium.com/@fred.gauthier.dev/web-development-environment-with-wsl-2-and-docker-for-symfony-5860704e127a][https://medium.com/@fred.gauthier.dev/web-development-environment-with-wsl-2-and-docker-for-symfony-5860704e127a]


#### Uso de docker

> Para la construcción del contenedor
```
make build
```
> Para lanzar el contenedor
```
make run
```
> Para parar el contenedor
```
make stop
```


#### Configuración 
Sf 2.8

```
mail_mailer: smtp
mail_host: 172.21.0.2
mail_port: 1025
mail_username: null
mail_password: null
mail_encryption: null
mail_auth: null
```


SF 4.4
```
MAILER_DSN=smtp://null:null@172.21.0.2:1025
```

#### Visualización

[http://localhost:1080](http://localhost:1080)


## Servicios Internos
### Simple ServerMail con Docker

#### Pasos Previos
> Se debe tener docker instalado
> El comando make también tiene que estar instalado
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


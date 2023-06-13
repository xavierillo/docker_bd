# Requisitos


* mysql:8.0 Docker

# Usando Docker
---


## Inicialización de imagen en docker


### 1. Versión rápida

```
docker compose up --build -d
```

* Build = Geneara la imagen a partir de los archivos de configuración
* D = Agrega el contenedor a background (daemon)

### 2. Versión detallada
```
docker-compose build app
docker-compose up -d
```

## Conexión BD

 `HOST = 127.0.0.1 | db
 USER = root 
 PASSWORD = toor`

Si se utiliza el contenedor docker de intranet, se debe agregar lo siguiente `DB_HOST=db` para señalar a docker que se utilizará el servicio DB de la red intranet.


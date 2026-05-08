# README - Bitácora IV Sistemas Informáticos I

## El objetivo principal es desplegar una infraestructura basada en contenedores Docker y practicar conexiones remotas 
La práctica incluye generación de claves SSH, autenticación segura y acceso remoto a un entorno Ubuntu gráfico.


# Requisitos Previos

Necesitamos tener descargado docker, creamos el documento docker-compose 

Levantamis el contenedor con docker-compose up -d
posteriormente  verificamos con docker p

Deberían aparecer:

- Un servidor SSH
- Un entorno gráfico Ubuntu
- Servicio web Apache Guacamole

# Configuración SSH

Entramos en la powershell e introducimos ssh alberto@localhost -p 2222

La contraseña es sistemas_informaticos



## Generamos la identidad

Desde la máquina anfitriona:

ssh-keygen -t ed25519 -C albertorueda.25@campuscamara.es

---

## Transferir la clave pública

ssh-copy-id -p 2222 alberto@localhost
y aceptamos
# Acceso Remoto mediante RDP

## Conexión desde cliente RDP


## localhost:3000
Abrimos esto en google y observamos nuestro escritorio d ubuntu

creamos el archivo de texto indicado PRUEBA_LOGRADA.txt y finalizamos el proceso




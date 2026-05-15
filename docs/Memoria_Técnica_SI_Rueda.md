# MEMORIA TÉCNICA DE LA BITÁCORA 4

### ALBERTO RUEDA ROMERO
### 1º DAW
### 15 DE MAYO DE 2026

# Índice

1. Introducción  

2. Infraestructura Utilizada  

3. Configuración SSH  

4. Acceso Remoto con Guacamole  

5. Análisis de Necesidades  

6. Conclusión  

# 1. Introducción

En esta práctica vamos a analizar las necesidades para la empresa con guacamole, docker , ssh y ubuntu

# 2. Infraestructura Utilizada

La infraestructura utilizada está formada por varios contenedores Docker:

- Servidor SSH

- Ubuntu gráfico

- Apache Guacamole

- Ubuntu

Todos los servicios fueron desplegados utilizando el archivo `docker-compose.yml`.

# 3. Configuración SSH

Se configuró el acceso remoto mediante SSH usando claves públicas.

Los pasos realizados fueron:

1. Conexión inicial mediante contraseña.

2. Generación de claves SSH.

3. Copia de la clave pública al servidor.

4. Acceso seguro sin contraseña.

El acceso se realizó mediante el puerto `2222`.

# 4. Acceso Remoto con Guacamole

Apache Guacamole permite acceder al escritorio remoto desde el navegador web.

La conexión se realizó desde:

`http://localhost:3000`

También se utilizó el puerto `3389` para conexiones RDP.

Para comprobar el funcionamiento del sistema se creó el archivo `PRUEBA_LOGRADA.txt` dentro del escritorio remoto.

# 5. Análisis de Necesidades

La empresa necesitaba una solución que permitiera a los trabajadores acceder de forma remota a distintos equipos y servicios de manera segura y sencilla. Antes de implementar esta infraestructura, cada ordenador debía configurarse individualmente para permitir conexiones remotas mediante RDP o SSH. Esto suponía varios problemas relacionados con la seguridad, el mantenimiento y la administración de los sistemas.


Uno de los principales inconvenientes era la necesidad de abrir varios puertos en la red para permitir las conexiones externas. Cuantos más puertos abiertos existen, mayor es el riesgo de sufrir ataques o accesos no autorizados. Además, cada usuario necesitaba instalar programas específicos para conectarse remotamente, lo que complicaba todavía más el trabajo y aumentaba el tiempo necesario para configurar nuevos equipos.






# 6. Conclusión


La práctica permitió aprender el uso de Docker, SSH y Apache Guacamole para crear una infraestructura remota segura y organizada.

La solución implementada mejora la seguridad, facilita el acceso remoto y simplifica la administración de los servicios.


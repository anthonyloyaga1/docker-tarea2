# Nexcloud

Este proyecto contiene la configuración para desplegar nextcloud utilizando las imágenes:  
- nextcloud:31.0-apache
- redis:8.2-alpine
- mariadb:11.4

## Grupo 5
- Roberto Maldonado
- David Saa
- Anthony Loyaga
- Nelson Lopez

## Requisitos

- Docker Engine
- Navegador web

## Instalación y Configuración

### 1. Verificando archivo docker-compose.yml

Se creó el archivo docker-compose.yml usando las imágenes antes indicadas

```bash
nano docker-compose.yml
```

<img width="886" height="23" alt="image" src="https://github.com/user-attachments/assets/fe40b7d2-f740-4987-a995-f4f1b8438b9b" />


### 2. Ejecutando archivo docker-compose.yml

Ejecutar en segundo plano (detached mode) el archivo archivo docker-compose.yml

```bash
docker compose up -d
```

<img width="886" height="283" alt="image" src="https://github.com/user-attachments/assets/5285dafa-96d3-4240-b48c-2605695dcf27" />


### 3. Verificar los contenedores

Para verificar que todos los contenedores estén ejecutándose correctamente:

```bash
docker compose ps
```

<img width="886" height="99" alt="image" src="https://github.com/user-attachments/assets/8f450ae7-6c8e-41d5-a853-1eeef6885c04" />


### 4. Verificar en el navegador

1. Abre el navegador web
2. Ingresar la rul `http://localhost`

<img width="886" height="779" alt="image" src="https://github.com/user-attachments/assets/e4365b0f-cf71-477f-849b-201bcf936865" />


### Post Implementación: Detener y eliminar contenedores + volúmenes

```bash
docker compose down -v
```

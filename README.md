# Práctica 7: Dockerización, Auditoría y Logging (Django REST API)

Proyecto backend desarrollado con **Django REST Framework**, **PostgreSQL** y **Docker**, que incorpora registro de eventos técnicos y de auditoría, autenticación JWT con trazabilidad de IP y documentación mediante Swagger.

## 🚀 Características principales
* **Contenedorización completa:** Orquestación de servicios con `Docker Compose` (`api-rest-django` y `api-rest-postgres`).
* **Sistema de Auditoría y Logs:** Captura de eventos críticos (`LOGIN_EXITOSO`, `LOGIN_FALLIDO`) con registro de dirección IP y detalles del usuario.
* **Documentación interactiva:** Swagger UI y ReDoc integrados mediante `drf-yasg` con soporte para autenticación Bearer (JWT).
* **Seguridad y CORS:** Configuración de cabeceras y control de acceso para peticiones externas.

## 🛠️ Requisitos previos
* Docker y Docker Compose instalados en tu sistema.
* Python 3.11+ (para desarrollo local opcional).

---

## 🛠️ Instrucciones de Configuración y Ejecución

Sigue estos pasos en tu terminal para poner a marchar el proyecto en tu equipo local:

### 1. Clonar el repositorio
```bash
git clone [https://github.com/TS-UAM26O-JMVH/p07_django.git](https://github.com/TS-UAM26O-JMVH/p07_django.git)
cd p07_django/proyectos_django/django4/proyecto_django/back_end_django
```

### 2. Activar el entorno virtual
```bash
source venv/bin/activate
```

### 2.1 Cómo desactivar el entorno virtual
Para salir del entorno virtual y regresar a la terminal normal del sistema, simplemente ejecuta:
```bash
deactivate
```
### 3 Construye y levanta los contenedores en segundo plano:
```bash
docker compose up -d --build
```
### 3.1 como detener la base de datos de Docker
Cuando termines de trabajar y desees apagar el contenedor de PostgreSQL de forma limpia, ejecuta el siguiente comando en la misma ruta donde se encuentra tu docker-compose.yml:
```bash
sudo docker compose down
```
### 3.1 Para detener el servidor de desarrollo de django
para detener el servidor en cualquier momento presiona en la terminal:
```
Ctrl +  C
```
---

### 4 la aplicacion disponible en la direccion:
```
http://localhost:8000/swagger/
```
## 👨‍💻 Autor

Desarrollado por Juan Valentin.



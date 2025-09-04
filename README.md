# test-alquiler-video
Este proyecto implementa una API REST para una tienda virtual de videos (venta-alquiler), construida con lenguaje Python y el Framework FastAPI. El objetivo es gestionar un catálogo de discos (películas o videos digitales) junto con las operaciones de registro de usuarios, ventas y alquiler.

## Estructura del Proyecto
|--Main.py #Punto de entrada de la aplicación de la API, FastAPI
|
  entidades/  #Directorio de paquetes que contiene todas las clases
    |- __init__.py
    |- disco.py
    |- usuario.py
    |- venta.py
    |- alquiler.py
    |- catalogo.py

## Instalación y ejecución
  1. Clonar el repositorio
     git clone https://github.com/usuario/test-alquiler-video.git
  2. cd test-alquiler-video
  3. Crear y activar entorno virtual (opcional, recomendado)
  4. python -m venv venv
  5. source venv/bin/activate  #Linux/Mac
  6. venv\Scripts\activate     #Windows
  7. instalar dependencia
     7.1. pip install fastapi uvicorn pydantic
  8. Ejecutar el servidor
     8.1. uvicorn main:app --reload
  9. Acceder a la API
      * Documentación interactiva: http//127.0.0.1:8000/docs
      * Documentación interactiva (ReDoc): http://127.0.0.1:8000/redoc

## Endpoints principales (versión inicial)
Metodo Endpoint       Descripción
GET    /discos/       Lista los discos disponibles
POST   /discos/       Agregar un nuevo disco
PUT    /discos/{id}   Actualizar información de un disco
DELETE /discos/{id}   Eliminar el disco
POST   /usuarios/     Registro de nuevo usuario
POST   /ventas/       Registrar ventas
POST   /alquileres/   Registrar un alquiler

## Tecnologías utilizadas
* Python 3.12.8
* FastAPI
* Uvicorn (Servidor ASGI)

## Proyecto desarrollado como casa de estudio
* Nombre: **Emely Moreno
* Github: Morenrz

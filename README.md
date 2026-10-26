# Proyecto Django — Pesqueira Gamez, Manuel Angel

## Cómo correrlo localmente
1. Crear y activar un entorno virtual
2. pip install -r requirements.txt
3. Copiar .env.example a .env y completar con credenciales propias de Aiven
4. python manage.py migrate
5. python manage.py runserver

## Evidencia
Ver capturas de `migrate` y de las tablas en Aiven en la carpeta /evidencias.

## Prueba de la aplicación
Se probo el aislamiento de la aplicación creando dos usuarios independientes al
super usuario. Creamos dos servicios en cada uno y verificamos que estos no
aparecieran en el servicio de otro usuario.

Tambien nos tratamos de saltar el aislamiento manualmente forzando la url sin embargo
recibimos un error 404 confirmando el total aislamiento por usuario.
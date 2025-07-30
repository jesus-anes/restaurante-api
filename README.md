# API de Restaurantes

Este proyecto es una API RESTful sencilla para gestionar restaurantes, desarrollada con Symfony 7 y desplegada con Docker. Incluye frontend básico, documentación automática y base de datos MySQL.

## 🚀 Tecnologías

- PHP 8.2 + Symfony
- MySQL 8
- Docker y Docker Compose
- Composer
- NelmioApiDocBundle (documentación Swagger)

## 📦 Requisitos

- Docker
- Docker Compose

## 🔧 Instalación

```bash
git clone https://github.com/jesus-anes/restaurante-api.git
cd proyecto-api

# Inicia los contenedores
docker-compose up --build -d

# Accede al contenedor para ejecutar migraciones
docker exec -it nombre-contenedor-app bash
php bin/console doctrine:migrations:migrate

# Microservices Project

Este proyecto utiliza microservicios gestionados con Git Submodules y Docker.

## Instrucciones

1. **Clonar el repositorio**:
   ```bash
   git clone <repository_url>
   ```

2. **Crear archivo `.env`** basado en `.env.template`.

3. **Inicializar submódulos**:
   ```bash
   git submodule update --init --recursive
   ```

4. **Construir y ejecutar con Docker**:
   ```bash
   docker-compose up --build
   ```

## Uso de Submódulos

1. **Añadir un submódulo**:
   ```bash
   git submodule add <repository_url> <directory_name>
   git add .
   git commit -m "Add submodule"
   git push
   ```

2. **Actualizar submódulos**:
   ```bash
   git submodule update --remote
   ```

## ⚠️ Nota Muy Importante

Cuando trabajes con submódulos (que son otros **repositorios**):

- **Actualiza y haz push primero en los submódulos**, luego en el repositorio principal.
- Si haces push primero en el repositorio principal, podrías perder las referencias del submódulo y generar conflictos.

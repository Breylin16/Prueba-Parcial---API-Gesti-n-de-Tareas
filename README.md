# Gestor de Estudiantes - API con Notion

Este proyecto es una API desarrollada en Node.js con Express que permite gestionar un registro de estudiantes almacenado en una base de datos de Notion.

## Funcionalidades
- **Consultar estudiantes**: Obtiene la lista de estudiantes registrados en Notion.
- **Agregar estudiantes**: Permite registrar un nuevo estudiante con su matrícula, nombre y calificaciones.
- **Editar datos**: Modifica un campo específico de un estudiante.
- **Eliminar estudiantes**: Archiva un estudiante en Notion.
- **Eliminar un campo**: Establece en 0 un campo específico (asistencia, prácticas, etc.).

## Requisitos
- Node.js instalado
- Una base de datos en Notion
- Variables de entorno configuradas (`.env`):
  - `NOTION_TOKEN`: Token de acceso a Notion.
  - `NOTION_DATABASE_ID`: ID de la base de datos de Notion.
  - `PORT`: Puerto en el que se ejecutará el servidor (opcional).

## Instalación y uso
1. Clona el repositorio.
2. Instala las dependencias con:
   ```sh
   npm install
   ```
3. Configura el archivo `.env` con tus credenciales de Notion.
4. Ejecuta el servidor:
   ```sh
   npm start
   ```
5. La API estará disponible en `http://localhost:3000` (o el puerto configurado).

## Endpoints principales
- `GET /estudiantes` → Obtiene la lista de estudiantes.
- `POST /agregar` → Agrega un estudiante.
- `PATCH /editar` → Modifica un campo de un estudiante.
- `DELETE /eliminar` → Archiva un estudiante.
- `PATCH /eliminar-campo` → Resetea un campo específico.

#### Breylin Sanchez


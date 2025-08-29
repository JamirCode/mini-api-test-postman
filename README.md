# Mini Proyecto API Test - Javi

Este proyecto es un ejemplo simple de **API Testing con Postman**, usando la API pública [JSONPlaceholder](https://jsonplaceholder.typicode.com), que permite practicar solicitudes REST sin necesidad de configurar un servidor propio.

## 🚀 Objetivo
Demostrar conocimientos básicos de **pruebas de API** con Postman:
- Enviar requests (GET, POST, PUT, DELETE)
- Validar respuestas con tests automáticos en Postman
- Documentar y compartir la colección

## 📂 Contenido del repositorio
- `MiniProyectoAPI.postman_collection.json` → Colección exportada lista para importar en Postman.
- `README.md` → Explicación del proyecto.

## 🔧 Requests incluidos
La colección incluye pruebas básicas de CRUD sobre la ruta `/posts` de JSONPlaceholder:

1. **GET All Posts** → Obtiene todos los posts y valida que la respuesta sea un array.
2. **GET Post by ID** → Obtiene un post específico y valida que tenga propiedades como `userId` y `title`.
3. **POST Create Post** → Crea un nuevo post y valida que el status sea `201` y que se genere un `id`.
4. **PUT Update Post** → Actualiza un post existente y valida que el título se haya modificado.
5. **DELETE Post** → Elimina un post y valida que el status code sea `200` o `204`.

## 🛠️ Tecnologías usadas
- [Postman](https://www.postman.com/) para la ejecución de requests y validación.
- [JSONPlaceholder](https://jsonplaceholder.typicode.com/) como API de prueba pública.

## ▶️ Cómo usar este proyecto
1. Descargar este repositorio o clonar con:
   ```bash
   git clone https://github.com/tu-usuario/mini-api-test-postman.git
   ```
2. Abrir Postman.
3. Importar el archivo `MiniProyectoAPI.postman_collection.json`.
4. Ejecutar los requests individualmente o en conjunto.

## 📌 Notas
- JSONPlaceholder es una API **falsa** (mock), por lo tanto, los cambios de `POST`, `PUT` o `DELETE` no persisten realmente, pero sí devuelven respuestas simuladas que permiten practicar.
- Este proyecto está pensado como **demo simple para entrevistas**, mostrando que manejo las bases de API Testing con Postman.

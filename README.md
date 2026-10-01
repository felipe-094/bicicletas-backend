# Carrito de Compras — Backend 🚲⚙️

API REST desarrollada en Node.js que sirve el catálogo de productos (bicicletas) consumido por el [frontend](https://github.com/felipe-094/bicicletas-frontend) de este proyecto.

## Descripción

Backend sencillo que se conecta a una base de datos MySQL y expone un endpoint para consultar los productos disponibles en la tienda.

## Tecnologías utilizadas

- Node.js
- Express
- MySQL (mysql2)
- Nodemon (entorno de desarrollo)
- dotenv (variables de entorno)

## Endpoints

| Método | Ruta         | Descripción                          |
|--------|--------------|---------------------------------------|
| GET    | `/productos` | Devuelve el listado completo de productos |

## Variables de entorno

Crea un archivo `.env` en la raíz del proyecto (no se sube al repositorio) con las siguientes variables:

```
DB_HOST=localhost
DB_USER=tu_usuario
DB_PASSWORD=tu_contraseña
DB_NAME=productos_en_vivo
PORT=4000
```

> Ajusta los nombres según cómo estén definidas en tu `database.js`.

## Cómo ejecutar el proyecto

1. Clona este repositorio:
   ```bash
   git clone https://github.com/felipe-094/bicicletas-backend.git
   ```
2. Instala las dependencias:
   ```bash
   npm install
   ```
3. Crea el archivo `.env` con tus credenciales de MySQL (ver sección anterior).
4. Asegúrate de tener la base de datos `productos_en_vivo` creada con su tabla `producto`.
5. Inicia el servidor en modo desarrollo:
   ```bash
   npm run dev
   ```
6. El servidor quedará escuchando en `http://localhost:4000`.

## Estructura del proyecto

```
back/
├── src/
│   ├── database.js
│   └── index.js
├── .env (no incluido, debes crearlo)
├── .gitignore
├── package.json
└── package-lock.json
```

## Autor

**Luis Felipe Balanta Quintero**
Desarrollador Fullstack (React, Node.js)

- GitHub: [@felipe-094](https://github.com/felipe-094)
- LinkedIn: [Felipe Quintero](https://www.linkedin.com/in/felipe-quintero-8b99812a1/)

## Proyecto relacionado

- [Frontend del carrito de compras](https://github.com/felipe-094/bicicletas-frontend)

# Proyecto Restaurante Dinely

Proyecto final para la asignatura de Programación. Sitio web para restaurante ficticio creado con Astro e implementado con Strapi y TailwindCSS.

## ¡IMPORTANTE!

Este proyecto utilizó Inteligencia Artificial únicamente para la extensión de párrafos de los blogs y la creación de imágenes para los productos. En términos de código, se utilizó para resolver el tema de llamar relaciones desde Astro a Strapi, como "categoría":

`category={item.tipos?.[0]?.tipo ?? 'General'}`

En general el resto del proyecto debería estar libre de IA.

## Configuración Para Iniciar el Proyecto

Luego de clonar el proyecto, se debe crear un archivo llamado `.env` en la carpeta raiz del proyecto (`/backend-restaurant`), escribiendo lo siguiente dentro de su contenido:

```env
HOST=0.0.0.0
PORT=1337
APP_KEYS=H+xk3zfybj3BhzQ0roMgtw==,haE0z6LlWnjiTuVpQCHLzg==,k8C5t6IV+OOBBK0liQslIg==,HE8FJ2E/dvoEvJnJ81/Bhg==
API_TOKEN_SALT=n+v5tVkANO311nIt8+zGfw==
ADMIN_JWT_SECRET=GAz+LZzPkOzRFlhTuHDD2w==
TRANSFER_TOKEN_SALT=O+jKdFSB9eNfcZLOOGCeKw==
ENCRYPTION_KEY=nugBbi2goRTBgS2HZunzbw==
DATABASE_CLIENT=postgres
DATABASE_HOST=ep-super-mouse-actb6a9d-pooler.sa-east-1.aws.neon.tech
DATABASE_PORT=5432
DATABASE_NAME=restaurantbackend
DATABASE_USERNAME=neondb_owner
DATABASE_PASSWORD=npg_bILTM2zNOwD3
DATABASE_SSL=true
DATABASE_FILENAME=
JWT_SECRET=JeGhekMYsOIvvcbceKcL9Q==
```
Seguidamente de crear este archivo, se debe abrir una nueva terminal y ejecutar los siguientes comandos:

npm install

npm run develop

El proyecto correrá en http://localhost:1337

Integrantes y Contribuciones
Este proyecto fue desarrollado de manera colaborativa. A continuación se detalla la responsabilidad principal de cada uno:
### Responsabilidad principal de cada uno:

| Integrante | Rol Principal | Contribuciones Específicas |
| :--- | :--- | :--- |
| **Nataly Bahamonde** | Líder del Proyecto / Líder Frontend | Desarrollo de la arquitectura de componentes, lógica de consumo de datos (API Fetch), implementación de rutas dinámicas y maquetación general. |
| **Krishna Colivoro** | Frontend Setup y Configuración Responsive | Configuración inicial del proyecto (Astro + TailwindCSS), estructura de carpetas, configuración responsive. |
| **Lucas Vásquez** | Líder Backend | Configuración de Strapi, creación de Content Types. |
| **Antonieta Torres** | Manejo de Contenido Backend | Generación y organización de todo el contenido dinámico del sitio. |

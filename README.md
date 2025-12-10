# Proyecto Restaurante Dinely

Proyecto final para la asignatura de Programación. Sitio web para restaurante ficticio creado con Astro e implementado con Strapi y TailwindCSS.

## ¡IMPORTANTE!

Este proyecto utilizó Inteligencia Artificial únicamente para la extensión de párrafos de los blogs y la creación de imágenes para los productos. En términos de código, se utilizó para resolver el tema de llamar relaciones desde Astro a Strapi, como "categoría":

`category={item.tipos?.[0]?.tipo ?? 'General'}`

En general el resto del proyecto debería estar libre de IA.

## Configuración Para Iniciar el Proyecto
## 🛠️ Guía de Instalación y Configuración

Sigue estos pasos para replicar el entorno de desarrollo localmente.

### Prerrequisitos
* Node.js (v18 o superior)
* npm o yarn
* Una cuenta en GitHub
* Una cuenta en Neon.tech

---

### Paso 1: Configuración de Base de Datos (Neon)
Dado que Neon es una base de datos *serverless* en la nube, no requiere instalación local, solo configuración:

1. Accede a [Neon Console](https://console.neon.tech).
2. Crea un **Nuevo Proyecto**.
3. Selecciona la versión de **Postgres** y la región deseada.
4. Una vez creado, copia el **Connection String** (cadena de conexión) del dashboard.

---

### Paso 2: Instalación de Strapi
Instalación del CMS y configuración del cliente de base de datos.

```
npx create-strapi-app@latest nombre-del-proyecto

Elegir custom y PostgreSQL

se Responde a la terminal de la siguiente manera:

Database name:

Escribe:el nombre que salga al final de el link de Neon

Host:

Escribir solo la dirección (sin postgres:// y sin el usuario):

Ejemplo: ep-cool-app.us-east-2.aws.neon.tech

Port:

Escribe: 5432 

Username:

Copia el usuario del string de Neon 

Password:

Copiar la contraseña larga de Neon. 

Enable SSL connection:

IMPORTANTE: Seleccionar Yes. Neon requiere SSL.
```

para poder iniciar el proyecto se uso el comando

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

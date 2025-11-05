# 🥘 Mesa Mendocina – App Web Full Stack

### 🌎 Proyecto Final – Programación Web

**Mesa Mendocina** es una aplicación web desarrollada con el objetivo de **promocionar y difundir locales gastronómicos mendocinos** que ofrecen comida típica de la región.  
El sistema busca **conectar a turistas y habitantes locales** con una gran variedad de restaurantes, bodegas y casas de comida tradicional, permitiendo también que los dueños gestionen su presencia digital de manera sencilla.

---

## 📋 Índice

1. [Descripción del proyecto](#-descripción-del-proyecto)
2. [Objetivos](#-objetivos)
3. [Integrantes del equipo](#-integrantes-del-equipo)
4. [Tecnologías utilizadas](#-tecnologías-utilizadas)
5. [Arquitectura del sistema](#-arquitectura-del-sistema)
6. [Entidades principales](#-entidades-principales)
7. [Características principales](#-características-principales)
8. [Instrucciones de instalación](#-instrucciones-de-instalación)
9. [Migraciones y ejecución](#-migraciones-y-ejecución)
10. [Capturas o demostración](#-capturas-o-demostración)
11. [Futuras mejoras](#-futuras-mejoras)
12. [Licencia](#-licencia)

---

## 🧾 Descripción del proyecto

**Mesa Mendocina** es una **app web full stack** desarrollada para **visibilizar, promocionar y difundir locales gastronómicos mendocinos**.  
Su objetivo principal es **ofrecer una plataforma intuitiva y atractiva** donde los usuarios puedan descubrir lugares que ofrezcan comida regional, leer valoraciones, realizar reservas y conocer la cultura gastronómica de Mendoza.

Además, los dueños de locales pueden registrarse y administrar su información, platos, horarios y disponibilidad de reservas desde un panel dedicado.

---

## 🎯 Objetivos

- Facilitar la **búsqueda y descubrimiento de locales gastronómicos típicos**.  
- Brindar una **herramienta digital a los dueños de locales** para gestionar su presencia online.  
- Permitir a los usuarios **dejar reseñas, calificaciones y realizar reservas**.  
- Promover la **identidad cultural y culinaria mendocina**.

---

## 👥 Integrantes del equipo

| Nombre | Rol |
|--------|-----|
| **Enzo Rojas** | Backend Developer |
| **Matías Agüero** | Full Stack Developer |
| **Gustavo Vera** | Full Stack Developer |
| **Lautaro Videla** | Full Stack Developer |

---

## 🧰 Tecnologías utilizadas

### 🖥️ Frontend
- HTML5  
- CSS3  
- Bootstrap 5  
- JavaScript  
- Jinja2 (para renderizado dinámico de plantillas)

### ⚙️ Backend
- Python 3  
- Flask (framework principal)  
- SQLAlchemy (ORM)

### 🗄️ Base de datos
- SQLite (modo desarrollo)  
- MySQL / PostgreSQL (opcional para producción)

### 🧩 Control de versiones
- Git & GitHub

### 🛠️ Herramientas adicionales
- Visual Studio Code  
- Flask-Migrate  
- Flask-Login  
- Flask-WTF (formularios)  
- Bootstrap Icons / FontAwesome

---

## 🏗️ Arquitectura del sistema

El proyecto sigue el patrón **MVC (Modelo - Vista - Controlador)**:

- **Modelos:** Representan las entidades principales (Usuario, Local, Plato, Valoración, Reserva).  
- **Vistas:** Interfaz visual del usuario, construida con HTML, Jinja2 y Bootstrap.  
- **Controladores:** Gestionan la lógica del negocio y la comunicación entre vistas y modelos.

---

## 🧩 Entidades principales

- **Usuario (User):** Representa tanto a los clientes como a los dueños de locales.  
- **Local (Location):** Negocio gastronómico registrado por un dueño.  
- **Plato (Plate):** Comidas ofrecidas en un local.  
- **Valoración (Rating):** Reseña y puntaje que un cliente deja sobre un local.  
- **Reservación (Reservation):** Registro de reservas realizadas por los clientes.

---

## 🌟 Características principales

- 🔐 Sistema de **autenticación y registro** (usuarios y dueños).  
- 🏠 Panel de administración para dueños.  
- 🍽️ Listado y detalle de locales con platos típicos.  
- ⭐ Sistema de **valoraciones y comentarios**.  
- 📅 Gestión de **reservas online**.  
- 📱 Diseño **responsivo y moderno** con Bootstrap.  
- 📊 Base de datos relacional y migraciones automáticas.  
- 🌐 Arquitectura **Full Stack Python + Flask**.

---

## ⚙️ Instrucciones de instalación

1. **Clonar el repositorio**
   ```bash
   git clone https://github.com/EnzoER16/Mesa-Mendocina-App-Web-Full-Stack.git
   cd Mesa-Mendocina-App-Web-Full-Stack

2. **Crear un entorno virtual**
   ```bash
   Python -m venv vevnv

3. **Activar el entorno virtual**
   [Windows]
   ```bash
   venv/scripts/actívate
   [Linux]
   ```bash
   source venv/bin/actívate
4. **Instalar dependencias**
   ```bash
   pip install -r requirements.txt

## 🧱 Migraciones y Ejecución

### 1. Crear las Migraciones

    flask db init
    flask db migrate -m "Inicialización de la base de datos"
    flask db upgrade

### 2. Ejecutar la Aplicación

    flask run

> Por defecto, la aplicación estará disponible en:  
> **http://127.0.0.1:5000**

---

## 🌐 Funcionalidades Principales

- 🔍 Búsqueda y filtrado de locales gastronómicos.  
- 🧾 Visualización de platos típicos y precios.  
- ⭐ Valoración y comentarios de los usuarios.  
- 📅 Sistema de reservas online.  
- 👨‍💼 Panel para dueños de locales (gestión de información, platos y reservas).  
- 📱 Interfaz adaptable (responsive) desarrollada con Bootstrap.

---

## 🧠 Estructura del Proyecto

    Mesa-Mendocina/
    │
    ├── app/
    │   ├── static/           # Archivos estáticos (CSS, JS, imágenes)
    │   ├── templates/        # Vistas HTML con Jinja2
    │   ├── models.py         # Definición de las entidades
    │   ├── routes.py         # Rutas y controladores
    │   ├── forms.py          # Formularios y validaciones
    │   └── __init__.py       # Inicialización de Flask y base de datos
    │
    ├── migrations/           # Carpeta generada por Flask-Migrate
    ├── requirements.txt      # Dependencias del proyecto
    ├── config.py             # Configuración general
    ├── run.py                # Punto de entrada de la aplicación
    └── README.md             # Este archivo

---

## 💬 Posibles Mejoras Futuras

- Implementación de autenticación con JWT.  
- Integración con Google Maps API.  
- Sistema de notificaciones por correo electrónico.  
- Modo oscuro (dark mode).  
- Panel administrativo avanzado con estadísticas.

---

## 📸 Capturas de Pantalla *(Opcional)*

> Podés agregar imágenes de la app en funcionamiento cuando esté subida a GitHub.

---

## 📄 Licencia

Este proyecto fue desarrollado con fines educativos para la materia **Programación Web Full Stack**, dentro del **IES 9023** (Mendoza, Argentina).

---

## ❤️ Agradecimientos

A nuestro profesor y compañeros por el acompañamiento y guía durante el desarrollo del proyecto.  
Y a toda la comunidad mendocina que nos inspira a promover su cultura y gastronomía 🍇.


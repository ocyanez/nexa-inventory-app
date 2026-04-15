# 📱 NEXA — Aplicación de Inventario con IA

🚀 Proyecto Capstone desarrollado durante aproximadamente **6 meses** como parte del proceso de titulación en Ingeniería en Informática.

Aplicación móvil fullstack que permite la gestión de inventarios, integrando tecnologías modernas y un componente de inteligencia artificial.

---

## 🎯 Descripción del proyecto

NEXA es una aplicación orientada a la gestión eficiente de inventarios (productos, stock, usuarios), diseñada para operar desde dispositivos móviles.

El objetivo principal fue desarrollar una solución completa que abarque:

- Interfaz móvil moderna
- Backend robusto
- Integración con base de datos
- Uso de inteligencia artificial en procesos del sistema

---

## 👨‍💻 Mi rol en el proyecto

- Diseño de la arquitectura completa (frontend + backend)
- Desarrollo de la aplicación móvil con Ionic + React
- Implementación de API REST con FastAPI
- Integración con Supabase (autenticación, base de datos, storage)
- Desarrollo e integración de modelo de inteligencia artificial
- Manejo de estado, validaciones y flujo de datos

---

## 📸 Capturas de la aplicación

A continuación se muestran algunas vistas clave del sistema en funcionamiento:

### 🔐 Login
Pantalla de autenticación de usuarios.
![Login](https://github.com/ocyanez/nexa-inventory-app/blob/main/assets/login.png)

### 🏠 Inicio
Vista principal de la aplicación.
[![Inicio](https://github.com/ocyanez/nexa-inventory-app/blob/main/assets/Inicio.png)

### 📦 Productos
Gestión de inventario y productos.
![Productos](https://github.com/ocyanez/nexa-inventory-app/blob/main/assets/Productos.png)

### ➕ Registro
Formulario para creación de nuevos productos.
![Registro](https://github.com/ocyanez/nexa-inventory-app/blob/main/assets/Registrar.png)

### 📊 Reportes
Visualización de reportes y análisis.
![Reportes](https://github.com/ocyanez/nexa-inventory-app/blob/main/assets/Reportes.png)

### 👤 Perfil
Gestión de información del usuario.
![Perfil](https://github.com/ocyanez/nexa-inventory-app/blob/main/assets/Perfil.png)

---

## 🚀 Funcionalidades principales

- 🔐 Autenticación de usuarios (login, registro)
- 📦 Gestión de productos (CRUD completo)
- 📊 Control de stock
- 🔎 Búsqueda y filtrado de productos
- 👤 Gestión de usuarios
- 📱 Interfaz móvil moderna
- 🤖 Integración con inteligencia artificial

---

## 🛠 Tecnologías utilizadas

| Capa | Tecnología | Rol |
|------|-------------|------|
| Frontend | Ionic + React | Interfaz móvil y navegación |
| Backend | FastAPI | API REST y lógica de negocio |
| Base de datos | Supabase (PostgreSQL) | Persistencia, auth, storage |
| Otros | TypeScript, Python, CSS | Desarrollo general |

---

## 🏗 Arquitectura del sistema

- El **frontend** se comunica con el backend mediante API REST  
- El **backend** gestiona lógica de negocio, validaciones y datos  
- **Supabase** maneja autenticación, base de datos y almacenamiento  

---

## ⚠️ Nota importante

Debido a que el backend original (Supabase) ya no se encuentra activo:

- La autenticación fue deshabilitada en esta versión demo  
- Se presentan capturas funcionales del sistema  
- El proyecto se muestra con fines demostrativos  

---

## ⚙️ Instalación & Ejecución

### Backend

```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload

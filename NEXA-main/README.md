# NEXA — Inventario App (Ionic + React + Supabase)

> Aplicación móvil de inventario desarrollada como proyecto Capstone, usando tecnologías modernas para frontend, backend y base de datos.

---

## 📌 Índice
1. [Resumen](#resumen)  
2. [Tecnologías](#tecnologías)  
3. [Arquitectura & Estructura del proyecto](#arquitectura--estructura-del-proyecto)  
4. [Funcionalidades principales](#funcionalidades-principales)  
5. [Requisitos](#requisitos)  
6. [Instalación & Ejecución](#instalación--ejecución)  
7. [Configuración / Variables de entorno](#configuración--variables-de-entorno)  
8. [Cómo contribuir](#cómo-contribuir)  
9. [Licencia](#licencia)  
10. [Créditos / Contribuidores](#créditos--contribuidores)  

---

## 📖 Resumen

NEXA es una aplicación para gestión de inventario (productos, stock, almacenes, usuarios), con cliente móvil y backend.  
El objetivo es facilitar el manejo de inventarios a través de una interfaz móvil moderna y un backend robusto.  

El stack incluye:

- **Ionic + React** para la aplicación móvil / frontend  
- **Supabase** como servicio de base de datos / autenticación / almacenamiento /API 

---

## 🛠 Tecnologías

| Capa | Tecnología | Rol / Responsabilidad |
|------|-------------|------------------------|
| Frontend / Mobile | Ionic + React | UI, navegación, llamadas a API |
| Backend / API | Api Supabase | construcción de la API, integrando lógica de negocio y validaciones, IA |
| BBDD / Auth / Storage | Supabase | Base de datos PostgreSQL, autenticación (Auth), Storage, triggers |
| Otros | TypeScript, Python, CSS | Lenguajes base para frontend y backend |

En este proyecto se emplean tecnologías modernas que abarcan todo el ciclo de desarrollo. Ionic con React se utiliza en el frontend móvil, encargado de la interfaz de usuario, la navegación y la comunicación con el backend. En el lado del servidor, FastAPI funciona como framework principal para la construcción de la API, integrando lógica de negocio y validaciones, además de aprovechar capacidades de inteligencia artificial en ciertos procesos. Como servicio integral, Supabase proporciona la base de datos PostgreSQL, la autenticación de usuarios, el almacenamiento de archivos y funciones adicionales que facilitan la gestión de datos. Finalmente, lenguajes como TypeScript, Python y CSS sirven como base sólida para el desarrollo de tanto el cliente como el servidor.
---

## 🏗 Arquitectura & Estructura del proyecto

inventario-app
├── backend
│   ├── app
│   └── requirements.txt
├── docs
│   ├── diagramas
│   └── diagramas_img
├── frontend
│   ├── .vscode
│   ├── android
│   ├── Cypress
│   ├── dist
│   ├── node_modules
│   ├── public
│   └── src
├── .browserslistrc
├── .env
├── .gitignore
├── capacitor.config.ts
├── cypress.config.js
├── eslint.config.js
├── global.css
├── index.html
├── ionic.config.json
├── package-lock.json
├── package.json
├── postcss.config.js
├── tailwind.config.js
├── tsconfig.json
├── tsconfig.node.json
├── vite.config.ts
├── modelo_ia
│   ├── dataset_inicial
│   ├── dataset_limpio
│   ├── descargar_dataset.py
│   ├── modelo_final.h5
│   ├── modelo_final.tflite
│   ├── modelo_ia.py
│   └── preparar_dataset.py
├── node_modules
├── .gitattributes
├── .gitignore
├── package-lock.json
├── package.json
└── README.md

- El **frontend** se comunica con el backend vía HTTP (REST).  
- El **backend** gestiona la lógica, validaciones, autenticación, operaciones CRUD.  
- **Supabase** provee base de datos, autenticación y almacenamiento.  

---

## 🚀 Funcionalidades principales

- 🔐 Autenticación de usuarios (login, registro)  
- 📦 Gestión de productos (crear, leer, actualizar, eliminar)  
- 📊 Control de stock / cantidades disponibles  
- 🔎 Búsqueda y filtros de productos  
- 👤 Usuarios unicos  
- 📱 Interfaz móvil moderna  

---

## 📋 Requisitos

- Node.js ≥ 16  
- npm 
- Python 3.10+  
- pip  
- Supabase (proyecto configurado con URL y claves)  
- Ionic CLI  

---

## ⚙️ Instalación & Ejecución

### Backend (FastAPI)

```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
npm install apexcharts react-apexcharts @supabase/supabase-js
El servidor correrá en http://127.0.0.1:8000.

Frontend (Ionic + React)

cd frontend
npm install
ionic serve

🔑 Configuración / Variables de entorno
Backend (.env)

SUPABASE_URL=tu_url_de_supabase
SUPABASE_KEY=tu_api_key
DATABASE_URL=postgresql://user:pass@host:port/dbname
SECRET_KEY=clave_secreta
ALGORITHM=HS256
ACCESS_TOKEN_EXPIRE_MINUTES=30

Frontend (.env.local)

REACT_APP_SUPABASE_URL=tu_url_de_supabase
REACT_APP_SUPABASE_KEY=tu_api_key_publica
REACT_APP_API_URL= http://localhost:8100


🤝 Cómo contribuir
Haz un fork del repositorio
Crea una rama: git checkout -b feature/nueva-funcion
Haz tus cambios y commits claros
Envía un pull request

📄 Licencia
MIT License © 2025 — Equipo NEXA

👥 Créditos / Contribuidores
Octavio / Octavio Yáñez
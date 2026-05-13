# Proyecto Auth Fullstack

Sistema de autenticación con frontend y backend.  
Incluye registro de usuario y recuperación de contraseña mediante token.

## Descripción

El sistema está dividido en dos partes principales:

- Frontend (React + Vite): interfaz para el registro, inicio de sesión,  y recuperación de contraseña.
- Backend (Node.js + Express + MongoDB): API que gestiona usuarios, tokens.

## Funcionalidades

1. Registro de usuario  
   - El usuario completa el formulario de registro.  
   - Se guarda en la base de datos

<img width="800" height="638" alt="image" src="https://github.com/user-attachments/assets/c83feae1-af72-466a-a95b-7f926e96f298" />


2. Verificación de cuenta

<img width="682" height="237" alt="image" src="https://github.com/user-attachments/assets/f8c55723-2915-42f3-8a50-e85765987e4d" />


4. Inicio de sesión  
   - Solo usuarios verificados pueden iniciar sesión.  
   - Se genera un token JWT para mantener la sesión activa.

5. Recuperación de contraseña  
   - El usuario solicita recuperar su contraseña.  
   - Se envía un token temporal para restablecerla.
  
<img width="795" height="635" alt="image" src="https://github.com/user-attachments/assets/c4648362-de58-47da-ae28-cbede520ea45" />


## Estructura del proyecto

```bash
auth-fullstack/
│
├── backend/
│   ├── controllers/
│   │   └── auth.controller.js
│   ├── models/
│   │   └── User.js
│   ├── routes/
│   │   └── auth.routes.js
│   ├── utils/
│   │   └── sendEmail.js
│   ├── .env
│   ├── package.json
│   ├── package-lock.json
│   └── server.js
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── pages/
│   │   │   ├── Register.jsx
│   │   │   ├── VerifyAccount.jsx
│   │   │   ├── ForgotPassword.jsx
│   │   │   └── ResetPassword.jsx
│   │   ├── services/
│   │   │   └── authService.js
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   └── index.css
│   ├── package.json
│   ├── vite.config.js
│   └── README.md
│
└── .gitignore

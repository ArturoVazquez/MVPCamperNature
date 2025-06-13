🌲 CamperNature - MVP
CamperNature es una aplicación web desarrollada como MVP (Producto Mínimo Viable) para la gestión de reservas de parcelas, vehículos y servicios en entornos naturales. Incluye funcionalidades completas para usuarios y administradores, facilitando la reserva personalizada con servicios extra y fechas específicas.

🛠️ Tecnologías utilizadas
🔹 Frontend (React)
React 19, React DOM

React Router DOM 7 – Rutas dinámicas

Bootstrap 5.3 + React Bootstrap

Bootstrap Icons + React Bootstrap Icons

SweetAlert2 – Alertas visuales

Zod – Validación de formularios

Axios – Peticiones HTTP

React Day Picker – Selección de fechas

React Phone Input 2 – Campo de teléfono internacional

React Flags Select – Selección de países con banderas

i18n-iso-countries – Traducción de nombres de países

country-telephone-data – Códigos de país telefónicos

date-fns – Utilidades de fechas

🔸 Backend (Node.js + Express)
Express.js – API REST

MySQL2 – Conexión a base de datos

Sequelize – ORM para modelos y relaciones

Multer – Subida de imágenes

Bcrypt – Cifrado de contraseñas

JWT (jsonwebtoken) – Autenticación y sesiones

Nodemailer – Envío de correos para recuperación de contraseña

dotenv – Variables de entorno

CORS, Morgan, Cookie-Parser

country-telephone-data, date-fns, zod

📁 Estructura del proyecto
csharp
Copiar
Editar
MVPCamperNature/
├── backend/                # Servidor Express y lógica de negocio
│   ├── controllers/
│   ├── middlewares/
│   ├── models/
│   ├── routes/
│   ├── services/
│   ├── utils/
│   └── index.js
├── frontend/               # Aplicación React
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── schemas/
│   │   ├── services/
│   │   ├── App.jsx
│   │   └── main.jsx
└── README.md
✨ Funcionalidades principales
👤 Usuario
Registro, login y edición de perfil

Recuperación de contraseña vía email

Selección de fechas de entrada/salida con calendario

Reserva de parcelas con disponibilidad real

Selección de servicios adicionales (alta o baja temporada)

Vista previa y confirmación de reservas

🔐 Administrador
Panel de control para gestionar usuarios

Alta, baja y edición de servicios con imágenes

Listado y gestión de reservas activas

Visualización de días ocupados por parcela

⚙️ Configuración del entorno
1. Clonar el repositorio
bash
Copiar
Editar
git clone https://github.com/reposocratech/MVPCamperNature.git
cd MVPCamperNature
2. Instalar dependencias
Backend:

bash
Copiar
Editar
cd backend
npm install
Frontend:

bash
Copiar
Editar
cd ../frontend
npm install
3. Configurar variables de entorno
Crea un archivo .env dentro de la carpeta backend/ con el siguiente contenido:

env
Copiar
Editar
PORT=5000
DB_HOST=localhost
DB_NAME=campernature
DB_USER=root
DB_PASSWORD=tu_password
JWT_SECRET=una_clave_segura
EMAIL_USER=tu_email@gmail.com
EMAIL_PASS=tu_contraseña_de_aplicación
CLIENT_URL=http://localhost:5173
💡 Asegúrate de tener una base de datos MySQL creada con el nombre campernature.

4. Ejecutar el proyecto
Backend:

bash
Copiar
Editar
cd backend
npm run dev
Frontend:

bash
Copiar
Editar
cd ../frontend
npm run dev
🧪 Estado actual del MVP
✅ Autenticación con JWT
✅ Recuperación de contraseña con correo
✅ Formulario de reserva con calendario y validaciones
✅ Gestión de servicios en panel administrador
✅ Reserva con verificación de fechas
✅ Subida de imágenes y edición de servicios

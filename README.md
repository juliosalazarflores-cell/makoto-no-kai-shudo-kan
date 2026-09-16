# Makoto No Kai Shudo Kan - Sistema de Gestión de Escuelas de Karate

🥋 Plataforma SaaS para la administración completa de múltiples escuelas de karate.

## 📋 Características Principales

- **Gestión Multi-Escuela**: Administra múltiples escuelas desde una única plataforma
- **Gestión de Estudiantes**: Registro, niveles (cinturones), progreso y datos personales
- **Calendario de Clases**: Programación de clases, horarios e instructores
- **Registro de Asistencia**: Seguimiento automático de asistencia por clase
- **Sistema de Pagos**: Gestión de suscripciones, cuotas y pagos
- **Seguimiento de Progreso**: Historial de ascensos de cinturón y logros
- **Panel de Control**: Dashboards para instructores, administradores y estudiantes
- **Comunicaciones**: Notificaciones y mensajes entre escuela y estudiantes
- **Reportes**: Análisis de asistencia, ingresos y rendimiento

## 🛠️ Stack Tecnológico

### Frontend
- **React 18** - UI Library
- **TypeScript** - Type Safety
- **Tailwind CSS** - Styling
- **Vite** - Build tool
- **React Router** - Routing
- **Axios** - HTTP Client

### Backend
- **Node.js** - Runtime
- **Express.js** - Framework
- **PostgreSQL** - Database
- **Sequelize** - ORM
- **JWT** - Authentication
- **Docker** - Containerization

## 📁 Estructura del Proyecto

```
makoto-no-kai-shudo-kan/
├── frontend/                 # Aplicación React
│   ├── src/
│   │   ├── components/      # Componentes reutilizables
│   │   ├── pages/           # Páginas de la app
│   │   ├── services/        # Servicios API
│   │   ├── hooks/           # Custom hooks
│   │   ├── context/         # Context API
│   │   ├── styles/          # Estilos globales
│   │   ├── types/           # TypeScript types
│   │   └── App.tsx
│   ├── public/
│   ├── package.json
│   ├── tsconfig.json
│   ├── vite.config.ts
│   └── tailwind.config.js
│
├── backend/                  # API Node.js/Express
│   ├── src/
│   │   ├── models/          # Modelos de base de datos
│   │   ├── routes/          # Rutas de API
│   │   ├── controllers/     # Lógica de negocio
│   │   ├── middleware/      # Middlewares
│   │   ├── services/        # Servicios de negocio
│   │   ├── utils/           # Funciones utilitarias
│   │   ├── config/          # Configuración
│   │   └── server.ts
│   ├── migrations/          # Migraciones de BD
│   ├── seeders/            # Datos iniciales
│   ├── package.json
│   ├── tsconfig.json
│   └── .env.example
│
├── docs/                     # Documentación
│   ├── ARCHITECTURE.md      # Arquitectura del proyecto
│   ├── API.md               # Documentación API
│   ├── DATABASE.md          # Esquema de BD
│   ├── SETUP.md             # Guía de instalación
│   └── CONTRIBUTING.md      # Guías de contribución
│
├── docker-compose.yml       # Orquestación de servicios
├── .gitignore
├── .env.example
└── LICENSE
```

## 🚀 Inicio Rápido

### Requisitos
- Node.js 18+
- PostgreSQL 12+
- Docker (opcional)

### Instalación Local

1. **Clonar repositorio**
```bash
git clone https://github.com/juliosalazarflores-cell/makoto-no-kai-shudo-kan.git
cd makoto-no-kai-shudo-kan
```

2. **Configurar Backend**
```bash
cd backend
cp .env.example .env
npm install
npm run db:migrate
npm run dev
```

3. **Configurar Frontend**
```bash
cd frontend
npm install
npm run dev
```

4. **Acceder**
- Frontend: http://localhost:5173
- Backend API: http://localhost:3000

### Con Docker

```bash
docker-compose up -d
```

## 📚 Documentación

- [Arquitectura del Proyecto](./docs/ARCHITECTURE.md)
- [Documentación de API](./docs/API.md)
- [Esquema de Base de Datos](./docs/DATABASE.md)
- [Guía de Configuración](./docs/SETUP.md)

## 👥 Roles de Usuario

- **Admin Sistema**: Control total de la plataforma
- **Admin Escuela**: Administra su escuela específica
- **Instructor**: Crea clases, registra asistencia
- **Estudiante**: Ve su progreso, paga cuotas
- **Padre/Tutor**: Monitorea progreso del estudiante

## 📊 Módulos Principales

- **Autenticación & Autorización**: Multi-tenant con JWT
- **Gestión de Escuelas**: Crear y administrar escuelas
- **Gestión de Usuarios**: Estudiantes, instructores, padres
- **Gestión de Clases**: Horarios, instructores, capacidad
- **Sistema de Pagos**: Suscripciones y transacciones
- **Reportes**: Análisis y estadísticas

## 📄 Licencia

MIT License - Ver [LICENSE](./LICENSE) para detalles

## 📞 Soporte

Para reportar bugs o sugerir features, abre un [issue](https://github.com/juliosalazarflores-cell/makoto-no-kai-shudo-kan/issues)

---

**Hecho con ❤️ para la comunidad de karate**

# Appointment Booker 🚀

**Full-stack appointment booking system** built with **Laravel 12+**, **Vue 3 + TypeScript**, **TailwindCSS** and **Docker**. Designed for healthcare, clinics, consultants, and SaaS platforms.

[![Laravel](https://img.shields.io/badge/Laravel-12+-red.svg?logo=laravel&logoColor=white)](https://laravel.com)
[![Vue.js](https://img.shields.io/badge/Vue.js-3-green.svg?logo=vuedotjs)](https://vuejs.org)
[![TypeScript](https://img.shields.io/badge/TypeScript-strict-blue.svg?logo=typescript&logoColor=white)](https://www.typescriptlang.org)
[![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3+-cyan.svg?logo=tailwind-css)](https://tailwindcss.com)
[![Docker](https://img.shields.io/badge/Docker-ready-2496ED.svg?logo=docker&logoColor=white)](https://docker.com)

## ✨ **Live Demo** *(coming soon)*

Frontend: https://appointment-booker-frontend.vercel.app
Backend API: https://api.appointment-booker.purgato96.com

## 🎯 **Features Planned**

- [x] **Multi-role Authentication** (Patients, Doctors, Admins) - Sanctum/JWT
- [x] **Interactive Calendar** - FullCalendar + Vue 3 + Axios API
- [ ] **Real-time Availability** - WebSockets/Pusher
- [ ] **Email Notifications** - Laravel Mail + Queues
- [ ] **Multi-tenant SaaS Ready** - Spatie Permission
- [x] **Responsive Design** - TailwindCSS + Mobile-first
- [x] **TypeScript Everywhere** - Frontend + API contracts
- [ ] **Admin Dashboard** - Doctors/Services management
- [x] **API-First Architecture** - RESTful + Documentation
- [ ] **Testing** - Pest (Backend) + Cypress (E2E)
- [x] **Dockerized** - One-command setup

## 🛠 **Tech Stack**

Backend: Laravel 12+ | PostgreSQL | Redis | Sanctum
Frontend: Vue 3 | TypeScript | TailwindCSS | Axios | Pinia
DevOps: Docker | GitHub Actions CI/CD | Vercel | Railway
Testing: Pest | Cypress | Vitest

## 🚀 **Quick Start (Docker)**

### Pré-requisitos
- Docker & Docker Compose
- Git

```bash
git clone https://github.com/Purgato96/appointment_booker.git
cd appointment_booker
```

### 1. Copia ambiente
```bash
cp .env.example .env
# Edita .env com tuas chaves (DB, APP_KEY, etc.)
```

### 2. Subir tudo (30s)
```bash
docker-compose up -d
```

### 3. Frontend dev
```bash
cd frontend
npm install
npm run dev
```

**Acessa:**
- **Frontend**: http://localhost:5173
- **Backend**: http://localhost:8000
- **Adminer/DB**: http://localhost:8080

## 📁 **Estrutura do Projeto**

```
appointment_booker/
├── backend/           # Laravel 12+ API
│   ├── app/Http/Controllers/AppointmentController.php
│   ├── routes/api.php
│   └── database/migrations/
├── frontend/          # Vue 3 + TS SPA
│   ├── src/
│   │   ├── components/Calendar.vue
│   │   ├── views/Dashboard.vue
│   │   └── stores/appointment.ts
│   ├── vite.config.ts
│   └── tailwind.config.js
├── docker-compose.yml # (local only)
└── README.md
```

## 🔗 **API Endpoints** (Swagger docs coming)

```
GET    /api/doctors
GET    /api/appointments/slots?doctor_id=1&date=2026-03-13
POST   /api/appointments/book
GET    /api/appointments/my-bookings
PATCH  /api/appointments/{id}/cancel
```

**Exemplo com Axios:**
```javascript
const response = await axios.get('/api/appointments/slots', {
  params: { doctor_id: 1, date: '2026-03-13' }
})
```

## 🧪 **Testing**

```bash
# Backend
cd backend && ./vendor/bin/pest

# Frontend
npm run test:unit
npm run test:e2e

# E2E completo
npm run test:e2e:ci
```

## 🚀 **Deploy em Produção**

- **Frontend**: Vercel/Netlify (estático)
- **Backend**: Railway/DigitalOcean/FORGE (Docker)
- **CI/CD**: GitHub Actions incluído

## 🤝 **Contribuições**

1. Fork o projeto
2. Crie feature branch (git checkout -b feature/AmazingFeature)
3. Commit (git commit -m 'Add some AmazingFeature')
4. Push (git push origin feature/AmazingFeature)
5. Abre Pull Request

## 📄 **Licença**

MIT - Veja LICENSE para mais detalhes.

## 👨‍💻 **Autor**

**Matheus Purgato** - LinkedIn: https://linkedin.com/in/purgato96 | Portfolio: https://purgato.dev | GitHub: https://github.com/Purgato96

**Full-Stack Developer** | Laravel | Vue.js | TypeScript | SaaS Architecture

---

**⭐ Star se curtiu!** **🔔 Watch pra updates!**

---

#Laravel #VueJS #TypeScript #SaaS #Portfolio #FullStack #RemoteDev
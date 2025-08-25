---
layout: default
---

# File Structure de Nitro 📁

## Estructura básica 🏗️
```
my-nitro-app/
├── server/           📦 Server endpoints
│   ├── api/          🔌 REST APIs
│   ├── routes/       🛣️ Rutas personalizadas
│   ├── middleware/   ⚙️ Middlewares
│   └── plugins/      🔧 Plugins server-side
├── nitro.config.ts   ⚙️ Configuración
└── package.json      📦 Dependencias
```

## Endpoints automáticos 🚀
```bash
server/api/hello.ts     → GET /api/hello
server/routes/users.ts  → GET /users
server/middleware/auth.ts → Middleware global
```
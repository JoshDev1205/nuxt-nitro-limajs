---
layout: default
---

# File System Routing de Nitro 🗺️

## Rutas automáticas desde archivos 📁
```
server/
├── api/
│   ├── hello.ts          → GET /api/hello
│   ├── users/
│   │   ├── index.ts      → GET /api/users
│   │   ├── [id].ts       → GET /api/users/123
│   │   └── [id]/
│   │       └── posts.ts  → GET /api/users/123/posts
│   └── auth/
│       └── login.post.ts → POST /api/auth/login
├── routes/
│   ├── index.ts          → GET /
│   ├── about.ts          → GET /about
│   └── admin/
│       └── index.ts      → GET /admin
```
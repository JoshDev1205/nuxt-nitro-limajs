## Métodos HTTP por extensión 🔄
```typescript
// server/api/users.get.ts
export default defineEventHandler(() => {
  return { users: [] }
})

// server/api/users.post.ts
export default defineEventHandler(async (event) => {
  const body = await readBody(event)
  return { created: true }
})
```

## Parámetros dinámicos 🎯
• **[id].ts** → Parámetros dinámicos

• **[...slug].ts** → Catch-all params or routes

⚡ *Rutas sin configuración, solo archivos*
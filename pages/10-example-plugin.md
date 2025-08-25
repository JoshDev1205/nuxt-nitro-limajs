---
layout: default
---

## Ejemplos prácticos 🛠️

### Database Plugin 🗄️
```typescript
// server/plugins/database.ts
export default defineNitroPlugin(() => {
  const db = connectToDatabase()
  nitroApp.hooks.hook('request', (event) => {
    event.context.db = db
  })
})
```

### Logger Plugin 📝
```typescript
// server/plugins/logger.ts
export default defineNitroPlugin(() => {
  nitroApp.hooks.hook('request', (event) => {
    console.log(`[${event.method}] ${event.path}`)
  })
})
```

🔌 *Extiende Nitro, hazlo tuyo*
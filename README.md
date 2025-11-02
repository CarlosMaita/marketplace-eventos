# Marketplace Eventos

Marketplace para músicos, DJs, salones de eventos y proveedores de entretenimiento.

## 🚀 Stack Tecnológico

### Frontend Web
- **Framework:** Next.js (React, TypeScript)
- **UI:** Tailwind CSS o Chakra UI
- **Autenticación:** NextAuth.js
- **Integración de diseño:** Figma Pro (tokens/plugins exportables)
- **Gestión de componentes:** (Opcional) Storybook

### App Mobile
- **Framework:** Flutter (Android/iOS)
- **Lenguaje:** Dart
- **Consumo de API:** HTTP/gRPC, compatible con el backend NestJS

### Backend
- **Lenguaje:** TypeScript
- **Framework:** NestJS (o API Routes de Next.js)
- **ORM:** Prisma
- **Base de datos:** PostgreSQL

### Infraestructura y despliegue
- **Despliegue principal:** VPS (DigitalOcean, etc.) usando Docker y docker-compose
- **Orquestación:** Docker y docker-compose para desarrollo y producción.

### Servicios externos
- **Almacenamiento archivos:** Cloudinary o AWS S3
- **Pagos:** Stripe
- **Email:** Resend o SendGrid
- **Notificaciones:** Firebase Cloud Messaging (opcional)
- **Buscador:** Algolia (opcional)
- **Mapas:** Google Maps API

### DevOps / Colaboración
- **Diseño:** Figma Pro
- **Gestión de tareas:** Notion, Jira, Trello, etc.
- **Control de versiones:** GitHub

---

## 📋 Estructura de carpetas propuesta

```
/ 
├── apps/ 
│   ├── frontend/        # Next.js (React web)
│   ├── backend/         # NestJS (API)
│   └── mobile/          # Flutter (Android/iOS)
├── packages/ 
│   └── ui/              # (Opcional) Componentes, modelos o utilidades compartidas
├── docker-compose.yml   # Orquestación local para web/backend/db
├── .env.example
├── README.md
└── docs/
```

### Ejemplo de estructura interna para `apps/mobile/` (Flutter)
```
apps/mobile/
├── android/
├── ios/
├── lib/
│   ├── src/
│   │   ├── core/
│   │   ├── features/
│   │   ├── shared/
│   │   └── app.dart
│   └── main.dart
├── test/
├── pubspec.yaml
└── (otros archivos clásicos de Flutter)
```

---

## 💡 Notas

- **Flutter** permite una sola base de código para Android y iOS.
- **API Backend** debe diseñarse para ser consumida tanto por web como por mobile.
- Lógica, modelos o assets compartidos pueden ubicarse en `packages/ui/` o subcarpetas de `packages/`.
- Figma sigue siendo la fuente central para el diseño visual y tokens.
- Documentación técnica o de producto puede ir en `docs/`. 

---

¿Listo para el siguiente paso? ¡Avísame si quieres que te ayude a crear archivos base, ejemplos de configuración, o el primer commit!
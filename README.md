# Loyal Light - Plataforma Freemium de Fidelización Retail LATAM

## Descripción
Loyal Light es una plataforma freemium que ofrece fidelización y recompensas con IA explicable, analítica predictiva y automatizaciones multicanal para comercios minoristas en LATAM. MVP 100% gratis con onboarding asistido.

## Stack
- Frontend: Next.js 14 (App Router) + TypeScript + TailwindCSS + shadcn/ui
- Backend/BBDD: Supabase Free Tier (Auth, Postgres, RLS, Edge Functions)
- Despliegue: Vercel Free Tier (frontend), Supabase (backend)
- Automatización: Make.com (guías para cuentas propias de comercios)
- Emails/Notificaciones: EmailJS, SMTP gratuito, WhatsApp API (claves propias)
- Paquetería: pnpm
- Node: 20 LTS

## Setup Local
1. Instala pnpm: `npm install -g pnpm`
2. Clona el repo: `git clone <repo-url>`
3. Instala dependencias: `pnpm install`
4. Configura Supabase local: `pnpm supabase init` y `pnpm supabase start`
5. Crea .env.local (ver notas de migración)
6. Ejecuta dev: `pnpm dev` (para /apps/web)

## Despliegue
- Frontend: Vercel CLI `vercel` (conecta a proyecto Free Tier)
- Backend: Supabase dashboard (push migraciones con `pnpm supabase db push`)

## Ramas
- main: Estable
- develop: Desarrollo
- feature/*: Features específicas

## Documentación
- /docs/checklist.md: Tareas pendientes
- /docs/decisiones.md: Decisiones clave
- /docs/roadmap.md: Roadmap MVP
- /docs/referencias.md: Referencias externas
- /docs/adrs/: ADRs ligeros

## Licencia
MIT
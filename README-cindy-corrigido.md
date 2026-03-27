<div align="center">

![Banner](https://raw.githubusercontent.com/fabryciobermudes/cindy-condominio/main/banner.svg)

# Cindy Condomínio
</div>

Plataforma completa de gestão condominial desenvolvida com **React**, **TypeScript**, **Vite** e **Supabase**.

[![Tecnologias](https://img.shields.io/badge/React-18.3-blue?logo=react)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.8-blue?logo=typescript)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-7.3-purple?logo=vite)](https://vitejs.dev/)
[![Supabase](https://img.shields.io/badge/Supabase-PostgreSQL-green?logo=supabase)](https://supabase.com/)

---

## 🚀 Funcionalidades

- 🏠 **Gestão de Moradores** — Cadastro, tipos (proprietário/inquilino/dependente), termos digitais
- 🚗 **Veículos** — Aprovação, tags de acesso, vagas de garagem
- 📦 **Encomendas** — Recebimento, notificação, controle de retirada
- ⚠️ **Ocorrências** — Reclamações, advertências, multas
- 📅 **Reservas** — Salão de festas, churrasqueira, áreas comuns
- 🗳️ **Assembleias** — Votação online, pautas, atas digitais
- 💬 **Chat** — Comunicação interna (integração WhatsApp)
- 📢 **Comunicados** — Avisos e documentos compartilhados
- 📊 **Dashboard** — Métricas e indicadores em tempo real

---

## 🛠️ Tecnologias

| Frontend | Backend | UI/UX |
|---|---|---|
| React 18.3 | Supabase (PostgreSQL) | shadcn/ui |
| TypeScript 5.8 | Edge Functions (Deno) | Tailwind CSS |
| Vite 7.3 | Auth (JWT) | Radix UI |
| React Router DOM v6 | Realtime (WebSocket) | Lucide Icons |
| TanStack Query v5 | Storage | Recharts |
| React Hook Form | | TipTap Editor |

---

## 📖 Documentação

A documentação técnica completa está disponível no diretório [`docs/`](./docs/README.md):

- [**Visão Geral**](./docs/00-visao-geral.md) — Arquitetura e stack tecnológico
- [**Design System**](./docs/01-design-system.md) — Cores, tipografia, componentes
- [**Estrutura**](./docs/10-estrutura-pastas.md) — Organização de pastas e arquivos
- [**Rotas**](./docs/11-rotas-navegacao.md) — Mapa de navegação da aplicação
- [**Dashboard**](./docs/20-dashboard.md) — Métricas e cálculos
- [**Supabase**](./docs/30-supabase-config.md) — Configuração e queries
- [**Edge Functions**](./docs/40-edge-functions.md) — 31 funções serverless
- [**APIs**](./docs/41-api-residents.md) — APIs REST (residents, vehicles)
- [**Emails**](./docs/50-emails-automaticos.md) — Automações de email
- [**Referência Rápida**](./docs/99-referencia-rapida.md) — Comandos e snippets

---

## 🚀 Quick Start

### Pré-requisitos

- Node.js 18+ (recomendado via [nvm](https://github.com/nvm-sh/nvm))
- npm ou yarn
- Projeto Supabase configurado

### Instalação

```bash
# Clonar repositório
git clone <URL_DO_REPOSITORIO>
cd "Cindy Condominio"

# Instalar dependências
npm install

# Configurar variáveis de ambiente (.env)
# VITE_SUPABASE_URL=...
# VITE_SUPABASE_ANON_KEY=...

# Iniciar servidor de desenvolvimento
npm run dev
```

Acesse: `http://localhost:8080`

---

## 📁 Estrutura do Projeto

```
Cindy Condominio/
├── src/
│   ├── components/     # Componentes React (UI + módulos)
│   ├── contexts/       # Context API (6 providers)
│   ├── pages/          # 25 páginas da aplicação
│   ├── hooks/          # Custom hooks
│   ├── integrations/   # Cliente Supabase
│   ├── lib/            # Utilitários
│   └── types/          # TypeScript types
├── supabase/
│   ├── functions/      # 31 Edge Functions
│   ├── migrations/     # 66 migrations SQL
│   └── config.toml
├── docs/               # Documentação técnica
├── scripts/            # Scripts de deploy
└── tests/              # Testes
```

---

## 🔧 Scripts Disponíveis

| Comando | Descrição |
|---|---|
| `npm run dev` | Servidor de desenvolvimento (porta 8080) |
| `npm run build` | Build para produção |
| `npm run build:dev` | Build mode development |
| `npm run preview` | Preview do build |
| `npm run lint` | ESLint |
| `npm run deploy:functions` | Deploy de todas Edge Functions |
| `npm run deploy:functions <nome>` | Deploy de função específica |
| `npm run sync:secrets` | Sincronizar secrets |

---

## 🔐 Autenticação

O sistema utiliza **Supabase Auth** com os seguintes fluxos:

- Login/Logout
- Signup (cadastro)
- Recuperação de senha
- Convites por email
- Multi-tenant (usuário pode pertencer a múltiplos condomínios)

**Roles:** `owner` | `admin` | `resident` | `staff`

---

## 📊 Banco de Dados

Principais tabelas:

| Tabela | Descrição |
|---|---|
| `tenants` | Condomínios (multi-tenant) |
| `profiles` | Perfis de usuário |
| `user_roles` | Vínculo usuário-condomínio |
| `residents` | Moradores |
| `vehicles` | Veículos |
| `packages` | Encomendas |
| `occurrences` | Ocorrências |
| `assemblies` | Assembleias |
| `space_reservations` | Reservas de espaços |

---

## 🌐 Links

- **Lovable Project:** https://lovable.dev/projects/253b1b3e-9e51-4384-8bb8-baaea86d7f27
- **Supabase Dashboard:** https://app.supabase.com/project/bkylmrplggbfraeriynr

---

## 📝 Licença

Projeto proprietário — Cindy Condomínio © 2025-2026

---

*Desenvolvido com ❤️ para simplificar a gestão condominial*

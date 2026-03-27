<div align="center">
  <img src="https://raw.githubusercontent.com/fabryciobermudes/dashboard_usabit/main/banner.svg" width="100%" alt="Usabit Meta Ads Dashboard Banner">

  <br />

  # 🚀 Usabit Meta Ads Dashboard
  **Alta performance e gestão estratégica de campanhas do Meta Ads.**

  <br />

  ![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.dot.js&logoColor=white)
  ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
  ![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)

  <br />

  ---

  Um dashboard de alta performance desenvolvido para a **Usabit**, focado no monitoramento estratégico de campanhas do Meta Ads e gestão automatizada de leads via Google Sheets.
</div>

## ✨ Funcionalidades Principais

### 📊 Monitoramento de Campanhas
- **Visão 360º**: KPIs em tempo real (Spend, Reach, Clicks, CTR, CPC, CPM).
- **Analytics Visual**: Gráficos interativos de investimento diário e distribuição por objetivo.
- **Filtros Avançados**: Segmentação por status, data (hoje, 7 dias, 30 dias, personalizado) e campanha específica.
- **Detalhamento**: Tabela interativa com Drawer lateral para análise profunda de cada anúncio.

### 🎯 Gestão de Leads (Pipeline)
- **Kanban Integrado**: Fluxo de trabalho visual (Novo → Contato → Qualificado → Convertido).
- **Google Sheets Sync**: Integração dinâmica com múltiplas planilhas.
- **Banco de Leads**: Repositório centralizado para busca e exportação.

### 🧭 Experiência de Usuário (UX/UI)
- **Dual Nav Mode**: Alterne entre Menu Lateral (Sidebar) e Abas Superiores (TopBar).
- **Brutalist Design**: UI moderna, de alto contraste, otimizada para eficiência técnica.
- **Login v2**: Portal de acesso seguro com estética inspirada no Meta Business Suite.

## 🛠️ Stack Técnica

- **Framework**: Next.js 15+ (App Router)
- **Estilização**: Tailwind CSS v4 (CSS-first configuration)
- **Ícones**: Lucide React
- **Linguagem**: TypeScript (Strict Mode)
- **Estado**: Context API para gerenciamento de preferências (Navigation Mode)

## 🚀 Como Iniciar

### Pré-requisitos
- Node.js 18+
- NPM ou Yarn

### Instalação

1. Clone o repositório:
```bash
git clone https://github.com/usabit/dashboard_usabit.git
```

2. Instale as dependências:
```bash
npm install
```

3. Configure as variáveis de ambiente:
Crie um arquivo `.env.local` na raiz com:
```env
META_ACCESS_TOKEN=your_token
META_AD_ACCOUNT_ID=your_id
GOOGLE_SERVICE_ACCOUNT_JSON={"your": "json_config"}
```

4. Inicie o servidor de desenvolvimento:
```bash
npm run dev
```

Acesse `http://localhost:3000` para visualizar.

## 📁 Estrutura do Projeto

- `/src/app`: Rotas e layouts (Next.js App Router).
- `/src/components`: Componentes de UI divididos por domínio (layout, campaigns, leads).
- `/src/lib`: Utilidades, dados mockados e lógica de integração de APIs.
- `/src/types`: Definições globais de tipos TypeScript.
- `/data`: Arquivos de configuração local (ex: sheets-config.json).

---

## 🤝 Contribuição

Este é um projeto proprietário desenvolvido pela **Usabit**. Para sugestões de melhorias técnicas, entre em contato com o time de engenharia.

---

<div align="center">
  Desenvolvido com ❤️ pela **Usabit**
</div>

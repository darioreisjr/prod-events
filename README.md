# TechEVentos - Plataforma de Eventos de Tecnologia

<div align="center">
  <img src="/public/images/events/banner.png" alt="TechEventos Logo" width="1000" height="232" />
  
  <p>
    <strong>A maior plataforma de eventos de tecnologia do Brasil</strong>
  </p>
  
  <p>
    Conectando pessoas e comunidades tecnológicas através de eventos de alta qualidade
  </p>

![Next.js](https://img.shields.io/badge/Next.js-14.0+-black?style=for-the-badge&logo=next.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-039BE5?style=for-the-badge&logo=Firebase&logoColor=white)

</div>

## 📋 Sobre o Projeto

TechEVentos é uma plataforma completa e moderna para descoberta, organização e participação em eventos de tecnologia. Desenvolvida com as mais recentes tecnologias web, oferece uma experiência fluida e intuitiva para conectar profissionais, estudantes e entusiastas da área tecnológica.

### 🎯 Objetivo

Facilitar a descoberta e participação em eventos de tecnologia, criando uma ponte entre organizadores e participantes, promovendo networking e compartilhamento de conhecimento na comunidade tech brasileira.

## ✨ Funcionalidades Principais

### 🔐 **Sistema de Autenticação**

- Login/cadastro com email e senha
- Autenticação social com Google
- Recuperação de senha
- Autenticação de dois fatores
- Gerenciamento de sessões

### 📅 **Gerenciamento de Eventos**

- Listagem completa de eventos com filtros avançados
- Busca inteligente por título, descrição e localização
- Categorização por área (Frontend, Backend, DevOps, etc.)
- Visualização detalhada com informações completas
- Sistema de inscrições com validação
- Controle de capacidade e lista de espera

### 👤 **Perfil de Usuário**

- Perfil personalizado com informações profissionais
- Histórico de eventos participados
- Sistema de certificados
- Configuração de interesses e preferências
- Integração com redes sociais (GitHub, LinkedIn)

### 💬 **Chat em Tempo Real**

- Sistema de chat integrado para cada evento
- Comunicação entre participantes
- Moderação de mensagens
- Notificações em tempo real

### ⚙️ **Configurações Avançadas**

- Preferências de notificação personalizáveis
- Configurações de privacidade granulares
- Temas claro/escuro
- Acessibilidade avançada
- Integrações com calendários (Google, Outlook)

### 📱 **Interface Responsiva**

- Design mobile-first
- PWA (Progressive Web App)
- Sidebar navegacional intuitiva
- Experiência otimizada para todos os dispositivos

## 🛠️ Tecnologias Utilizadas

### **Frontend**

- **[Next.js 14+](https://nextjs.org/)** - Framework React com App Router
- **[TypeScript](https://www.typescriptlang.org/)** - Tipagem estática
- **[Tailwind CSS](https://tailwindcss.com/)** - Framework CSS utilitário
- **[React Hook Form](https://react-hook-form.com/)** - Gerenciamento de formulários
- **[Zod](https://zod.dev/)** - Validação de esquemas
- **[date-fns](https://date-fns.org/)** - Manipulação de datas

### **Backend & Infraestrutura**

- **[Firebase Authentication](https://firebase.google.com/docs/auth)** - Autenticação
- **[Socket.IO](https://socket.io/)** - Comunicação em tempo real
- **[Axios](https://axios-http.com/)** - Cliente HTTP

### **Desenvolvimento**

- **[ESLint](https://eslint.org/)** - Linting de código
- **[Prettier](https://prettier.io/)** - Formatação de código
- **[Husky](https://typicode.github.io/husky/)** - Git hooks

## 📁 Estrutura do Projeto

```
src/
├── app/                          # App Router (Next.js 14+)
│   ├── (auth)/
│   │   ├── login/               # Página de login
│   │   └── register/            # Página de cadastro
|   ├── communities/             # Módulo de comunidades
|   |   ├── page.tsx             # Página de comunidades
│   ├── events/                  # Módulo de eventos
│   │   ├── page.tsx            # Lista de eventos
│   │   ├── register/           # Inscrição em eventos
│   │   └── chat/               # Chat do evento
│   ├── my-events/              # Eventos do usuário
│   ├── profile/                # Perfil do usuário
│   ├── settings/               # Configurações
│   ├── layout.tsx              # Layout raiz
│   ├── page.tsx                # Página inicial
│   └── globals.css             # Estilos globais
├── components/                  # Componentes reutilizáveis
│   ├── ui/                     # Componentes base (Button, Input, etc.)
│   ├── layout/                 # Componentes de layout
│   ├── events/                 # Componentes específicos de eventos
│   ├── chat/                   # Componentes de chat
|   └── communities/            # Componentes da página de comunidades
├── context/                    # Context API
│   └── UserContext.tsx         # Contexto do usuário
├── hooks/                      # Custom hooks
│   └── useAuth.tsx             # Hook de autenticação
├── lib/                        # Utilitários e configurações
│   ├── firebase.ts             # Configuração Firebase
│   ├── api.ts                  # Cliente API
│   ├── types.ts                # Definições de tipos
│   └── validation.ts           # Esquemas de validação
└── styles/                     # Estilos adicionais
```

## 🚀 Como Executar o Projeto

### **Pré-requisitos**

- Node.js 18+
- npm ou yarn
- Conta no Firebase

### **1. Clone o repositório**

```bash
git clone https://github.com/seu-usuario/techeventos.git
cd techeventos
```

### **2. Instale as dependências**

```bash
npm install
# ou
yarn install
```

### **3. Configure as variáveis de ambiente**

Crie um arquivo `.env.local` na raiz do projeto:

```env
# Firebase Configuration
NEXT_PUBLIC_FIREBASE_API_KEY=sua_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=seu_projeto.firebaseapp.com
NEXT_PUBLIC_FIREBASE_PROJECT_ID=seu_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=seu_projeto.appspot.com
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=seu_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=seu_app_id

# API Configuration
NEXT_PUBLIC_API_URL=http://localhost:3001/api

# Other configurations
NEXT_PUBLIC_SOCKET_URL=http://localhost:3001
```

### **4. Configure o Firebase**

1. Acesse o [Console do Firebase](https://console.firebase.google.com/)
2. Crie um novo projeto
3. Ative a autenticação e configure os provedores desejados
4. Copie as configurações para o arquivo `.env.local`

### **5. Execute o projeto**

```bash
npm run dev
# ou
yarn dev
```

O projeto estará disponível em `http://localhost:3000`

## 🧪 Scripts Disponíveis

```bash
# Desenvolvimento
npm run dev          # Inicia o servidor de desenvolvimento

# Build
npm run build        # Gera build de produção
npm run start        # Inicia servidor de produção

# Qualidade de código
npm run lint         # Executa ESLint
npm run lint:fix     # Corrige problemas do ESLint automaticamente
npm run format       # Formata código com Prettier

# Testes
npm run test         # Executa testes
npm run test:watch   # Executa testes em modo watch
npm run test:coverage # Executa testes com cobertura
```

Os testes unitários utilizam **Jest** com a **React Testing Library**. Coloque
arquivos de teste com sufixo `.test.ts` ou `.test.tsx` dentro de `src/`.

## 🎨 Guia de Estilo e Padrões

### **Componentes**

- Use TypeScript para todos os componentes
- Implemente PropTypes ou interfaces TypeScript
- Siga o padrão de nomenclatura PascalCase
- Use React.forwardRef quando necessário

### **Styling**

- Utilize Tailwind CSS para estilização
- Crie componentes reutilizáveis na pasta `components/ui`
- Mantenha responsividade mobile-first
- Use variáveis CSS para temas personalizados

### **Estado e Dados**

- Use Context API para estado global
- Implemente Custom Hooks para lógica reutilizável
- Utilize React Hook Form para formulários
- Aplique Zod para validação de dados

## 🔧 Configuração Avançada

### **PWA (Progressive Web App)**

```javascript
// next.config.js
const withPWA = require("next-pwa")({
  dest: "public",
  disable: process.env.NODE_ENV === "development",
});

module.exports = withPWA({
  // suas configurações
});
```

### **Interceptadores de API**

```typescript
// lib/api.ts
api.interceptors.request.use(async (config) => {
  const token = localStorage.getItem("authToken");
  if (token) {
    config.headers.Authorization = `Bearer ${token}`;
  }
  return config;
});
```

### **Middleware de Autenticação**

```typescript
// middleware.ts
export function middleware(request: NextRequest) {
  // Lógica de autenticação
}

export const config = {
  matcher: ["/events/:path*", "/profile/:path*"],
};
```

## 📚 Principais Dependências

| Dependência      | Versão  | Finalidade                   |
| ---------------- | ------- | ---------------------------- |
| next             | ^14.0.0 | Framework React              |
| react            | ^18.0.0 | Biblioteca de UI             |
| typescript       | ^5.0.0  | Tipagem estática             |
| tailwindcss      | ^3.3.0  | Framework CSS                |
| firebase         | ^10.0.0 | Backend como serviço         |
| react-hook-form  | ^7.45.0 | Gerenciamento de formulários |
| zod              | ^3.22.0 | Validação de esquemas        |
| socket.io-client | ^4.7.0  | Cliente WebSocket            |
| date-fns         | ^2.30.0 | Utilitários de data          |
| axios            | ^1.5.0  | Cliente HTTP                 |

## 🤝 Como Contribuir

1. **Fork** o projeto
2. Crie uma **branch** para sua feature (`git checkout -b feature/nova-feature`)
3. **Commit** suas mudanças (`git commit -m 'Adiciona nova feature'`)
4. **Push** para a branch (`git push origin feature/nova-feature`)
5. Abra um **Pull Request**

### **Diretrizes de Contribuição**

- Siga os padrões de código estabelecidos
- Escreva testes para novas funcionalidades
- Documente adequadamente o código
- Use commits semânticos (Conventional Commits)

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👥 Equipe

- **Frontend**: Desenvolvido com Next.js e TypeScript
- **Design**: Interface moderna e responsiva
- **Backend**: Firebase e integração com APIs REST
- **DevOps**: Deploy automatizado e CI/CD

## ⚙️ CI/CD

O repositório possui dois fluxos de trabalho no GitHub Actions:

- **CI** (`.github/workflows/ci.yml`): executado em todo _push_ ou _pull request_ para `main`. Utiliza cache de dependências, realiza checagem de tipos, lint e build. Se houver arquivos de teste (`*.test.ts` ou `*.test.tsx`), executa `npm run test`.
- **CD** (`.github/workflows/cd.yml`): disparado quando há _push_ na branch `main` ou tags no formato `v*`. Constrói o projeto e faz o deploy no Vercel.

Para que o deploy funcione é necessário configurar os segredos `VERCEL_TOKEN`, `VERCEL_ORG_ID` e `VERCEL_PROJECT_ID` nas configurações do repositório.

### Executando localmente

```bash
npm ci
npm run lint
npm run type-check
npm run build
npm test # se houver testes
```

## 🚀 Contribuidores

Agradecemos a todos os desenvolvedores que contribuíram para tornar o TechEVentos uma realidade:

<div align="center">
  <table>
    <tr>
      <td align="center">
        <a href="https://github.com/darioreisjr">
          <img src="https://github.com/darioreisjr.png" width="100px;" alt="Dario Reis Jr"/><br />
          <sub><b>Dario Reis Jr</b></sub>
        </a>
      </td>
      <td align="center">
        <a href="https://github.com/starch0">
          <img src="https://github.com/starch0.png" width="100px;" alt="Starch0"/><br />
          <sub><b>Starch0</b></sub>
        </a>
      </td>
      <td align="center">
        <a href="https://github.com/zeneiltongpdev">
          <img src="https://github.com/zeneiltongpdev.png" width="100px;" alt="Zeneilton GP Dev"/><br />
          <sub><b>Zeneilton GP Dev</b></sub>
        </a>
      </td>
      <td align="center">
        <a href="https://github.com/rmullo">
          <img src="https://github.com/rmullo.png" width="100px;" alt="R Mullo"/><br />
          <sub><b>R Mullo</b></sub>
        </a>
      </td>
      <td align="center">
        <a href="https://github.com/viniciusbavosa">
          <img src="https://github.com/viniciusbavosa.png" width="100px;" alt="Vinicius Bavosa"/><br />
          <sub><b>Vinicius Bavosa</b></sub>
        </a>
      </td>
    </tr>
  </table>
</div>

<div align="center">
  <p>
    <strong>🌟 Quer fazer parte desta lista?</strong><br>
    Contribua com o projeto e junte-se à nossa comunidade de desenvolvedores!
  </p>
</div>

## 🆘 Suporte e Comunidade

- 📧 **Email**: contato@techeventos.com.br
- 💬 **Discord**: [Comunidade TechEventos](https://discord.gg/techeventos)
- 📱 **Telegram**: [@techeventos_brasil](https://t.me/techeventos_brasil)
- 🐦 **Twitter**: [@techeventos](https://twitter.com/techeventos)

## 🔄 Atualizações e Roadmap

### **Versão Atual: 1.0.0**

- ✅ Sistema de autenticação completo
- ✅ CRUD de eventos
- ✅ Chat em tempo real
- ✅ Sistema de perfil de usuário
- ✅ Configurações avançadas

### **Próximas Versões**

- 🔄 Sistema de avaliações e feedback
- 🔄 Integração com sistemas de pagamento
- 🔄 API móvel nativa
- 🔄 Sistema de gamificação
- 🔄 IA para recomendações personalizadas

---

<div align="center">
  <p>Feito com ❤️ pela comunidade brasileira de tecnologia</p>
  <p>
    <a href="https://techeventos.com.br">🌐 Site</a> •
    <a href="https://docs.techeventos.com.br">📖 Documentação</a> •
    <a href="https://github.com/techeventos/techeventos/issues">🐛 Reportar Bug</a> •
    <a href="https://github.com/techeventos/techeventos/discussions">💡 Ideias</a>
  </p>
</div>

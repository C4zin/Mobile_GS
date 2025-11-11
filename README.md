# 🛡️ SafeWork

### Plataforma Inteligente de Segurança e Bem-Estar no Trabalho

<p align="center">
  <img src="./assets/safework-logo.png" alt="SafeWork Logo" width="200"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React%20Native-0.81.5-blue?style=for-the-badge&logo=react" alt="React Native"/>
  <img src="https://img.shields.io/badge/Expo-54.0.23-000020?style=for-the-badge&logo=expo" alt="Expo"/>
  <img src="https://img.shields.io/badge/TypeScript-5.3-3178C6?style=for-the-badge&logo=typescript" alt="TypeScript"/>
  <img src="https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow?style=for-the-badge" alt="Status"/>
</p>

---

## 👥 Equipe de Desenvolvimento

| Nome | RM |
|------|-----|
| **Angello Turano da Costa** | 556511 |
| **Cauã Sanches de Santana** | 558317 |
| **Gustavo de Souza Amorim** | 556999 |

---

## 🎯 Sobre o Projeto

O **SafeWork** é uma plataforma mobile desenvolvida em React Native que integra tecnologia e cuidado humano para melhorar a segurança, inclusão e sustentabilidade no ambiente de trabalho. 

A solução utiliza **IA de visão computacional** para monitorar o uso de EPIs (Equipamentos de Proteção Individual) em tempo real, promovendo o bem-estar dos funcionários através de notificações inteligentes, histórico de segurança e acompanhamento de conformidade.

### 🌟 Visão Geral

Este aplicativo mobile faz parte de um ecossistema completo que inclui:
- 📱 **App Mobile React Native** (este repositório)
- 🔧 **Backend .NET API** - Autenticação, usuários e eventos
- ☕ **Backend Java Service** - Análise e comunicação com IA
- 🤖 **Visão Computacional** - Python + OpenCV + YOLOv5
- 💾 **Banco SQL** - PostgreSQL/SQL Server
- ☁️ **Cloud Deploy** - Azure/AWS com Docker

---

## ✨ Funcionalidades Implementadas

### 🔐 Autenticação e Cadastro
- Tela de login com validação de email e senha
- Tela de cadastro de novos usuários
- Sistema de contexto de autenticação (AuthContext)
- Persistência de sessão do usuário
- Logout funcional com limpeza de sessão

### 🏠 Dashboard Principal (Home)
- Visão geral com estatísticas de segurança
- Alertas de EPIs em tempo real
- Notificações de eventos importantes
- Cards informativos sobre segurança
- Navegação fluida e intuitiva

### 🦺 Gerenciamento de Equipamentos
- Lista completa de EPIs disponíveis
- Informações detalhadas sobre cada equipamento
- Status de conformidade
- Pull-to-refresh para atualizar dados
- Design responsivo e acessível

### 📋 Procedimentos e EPIs
- Seção dedicada a procedimentos de segurança
- Lista organizada de EPIs por categoria
- Descrições claras de cada item
- Ícones intuitivos para identificação rápida
- Interface moderna com cards horizontais

### ⚙️ Configurações e Perfil
- Personalização de tema (claro/escuro)
- Seleção de idioma (PT-BR, PT-PT, EN, ES)
- Gerenciamento de notificações
- Edição de perfil do usuário
- Informações de segurança da conta

### 🔔 Sistema de Notificações
- Notificações push configuráveis
- Alertas em tempo real sobre EPIs
- Histórico de notificações
- Diálogo customizado de permissões
- Integração com Expo Notifications

### 🌐 Internacionalização (i18n)
- Suporte a 4 idiomas: Português BR, Português PT, Inglês e Espanhol
- Sistema de tradução dinâmica em toda a aplicação
- Contexto de linguagem compartilhado
- Fácil adição de novos idiomas

### 🎨 Design System Consistente
- Paleta de cores personalizada (vermelho SafeWork)
- Tipografia padronizada e legível
- Componentes reutilizáveis (Button, Card, TextInput)
- Sistema de sombras e elevações modernas
- Animações e micro-interações
- Acessibilidade com labels ARIA

---

## 🛠️ Tecnologias Utilizadas

### Frontend Mobile
- **React Native** - Framework para desenvolvimento mobile
- **Expo** - Plataforma de desenvolvimento e deploy
- **TypeScript** - Tipagem estática para JavaScript
- **Expo Router** - Navegação baseada em arquivos
- **Expo Notifications** - Sistema de notificações push
- **React Context API** - Gerenciamento de estado global

### Bibliotecas e Ferramentas
- **@expo/vector-icons** - Ícones vetoriais (Ionicons, MaterialIcons, etc.)
- **expo-image-picker** - Seleção de imagens
- **expo-secure-store** - Armazenamento seguro de dados
- **React Native Safe Area Context** - Suporte a áreas seguras

### Desenvolvimento
- **ESLint** - Linter para JavaScript/TypeScript
- **Prettier** - Formatação de código
- **Git** - Controle de versão

---

## 📁 Estrutura do Projeto

\`\`\`
safework-mobile/
├── app/                          # Rotas e telas (Expo Router)
│   ├── (tabs)/                   # Abas principais do app
│   │   ├── home.tsx             # Dashboard principal
│   │   ├── equipment.tsx        # Lista de equipamentos
│   │   ├── procedures.tsx       # Procedimentos e EPIs
│   │   └── settings.tsx         # Configurações
│   ├── login.tsx                # Tela de login
│   ├── signup.tsx               # Tela de cadastro
│   ├── profile.tsx              # Perfil do usuário
│   └── _layout.tsx              # Layout raiz com providers
├── src/
│   ├── components/              # Componentes reutilizáveis
│   │   ├── button.tsx          # Botão customizado
│   │   ├── card.tsx            # Card com variantes
│   │   ├── text-input.tsx      # Input de texto
│   │   └── permission-dialog.tsx # Diálogo de permissões
│   ├── contexts/               # Contextos React
│   │   ├── auth-context.tsx   # Autenticação
│   │   ├── theme-context.tsx  # Tema claro/escuro
│   │   ├── language-context.tsx # Internacionalização
│   │   └── notification-context.tsx # Notificações
│   └── constants/              # Constantes e configurações
│       ├── colors.ts           # Paleta de cores
│       ├── theme.ts            # Tema da aplicação
│       └── index.ts            # Exports centralizados
├── assets/                      # Imagens e recursos
│   ├── safework-logo.png       # Logo do app
│   └── news-image.jpg          # Imagens de conteúdo
├── CHECKLIST_PROJETO.md        # Checklist de requisitos
├── package.json                # Dependências do projeto
└── tsconfig.json               # Configuração TypeScript
\`\`\`

---

## 🚀 Como Executar o Projeto

### Pré-requisitos
- Node.js (v18 ou superior)
- npm ou yarn
- Expo CLI
- Emulador Android/iOS ou dispositivo físico com Expo Go

### Instalação

1. Clone o repositório:
\`\`\`bash
git clone https://github.com/seu-usuario/safework-mobile.git
cd safework-mobile
\`\`\`

2. Instale as dependências:
\`\`\`bash
npm install
# ou
yarn install
\`\`\`

3. Inicie o projeto:
\`\`\`bash
npx expo start
\`\`\`

4. Execute no dispositivo:
- Escaneie o QR code com o app **Expo Go** (Android/iOS)
- Ou pressione `a` para Android Emulator
- Ou pressione `i` para iOS Simulator

### Scripts Disponíveis

\`\`\`bash
npm start          # Inicia o Expo Dev Server
npm run android    # Executa no Android
npm run ios        # Executa no iOS
npm run web        # Executa no navegador
npm run lint       # Executa o linter
\`\`\`

---

## 📱 Capturas de Tela

### Autenticação
| Login | Cadastro |
|-------|----------|
| Tela de login com validação | Cadastro de novos usuários |

### Dashboard e Funcionalidades
| Home | Equipamentos | Procedimentos |
|------|--------------|---------------|
| Dashboard com alertas | Lista de EPIs | Procedimentos de segurança |

### Configurações
| Configurações | Perfil |
|---------------|--------|
| Ajustes do app | Dados do usuário |

---

## 🏗️ Arquitetura da Solução Completa

\`\`\`
┌─────────────────┐
│  React Native   │ ← Você está aqui
│   Mobile App    │
└────────┬────────┘
         │
         ├──────────────┐
         │              │
    ┌────▼─────┐   ┌───▼──────┐
    │ .NET API │   │ Java API │
    │  (Auth)  │   │   (IA)   │
    └────┬─────┘   └────┬─────┘
         │              │
         └──────┬───────┘
                │
         ┌──────▼───────┐
         │  PostgreSQL  │
         │   Database   │
         └──────────────┘
                │
         ┌──────▼───────────┐
         │ Python + YOLO    │
         │ Visão Computacional│
         └──────────────────┘
\`\`\`

### Fluxo de Funcionamento

1. **Captura** - Câmeras capturam imagens no ambiente de trabalho
2. **Análise IA** - Python + YOLO detecta uso de EPIs
3. **Processamento** - Java Service processa resultados
4. **Registro** - .NET API grava eventos no banco
5. **Notificação** - App mobile recebe push notifications
6. **Visualização** - Usuários veem alertas e estatísticas

---

## ✅ Requisitos Atendidos (Projeto Acadêmico)

### 1. Telas e Navegação (10 pontos) ✅
- [x] Mínimo de 6 telas distintas
- [x] Navegação fluida com Expo Router
- [x] Usabilidade e acessibilidade

**Telas implementadas:**
1. Login
2. Signup (Cadastro)
3. Home (Dashboard)
4. Equipment (Equipamentos)
5. Procedures (Procedimentos)
6. Settings (Configurações)
7. Profile (Perfil) - *BÔNUS*

### 2. CRUD com API (30 pontos) ⚠️
- [ ] Operações Create, Read, Update, Delete
- [ ] Integração com API REST (.NET/Java)
- [ ] Tratamento de erros e feedback visual

**Status:** *Em desenvolvimento - Requer backend*

### 3. Sistema de Autenticação (20 pontos) ⚠️
- [x] Tela de cadastro (signup)
- [x] Tela de login
- [x] Logout funcional
- [ ] Autenticação real com API
- [ ] Proteção de rotas

**Status:** *Interface completa, aguardando integração com backend*

### 4. Estilização (5 pontos) ✅
- [x] Personalização de cores
- [x] Fontes customizadas
- [x] Identidade visual clara
- [x] Design consistente

### 5. Arquitetura (20 pontos) ✅
- [x] Organização lógica de arquivos
- [x] Nomeação clara e padronizada
- [x] Separação de responsabilidades
- [x] Código limpo e bem estruturado

### 6. Vídeo Demonstrativo (10 pontos) ⏳
- [ ] Gravação de 5 minutos
- [ ] Demonstração das funcionalidades
- [ ] Upload no YouTube

**Status:** *Pendente*

### Pontuação Estimada: 55/100
*Necessária integração com backend para CRUD e autenticação completa*

---

## 🔄 Próximos Passos

### Prioridade Alta
- [ ] Implementar integração com API .NET para autenticação
- [ ] Desenvolver operações CRUD completas
- [ ] Adicionar proteção de rotas (middleware)
- [ ] Implementar validação de formulários avançada
- [ ] Conectar com backend Java para dados de IA

### Prioridade Média
- [ ] Adicionar testes automatizados (Jest)
- [ ] Implementar cache de dados offline
- [ ] Melhorar performance com React.memo
- [ ] Adicionar modo offline first
- [ ] Implementar analytics de uso

### Prioridade Baixa
- [ ] Adicionar mais idiomas
- [ ] Implementar tour guiado para novos usuários
- [ ] Adicionar gráficos e estatísticas avançadas
- [ ] Modo de alto contraste para acessibilidade
- [ ] Suporte a biometria (FaceID/TouchID)

---

## 📚 Documentação Adicional

- [Checklist do Projeto](./CHECKLIST_PROJETO.md) - Requisitos detalhados
- [Expo Documentation](https://docs.expo.dev/)
- [React Native Documentation](https://reactnative.dev/docs/getting-started)

---

## 🤝 Contribuindo

Contribuições são bem-vindas! Para contribuir:

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/NovaFuncionalidade`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova funcionalidade'`)
4. Push para a branch (`git push origin feature/NovaFuncionalidade`)
5. Abra um Pull Request

---

## 📄 Licença

Este projeto foi desenvolvido como parte de um trabalho acadêmico para a disciplina de **Mobile Application Development**.

---

## 📞 Contato

Para dúvidas ou sugestões, entre em contato com a equipe:

- **Angello Turano da Costa** - RM 556511
- **Cauã Sanches de Santana** - RM 558317
- **Gustavo de Souza Amorim** - RM 556999

---

<p align="center">
  Desenvolvido com ❤️ pela equipe SafeWork<br/>
  © 2025 - Todos os direitos reservados
</p>

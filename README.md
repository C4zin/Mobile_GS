# 🛡️ SafeWork

### Plataforma Inteligente de Segurança e Bem-Estar no Trabalho

<p align="center">
  <img src="./assets/safework-logo.png" alt="SafeWork Logo" width="200"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React%20Native-0.81.5-blue?style=for-the-badge&logo=react" alt="React Native"/>
  <img src="https://img.shields.io/badge/Expo-54.0.23-000020?style=for-the-badge&logo=expo" alt="Expo"/>
  <img src="https://img.shields.io/badge/TypeScript-5.3-3178C6?style=for-the-badge&logo=typescript" alt="TypeScript"/>
  <img src="https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow?style=for-the-badge" alt="Protótipo"/>
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
- ☕ **Backend Java Service** - API utilizada 
- 🤖 **Visão Computacional** - Python + OpenCV + YOLOv5
- 💾 **Banco SQL** - H2

---

## ✨ Funcionalidades Implementadas

### 🔐 Autenticação e Cadastro
- Tela de login com validação de email e senha
- Tela de cadastro de novos usuários
- Sistema de autenticação (Firebase Authentication)
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

### Bibliotecas e Ferramentas
- **@expo/vector-icons** - Ícones vetoriais (Ionicons, MaterialIcons, etc.)
- **expo-image-picker** - Seleção de imagens

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
\`\`\`
git clone https://github.com/felipecvo-fiap-mad/2tdspw-gs-2-safework
\`\`\`

2. Instale as dependências:
\`\`\`
npm install
# ou
yarn install
\`\`\`

3. Inicie o projeto:
\`\`\`
npx expo start
\`\`\`

4. Execute no dispositivo:
- Escaneie o QR code com o app **Expo Go** (Android/iOS)
- Ou pressione `a` para Android Emulator
- Ou pressione `i` para iOS Simulator

### Scripts Disponíveis

\`\`\`
npm start          # Inicia o Expo Dev Server
npm run android    # Executa no Android
npm run ios        # Executa no iOS
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
8. About (Sobre o App)
9. Privacy (Privacidade)
10. support (Ajuda e suporte)
11. equipment-eddit (Editar Equipamentos)
12. equipment-register (registrar equipamento)

### 2. CRUD com API (30 pontos) ✅
- [x] Operações Create, Read, Update, Delete
- [x] Integração com API REST (Java)
- [x] Tratamento de erros e feedback visual


### 3. Sistema de Autenticação (20 pontos) ✅
- [x] Tela de cadastro (signup)
- [x] Tela de login
- [x] Logout funcional
- [x] Autenticação real com API (Firebase)
- [x] Proteção de rotas (Obrigação Logar)

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
- [x] Gravação de 5 minutos
- [x] Demonstração das funcionalidades
- [x] Upload no YouTube

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
</p>

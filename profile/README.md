# 🚀 Renoova – Sua Central de Assinaturas

O **Renoova** é uma plataforma criada para ajudar pessoas a **organizar, acompanhar e economizar** com suas assinaturas digitais – seja de **streaming, SaaS, games ou qualquer serviço recorrente**.

Nosso objetivo é simples: **colocar você no controle dos seus gastos mensais e evitar surpresas na fatura.**

---

## 🌟 O que o Renoova oferece

- 📊 **Gestão completa de assinaturas**  
  Cadastre e acompanhe todas as suas assinaturas em um só lugar.

- ⏰ **Alertas inteligentes**  
  Receba notificações por email ou push sobre renovações e vencimentos.

- 🌍 **Multilíngue e multi-fuso**  
  Configure idioma e fuso horário de acordo com sua preferência.

- 🔒 **Segurança em primeiro lugar**  
  Login seguro com autenticação JWT, refresh tokens e criptografia.

- 💡 **Planos Free e Premium**
  - **FREE**: até 4 assinaturas ativas
  - **PREMIUM**: assinaturas ilimitadas + recursos avançados (em breve)

---

## 🏗️ Estrutura do Projeto

O Renoova foi pensado como um ecossistema moderno, dividido em **front-end** e **back-end**:

### 📱 Front-end

- Desenvolvido em **Angular 17**
- Mobile-first com **Capacitor** (Android/iOS)
- Interface simples, intuitiva e responsiva

### ⚙️ Back-end

- Construído em **Java 21** com **Spring Boot 3.5**
- Hospedado no **Railway**, organizado em microserviços:

  - **renoova-srv-param**  
    Serviço principal de API, responsável por:

    - Cadastro e autenticação de usuários
    - Gerenciamento de assinaturas
    - Preferências de notificação

  - **renoova-srv-scheduler**  
    Responsável por:

    - Agendar e disparar notificações (email e push)
    - Processar assinaturas, renovando ou marcando como expiradas conforme a data cadastrada

  - **Postgres**  
    Banco de dados principal, estruturado para usuários, assinaturas e notificações

  - **Redis**  
    Cache e armazenamento temporário de tokens, sessões e filas rápidas

### 🔗 Comunicação

- APIs REST seguras
- Integração com serviços de email (Resend) e push notifications (Firebase)

---

## 🛠️ Stack Tecnológica

- **Front-end**: Angular 17, Capacitor, TypeScript
- **Back-end**: Java 21, Spring Boot 3.5
- **Banco de Dados**: PostgreSQL
- **Cache e Sessões**: Redis
- **Infraestrutura**: Railway (deploy automatizado via GitHub)
- **Notificações**: Resend (email), Firebase (push)

---

## 📈 O Futuro

Estamos desenvolvendo o **Plano Premium**, que vai incluir:

- Relatórios avançados de gastos e previsões
- Integrações inteligentes para importação automática de assinaturas
- Dashboard com insights financeiros
- Categorização de assinaturas

---

## 💡 Nossa Visão

Queremos transformar o Renoova na **plataforma de referência em gestão de assinaturas no Brasil e no mundo**, ajudando usuários a economizar tempo e dinheiro.

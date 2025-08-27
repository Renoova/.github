# Renoova – Sua Central de Assinaturas

O **Renoova** é uma plataforma criada para ajudar pessoas a **organizar, acompanhar e economizar** com suas assinaturas digitais – seja de **streaming, SaaS, games ou qualquer serviço recorrente**.

Nosso objetivo é simples: **colocar você no controle dos seus gastos mensais e evitar surpresas na fatura.**

---

## O que o Renoova oferece

- **Gestão completa de assinaturas**  
  Cadastre e acompanhe todas as suas assinaturas em um só lugar.

- **Alertas inteligentes**  
  Receba notificações por email ou push sobre renovações e vencimentos.

- **Multilíngue e multi-fuso**  
  Configure idioma e fuso horário de acordo com sua preferência.
  
---

## Mockups

<p align="center">
  <img src="https://i.imgur.com/euE5SIR.png" alt="Tela de Dashboard" width="45%" style="max-width: 360px; border-radius: 8px; margin: 0 6px;" />
  <img src="https://i.imgur.com/J3pp8B1.png" alt="Tela de Seleção de Planos" width="45%" style="max-width: 360px; border-radius: 8px; margin: 0 6px;" />
</p>

## Planos

### 🆓 Free
- Até **4 assinaturas ativas** para controle
- Notificações **pré-configuradas** por push e email sobre renovações e vencimentos
- Acesso básico à gestão de assinaturas

### ⭐ Premium (PRO)
- **Assinaturas ilimitadas** para controle
- **Categorização de assinaturas** (organize por Streaming, Games, SaaS, etc.)
- **Relatórios personalizados** de gastos, filtrados e categorizados
- **Notificações push e email personalizadas**
- **Sugestão automática de assinaturas** a partir da fatura do cartão enviada pelo usuário
- Experiência completa sem restrições

---

## Estrutura do Projeto

### Front-end (APP)

- Desenvolvido em **Angular 17**
- Mobile-first com **Capacitor** (Android/iOS)

### Back-end

- Construído em **Java 21** com **Spring Boot 3.5**
- Hospedado no **Railway**, organizado em:

  - **renoova-srv-param**  
    Serviço principal de API, responsável por:
    - Cadastro e autenticação de usuários
    - Gerenciamento de assinaturas
    - Preferências de notificação
    - Integração com pagamentos (AbacatePay)

  - **renoova-srv-scheduler**  
    Responsável por:
    - Agendar e disparar notificações (email e push)
    - Processar assinaturas, renovando ou marcando como expiradas conforme a data cadastrada

  - **Postgres**  
    Banco de dados principal, estruturado para usuários, assinaturas e notificações

  - **Redis**  
    Cache e armazenamento temporário de tokens, sessões e filas rápidas

### Comunicação Externa

- Integração com serviços de email (Resend) e push notifications (Firebase)

---

## Stack Tecnológica

- **Front-end**: Angular 17, Capacitor, TypeScript
- **Back-end**: Java 21, Spring Boot 3.5
- **Banco de Dados**: PostgreSQL
- **Cache e Sessões**: Redis
- **Infraestrutura**: Railway (deploy automatizado via GitHub)
- **Notificações**: Resend (email), Firebase (push)
- **Pagamentos**: AbacatePay (PIX)

---

## O Futuro

Estamos expandindo o **Plano Premium** com:
- Mais automações para importação de faturas
- Dashboard inteligente com insights de economia
- Sugestões personalizadas para reduzir gastos
- Melhorias contínuas na experiência de uso mobile

---

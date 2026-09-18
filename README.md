# 🤖 MIA — Minha Inteligência Artificial

<p align="center">
  <img src="frontend/public/mia-icon.png" width="120" alt="MIA">
</p>

<h3 align="center">
  Uma inteligência artificial criada para tornar sua rotina mais simples, inteligente e conectada.
</h3>

<p align="center">
  <a href="https://mia-deploy.vercel.app/">🌐 Acessar a MIA</a>
</p>

---

## ✨ Sobre a MIA

A **MIA (Minha Inteligência Artificial)** é uma plataforma de inteligência artificial desenvolvida para oferecer uma experiência moderna, simples e intuitiva de interação com uma assistente virtual.

A plataforma combina **conversas com IA, histórico de conversas, informações de clima, configurações personalizadas e integração com dispositivos**, reunindo diferentes recursos em uma única experiência.

A MIA foi desenvolvida com foco em uma interface moderna e responsiva, permitindo sua utilização tanto em **computadores quanto em dispositivos móveis**.

---

## 🚀 Funcionalidades

### 💬 Inteligência Artificial

Converse com a MIA através de uma interface de chat moderna e receba respostas geradas por inteligência artificial.

- Conversas em tempo real
- Criação de novas conversas
- Histórico de conversas
- Contexto das conversas
- Interface de chat responsiva

### 📱 Experiência Mobile

A MIA possui uma interface adaptada para dispositivos móveis, permitindo acessar suas principais funcionalidades pelo celular.

### 🌦️ Clima

Consulte informações meteorológicas através da integração com serviço de clima.

### 📺 Dispositivos

A plataforma possui estrutura para integração e controle de dispositivos compatíveis, incluindo recursos relacionados a Smart TVs.

### ⚙️ Configurações

Gerencie as configurações e preferências da sua experiência com a MIA.

### 🔐 Autenticação

Sistema de usuários com:

- Cadastro
- Login
- Autenticação
- Sessões de usuário
- Proteção de informações

---

## 🖥️ Interface

A MIA foi projetada com uma abordagem visual moderna, utilizando uma interface limpa e focada na experiência do usuário.

### Desktop

A versão para computadores aproveita o espaço disponível para apresentar o chat, histórico, navegação e demais funcionalidades.

### Mobile

A interface responsiva adapta os componentes para telas menores, mantendo a experiência de utilização da plataforma.

---

## 🛠️ Tecnologias utilizadas

### Frontend

- React
- Vite
- JavaScript
- CSS
- HTML

### Backend

- Python
- FastAPI
- Uvicorn
- Pydantic

### Inteligência Artificial

- Google Gemini API

### Banco de dados

- PostgreSQL
- Supabase
- SQLAlchemy
- Psycopg2

### Deploy

- Vercel — Frontend
- Render — Backend
- Supabase — Banco de dados

---

## 🏗️ Arquitetura

A aplicação utiliza uma arquitetura separada entre frontend e backend:

```text
                         ┌─────────────────┐
                         │      Usuário    │
                         └────────┬────────┘
                                  │
                                  ▼
                         ┌─────────────────┐
                         │     Vercel      │
                         │    Frontend     │
                         └────────┬────────┘
                                  │
                                  ▼
                         ┌─────────────────┐
                         │     Render      │
                         │     FastAPI     │
                         └───────┬─┬───────┘
                                 │ │
                  ┌──────────────┘ └──────────────┐
                  ▼                               ▼
          ┌───────────────┐               ┌───────────────┐
          │ Google Gemini │               │   Supabase    │
          │      API      │               │  PostgreSQL   │
          └───────────────┘               └───────────────┘

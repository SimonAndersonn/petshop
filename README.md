# 🐾 Petshop Dashboard – Fullstack Challenge

Dashboard web para gerenciamento de pets (CRUD), desenvolvido como parte do desafio para Desenvolvedor Fullstack Jr.

O sistema permite que usuários autenticados cadastrem, editem, visualizem e excluam animais, respeitando regras de acesso.

---

## 🚀 Tecnologias

### Backend / API
- Node.js
- Next.js (App Router)
- Prisma ORM
- PostgreSQL

### Frontend
- React
- Next.js
- TailwindCSS
- React Hook Form
- Zod

### Infraestrutura
- Docker / Docker Compose
- AWS EC2
- PostgreSQL (Container)
- GitHub

---

## 📋 Funcionalidades

- ✅ Cadastro de usuário
- ✅ Login
- ✅ Autenticação
- ✅ CRUD de Pets
- ✅ Controle de permissões
- ✅ Pesquisa por nome do pet ou dono
- ✅ Interface responsiva (Mobile First)

---

## ⚙️ Requisitos

- Docker
- Docker Compose
- Git

---

## 🖥️ Rodando Localmente (Docker)

### 1️⃣ Clone o projeto

```bash
git clone https://github.com/SEU_USUARIO/petshop.git
cd petshop

2️⃣ Configure o ambiente

Crie o arquivo .env.local:

DATABASE_URL=postgresql://petuser:petpass@db:5432/petdb
NEXTAUTH_SECRET=local-secret
NEXTAUTH_URL=http://localhost:3000

3️⃣ Suba os containers
docker-compose up -d --build

4️⃣ Execute as migrations
docker exec -it petshop_app_1 sh
npx prisma migrate dev

5️⃣ Acesse o sistema
http://localhost:3000

☁️ Deploy (Produção)

O projeto é implantado em uma instância AWS EC2 utilizando Docker.

Processo:
git pull
docker-compose down
docker-compose up -d --build

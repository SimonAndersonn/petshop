👤 Autor
Anderson Simon
📧 Email: simon.duartte@gmail.com
📱 WhatsApp: (81) 9 9565-6552

# 🐾 Petshop Dashboard – Fullstack Challenge

Dashboard web para gerenciamento de pets (CRUD), desenvolvido como parte do desafio para Desenvolvedor Fullstack Jr.

O sistema permite que usuários autenticados cadastrem, editem, visualizem e excluam animais, respeitando regras de acesso e controle de permissões.

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
- ✅ Login e autenticação
- ✅ CRUD completo de pets
- ✅ Controle de acesso por usuário
- ✅ Pesquisa por nome do pet ou dono
- ✅ Interface responsiva (Mobile First)

---

## ⚙️ Requisitos

- Node.js (>= 18)
- Docker (opcional para ambiente isolado)
- Git

---

## 🖥️ Rodando Localmente (Modo Desenvolvimento)

### 1️⃣ Clonar o repositório

```bash
git clone https://github.com/SimonAndersonn/petshop.git
cd petshop
2️⃣ Instalar dependências
npm install
3️⃣ Configurar variáveis de ambiente
Crie o arquivo .env:

DATABASE_URL=postgresql://petuser:petpass@localhost:5432/petdb
NEXTAUTH_SECRET=local-secret
NEXTAUTH_URL=http://localhost:3000

4️⃣ Executar migrations
npx prisma migrate dev
5️⃣ Iniciar servidor
npm run dev
Acesse:http://localhost:3000
🐳 Rodando com Docker
Subir ambiente completo
docker-compose up -d --build
Executar migrations
docker exec -it petshop-app-1 sh
npx prisma migrate dev
Acesse:

http://localhost:3000
☁️ Deploy (Produção – AWS)
O projeto é implantado em uma instância AWS EC2 utilizando Docker.

Processo de atualização
git pull
docker-compose down
docker-compose up -d --build
🧠 Decisões Técnicas
Uso de Docker para padronização de ambientes

Prisma para versionamento e integridade do banco

Separação entre desenvolvimento e produção

Variáveis sensíveis protegidas por .env

Build multi-stage para otimização de imagem



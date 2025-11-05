# 🏋️‍♂️ LostFit — Treino e Nutrição Natural

**Encontre sua melhor versão — naturalmente.**

LostFit é um aplicativo de treino e nutrição equilibrada, criado para quem busca resultados reais sem abrir mão do bem-estar.
Nada de dietas extremas ou treinos impossíveis — aqui, o progresso é consciente, sustentável e no seu ritmo.

## 🌿 Conceito Central
- Treinos personalizados conforme peso, idade e objetivo.
- Nutrição natural, com foco em alimentos não processados.
- Acompanhamento inteligente do progresso, com gráficos, lembretes e mensagens motivacionais.
- Modo Consciência: dicas de sono, respiração, hidratação e equilíbrio emocional.

## ⚙️ Stack Tecnológica
| Área | Tecnologia |
| --- | --- |
| Frontend | React + Vite + Tailwind CSS |
| Backend | Node.js + Express + Prisma |
| Banco de Dados | PostgreSQL (Railway) |
| Deploy | Vercel (frontend) + Railway (API) |
| Infra | Docker + Docker Compose |
| UI/UX | Figma Design System |

## 🧱 Estrutura do Projeto
```
📦 lostfit/
 ┣ 📁 repo_ready/         → Frontend (React + Vite)
 ┣ 📁 backend_boilerplate/ → API (Express + Prisma)
 ┣ 📁 prisma_migration_logs/
 ┣ 📄 railway.json        → Config Railway (API + DB)
 ┣ 📄 .env.example        → Variáveis de ambiente modelo
 ┣ 📄 vercel.env.example  → Env para Vercel
 ┣ 📄 README.md           → Este arquivo
 ┗ 📄 push_to_github.sh   → Script de push automático
```

## 🚀 Como Rodar Localmente
```bash
# Clone o repositório
git clone git@github.com:mateusbenedito0k-svg/LostFit.git
cd LostFit

# Copie as variáveis de ambiente
cp .env.example .env

# Inicie com Docker
docker compose up --build

# Rode as migrações e seeds
docker compose exec api npx prisma migrate dev --name init
docker compose exec api node prisma/seed.js

# Acesse em:
# Frontend → http://localhost:5173
# Backend → http://localhost:3333
```

## ☁️ Deploy
**Backend (Railway)**
- Crie um projeto em Railway.app.
- Importe `railway.json`.
- Configure as variáveis de ambiente (`DATABASE_URL`, `JWT_SECRET`, etc.).
- Railway cria automaticamente o Postgres e a API.

**Frontend (Vercel)**
- Importe o repositório para o Vercel.com.
- Configure:
  - `VITE_API_URL = https://<railway-api-url>`
- Deploy automático via GitHub.

## 🎨 Identidade Visual
- **Logo:** Silhueta flexionando (inspirada em Arnold) com folha fluida no tronco.
- **Cores:**
  - Verde menta #3AF7B3 — equilíbrio e vitalidade.
  - Roxo grafite #1C1135 — tecnologia e foco.
- **Tipografia:** Poppins / Montserrat
- **Ícones:** Linhas finas em verde sobre fundo escuro.

## 📈 Roadmap (3 Meses)
- **Mês 1:** Setup técnico, design system e autenticação.
- **Mês 2:** Módulos de treino, nutrição e progresso.
- **Mês 3:** Modo Consciência, dashboard completo e deploy estável.

## 🤝 Contribuição
- Pull requests e sugestões são bem-vindas!
- Para grandes mudanças, abra uma issue primeiro para discutir o que você gostaria de alterar.

## 👤 Autor
- Mateus Benedito
- 💌 Contato: @mateusbenedito0k-svg
- 🌐 Site (em breve): lostfit.app
- 📸 Instagram: @lostfitapp

**🧠 “Disciplina é liberdade — e equilíbrio é força.”**

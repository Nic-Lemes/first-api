# Primeira API 

API simples em Node.js + TypeScript usando Fastify, Drizzle ORM (PostgreSQL) e Zod. Inclui documentação Swagger/Scalar em ambiente de desenvolvimento.

## Requisitos
- Node.js 22+
- Docker e Docker Compose
- npm (ou outro gerenciador, mas o projeto usa `package-lock.json`)

## Tecnologias
- Fastify 5
- TypeScript
- Drizzle ORM + PostgreSQL
- Zod (validação)
- Swagger/OpenAPI + Scalar API Reference (em `/docs` quando `NODE_ENV=development`)

## Modelos (schema)
Tabelas principais definidas em `src/database/schema.ts`:
- `courses`
  - `id` (uuid, pk, default random)
  - `title` (text, único, obrigatório)
  - `description` (text, opcional)
- `users` (exemplo para estudos)
  - `id` (uuid, pk, default random)
  - `name` (text, obrigatório)
  - `email` (text, único, obrigatório)

## Licença
ISC (ver `package.json`).

## Considerações Finais
Projeto desenvolvido utilizando como base as aulas fornecidas pela [Rocketseat](https://app.rocketseat.com.br/?type=ALL), sendo mestradas pelo tutor [Diego Fernandes](https://github.com/diego3g).

# Case: Symphor AI

## Resumo

Projeto próprio em desenvolvimento para orquestração local-first de agentes, tarefas, governança, execução controlada e integração com canais como dashboard e Telegram.

## Problema

Fluxos com agentes de IA podem ficar difíceis de auditar quando misturam intenção, planejamento, execução, custo, permissões e histórico sem uma camada explícita de governança.

## Solução

Sistema em monorepo com dashboard, agente local, pacotes compartilhados, providers de IA, orçamento, memória, execução controlada, Prisma/Postgres e documentação de governança para evoluir automações de forma auditável.

## Funcionalidades implementadas

- Dashboard para operação e acompanhamento.
- Agente local com integração a pacotes internos.
- Estrutura de governança e documentação operacional.
- Pacotes para providers de IA, orçamento, memória, execução e regras compartilhadas.
- Prisma/Postgres para estado persistente.
- Fluxos controlados com fronteiras explícitas entre proposta, aprovação e execução.

## Stack utilizada

- TypeScript, pnpm e monorepo.
- Next.js, React, Tailwind CSS e Zod.
- Prisma, PostgreSQL e pacotes internos.
- AI SDK, OpenAI/Gemini via providers, Puppeteer e Telegram quando aplicável.

## Arquitetura resumida

Monorepo com `apps/dashboard`, `apps/local-agent`, `packages/*`, `prisma`, `docs` e scripts operacionais. A arquitetura separa interface, agente local, providers, memória, orçamento, executor e governança para reduzir risco em automações.

## Meu papel

Desenvolvimento e evolução do projeto, incluindo arquitetura do monorepo, contratos internos, dashboard, agente local, pacotes compartilhados, documentação de governança, validações e controle de escopo.

## Decisões técnicas relevantes

- Usar abordagem local-first com possibilidade de evolução para cloud.
- Separar proposta, aprovação humana e execução controlada.
- Manter documentação de governança como parte do produto.
- Evitar ativar automações sensíveis sem fronteiras e validações explícitas.

## Desafios enfrentados

- Organizar um sistema multiagente sem perder auditabilidade.
- Separar experimentação de IA de execução real.
- Manter escopo controlado em fases pequenas e verificáveis.

## Aprendizados

Projetos de automação com IA precisam priorizar governança, rastreabilidade, limites de execução, custo e revisão humana antes de ampliar autonomia.

## Status atual

Projeto próprio / em desenvolvimento. Sem dados públicos de uso.

## Links

- Repositório público: não publicado no momento.
- Case público: este documento.

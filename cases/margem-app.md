# Case: Margem App

## Resumo

SaaS para gestão de ingredientes, fichas técnicas, precificação de receitas e rotulagem nutricional.

## Problema

Negócios de alimentação precisam controlar custo de compra, rendimento, ficha técnica, preço de venda, margem e informações nutricionais. Quando isso fica em planilhas isoladas, o processo fica mais sujeito a erro e difícil de escalar.

## Solução

Aplicação web que centraliza ingredientes, receitas, precificação, rotulagem nutricional, billing, administração interna e integrações de IA em um fluxo único.

## Funcionalidades implementadas

- Cadastro e histórico de ingredientes.
- Receitas padrão e compostas.
- Simulações de precificação com histórico.
- Fluxo de tabela nutricional, snapshots e impressão.
- Multi-workspace, autenticação, billing e entitlements.
- Painel administrativo, catálogo nutricional e diagnósticos de IA.

## Stack utilizada

- Next.js, React, TypeScript e Tailwind CSS.
- Prisma, Supabase, PostgreSQL e Zod.
- OpenAI, Google GenAI, OCR e automações.
- AbacatePay, Vercel, Playwright e testes automatizados.

## Arquitetura resumida

Aplicação Next.js com rotas públicas, área autenticada, APIs internas, Prisma para modelagem de dados, Supabase/PostgreSQL como camada de dados, módulos de domínio para precificação/nutrição e integrações externas para billing e IA.

## Meu papel

Desenvolvimento full stack do projeto, incluindo arquitetura, produto, banco de dados, autenticação, billing, UI, APIs, módulos administrativos, integrações de IA, documentação e validações.

## Decisões técnicas relevantes

- Separar fluxos de ingredientes, receitas, precificação e nutrição para reduzir acoplamento.
- Tratar billing e entitlements por workspace.
- Usar cálculo determinístico para precificação e IA apenas como apoio.
- Manter documentação técnica do estado real do repositório.

## Desafios enfrentados

- Modelar dados de receitas compostas e histórico de preços.
- Integrar IA sem tornar o cálculo principal dependente de LLM.
- Organizar módulos de produto, admin e billing no mesmo SaaS.

## Aprendizados

Construção de SaaS vertical exige clareza de domínio, limites de plano, consistência de dados e separação entre automação com IA e regras determinísticas.

## Status atual

Projeto próprio / MVP funcional em produção. Métricas ainda não publicadas.

## Links

- Produção: https://margemapp.com.br/
- Repositório: https://github.com/alvaro-amorim/margem-app

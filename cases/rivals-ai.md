# Case: Rivals AI

## Resumo

Rede social de entretenimento para criação, publicação e descoberta de debates gerados por IA.

## Problema

Conteúdos gerados por IA normalmente ficam presos a uma conversa individual. Faltava uma experiência de produto que transformasse a geração em conteúdo social publicável, com feed, perfis, interações e operação administrativa.

## Solução

Aplicação web que permite criar debates entre personagens de IA, publicar o resultado como post social, descobrir conteúdos no feed, interagir com outros usuários e operar billing, tokens, curadoria e providers por painel admin.

## Funcionalidades implementadas

- Home pública, feed, discovery, temas, perfis e posts públicos.
- Arena autenticada para geração de debates.
- Streaming de debates, veredito e publicação manual.
- Reações, comentários, reposts, saves, follows e notificações.
- Billing, pacotes de tokens, planos e entitlements.
- Painel administrativo para moderação, catálogo, analytics, usuários, billing e providers.

## Stack utilizada

- Next.js, React, TypeScript e Tailwind CSS.
- Supabase Auth, Supabase Postgres e Supabase Storage.
- OpenAI, Gemini, Anthropic, xAI e Cohere.
- AbacatePay, Vitest, Playwright e Vercel.

## Arquitetura resumida

Aplicação Next.js com camada pública de descoberta, área autenticada, API routes para debate/feed/social/billing/admin, Supabase para autenticação e persistência, storage para assets e serviços de provider para geração de texto e imagem.

## Meu papel

Desenvolvimento full stack do projeto, incluindo experiência pública, arena autenticada, API routes, modelagem social, billing, tokens, integrações de IA, admin, segurança, documentação e testes.

## Decisões técnicas relevantes

- Manter o feed público como camada de aquisição e exigir login para criação/interação.
- Separar tentativa de debate, debate salvo e post publicado.
- Controlar custo por tokens e resolver débito/refund no servidor.
- Concentrar operação sensível em painel administrativo.

## Desafios enfrentados

- Conectar geração por IA com experiência social.
- Controlar custo e falhas de provider.
- Organizar permissões, moderação e billing sem fechar a navegação pública.

## Aprendizados

Produtos com IA precisam tratar geração, custo, persistência, moderação e distribuição como partes do mesmo fluxo, não apenas como chamada a um modelo.

## Status atual

Projeto próprio / em desenvolvimento com versão publicada. Métricas ainda não publicadas.

## Links

- Produção: https://www.airivals.com.br/
- Repositório: https://github.com/alvaro-amorim/RIVAL

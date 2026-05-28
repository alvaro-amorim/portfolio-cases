# Case: Comerc IAs

## Resumo

Site institucional com área administrativa, conteúdo gerenciável, analytics, upload de mídia e organização comercial.

## Problema

Um site institucional precisa comunicar oferta e portfólio com clareza, mas também precisa ser mantido com dados, cases, mídia e métricas sem exigir alteração manual de código para cada atualização.

## Solução

Aplicação Next.js com site institucional, páginas bilíngues, dashboard administrativo, APIs internas, analytics próprio, consentimento, upload de mídia e dados estruturados de portfólio e preços.

## Funcionalidades implementadas

- Site institucional com rotas e componentes organizados.
- Área administrativa reutilizada em `/pt/loginadm`.
- APIs para auth, analytics, consentimento, upload de mídia e edição de cases.
- Dados estruturados de portfólio e catálogo de preços.
- Persistência de consentimento e tracking client-side.

## Stack utilizada

- Next.js, React, TypeScript e Node.js.
- Supabase para analytics/storage conforme configuração do projeto.
- Recharts, APIs internas e Vercel.

## Arquitetura resumida

Aplicação Next.js com App Router, rotas públicas, endpoints internos para admin/analytics/upload, dados estruturados em `src/data`, tracking client-side e integrações de storage/analytics configuradas por variáveis de ambiente.

## Meu papel

Desenvolvimento full stack do projeto, incluindo estrutura do site, dashboard admin, APIs, analytics, upload de mídia, conteúdo comercial, deploy e documentação.

## Decisões técnicas relevantes

- Manter conteúdo comercial estruturado para facilitar manutenção.
- Separar tracking, consentimento e dashboard admin da camada pública.
- Usar variáveis de ambiente para integrações sensíveis.

## Desafios enfrentados

- Organizar conteúdo institucional e portfólio sem acoplar tudo à interface.
- Manter analytics e upload de mídia com configuração segura.
- Evoluir a área admin sem perder simplicidade do site público.

## Aprendizados

Sites institucionais com painel admin exigem disciplina de conteúdo, organização de dados e cuidado com autenticação, mídia e métricas.

## Status atual

MVP funcional / em produção. Métricas ainda não publicadas.

## Links

- Produção: https://www.comercias.com.br/
- Repositório: https://github.com/alvaro-amorim/Comerc.IAs

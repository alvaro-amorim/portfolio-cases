# Case: Glacê Confeitaria / Controle Glacê

## Resumo

Ecossistema web com cardápio online, checkout assistido por WhatsApp, dashboard operacional, pedidos, estoque, financeiro, cardápio e IA aplicada à rotina.

## Problema

Uma operação de confeitaria precisa receber pedidos, controlar estoque, atualizar cardápio, registrar financeiro e manter atendimento organizado. Fazer isso com planilhas e conversas soltas aumenta retrabalho e risco de erro.

## Solução

Dois projetos integrados: um storefront público para clientes fazerem pedidos e um dashboard interno para controlar operação, cardápio, pedidos, estoque, financeiro, permissões e rotinas de apoio com IA.

## Funcionalidades implementadas

- Cardápio online com home, catálogo, carrinho e checkout.
- Personalização de produtos e redirecionamento para WhatsApp com mensagem pronta.
- APIs públicas para menu, pedidos e experiência visual.
- Dashboard interno de pedidos, estoque, financeiro e cardápio.
- Autenticação, permissões, step-up auth e auditoria.
- Rotina diária com Gemini e fallback quando a IA não está configurada.

## Stack utilizada

- Storefront: React, JavaScript, React Router DOM, React Bootstrap e Vercel.
- Dashboard: Next.js, React, TypeScript, Tailwind CSS, MongoDB e Mongoose.
- Integrações: Cloudinary, Google Gemini, APIs públicas e exportação XLSX.
- Testes: Jest, React Testing Library e ts-jest.

## Arquitetura resumida

O storefront consome endpoints públicos do dashboard para carregar menu, experiência visual e registrar pedidos. O dashboard mantém MongoDB como fonte de verdade e expõe módulos internos para operação, além de contratos públicos versionados para o site.

## Meu papel

Desenvolvimento do ecossistema web, incluindo storefront, integrações públicas, dashboard, APIs, modelos de dados, autenticação, permissões, módulos operacionais, IA aplicada, documentação e deploy.

## Decisões técnicas relevantes

- Separar site público e dashboard interno em repositórios próprios.
- Usar fallbacks no storefront para manter a experiência mesmo quando APIs externas falham.
- Manter pedidos, estoque, financeiro e cardápio conectados no dashboard.
- Aplicar ações sensíveis com reautenticação e auditoria.

## Desafios enfrentados

- Integrar fluxo público de pedido com operação interna.
- Evitar quebra do storefront quando o backend estiver indisponível.
- Modelar processos operacionais reais sem transformar o MVP em sistema excessivamente complexo.

## Aprendizados

Aplicações operacionais precisam equilibrar experiência simples para o cliente, controle interno consistente e proteção de ações críticas.

## Status atual

Projeto prático / case aplicado com versões publicadas. Sem dados públicos de uso.

## Links

- Cardápio: https://cardapio-glace.vercel.app/
- Dashboard: https://controle-glace.vercel.app/
- Repositório do cardápio: https://github.com/alvaro-amorim/cardapio-glace
- Repositório do dashboard: https://github.com/alvaro-amorim/ControleGlace

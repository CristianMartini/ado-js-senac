---
titulo: Claude + MCP — automatizar tarefas com conectores
data: 2026-11-03
tags: ia, claude, mcp, automacao, conectores
status: em andamento
---

# Claude + MCP — automatizar tarefas com conectores

## Pergunta / objetivo

Entender o reel de @eu.adrian_g.s ("Deixe o Claude fazer o trabalho dele") e o
que é o "MCP", a palavra que as pessoas comentam para receber o prompt.

## Resumo

O reel não mostra uma ferramenta nova: é uma isca de engajamento ("comente MCP
que eu mando o prompt"). O assunto por trás é o **MCP (Model Context
Protocol)**, padrão aberto criado pela Anthropic que deixa o Claude se conectar
a outros apps (Gmail, Google Drive, Agenda, GitHub, Slack etc.) e agir neles.
No app do Claude, o MCP aparece com o nome de **conectores**. Não é preciso um
prompt secreto: basta ativar os conectores e pedir a tarefa em linguagem normal.

## Pontos principais

- **O que é MCP:** padrão aberto lançado pela Anthropic em novembro de 2024
  para ligar IAs a ferramentas e dados ([docs da Claude](https://claude.com/docs/connectors/building/mcp)).
- **Conectores:** no app do Claude, cada MCP vira um "conector" que se ativa
  com login, sem programar ([DEV Community](https://dev.to/arshtechpro/claude-connectors-explained-how-to-give-claude-access-to-your-tools-471k)).
- **Prontos para usar:** Google Drive, Gmail, Google Agenda, GitHub, Slack,
  Microsoft 365, entre outros ([DEV Community](https://dev.to/arshtechpro/claude-connectors-explained-how-to-give-claude-access-to-your-tools-471k)).
- **Segurança:** cada conector é autorizado separadamente; conectores
  personalizados (não verificados pela Anthropic) só devem ser adicionados se a
  fonte for confiável ([docs da Claude](https://claude.com/docs/connectors/building/mcp)).
- **Para programadores:** a API do Claude aceita servidores MCP direto na
  chamada (campo `mcp_servers`).

## Conclusões / opinião

- O "comente MCP" é tática para inflar comentários (4,6 mil); o prompt
  prometido não é necessário.
- **Você já tem isso:** nesta própria central de pesquisas o Claude tem
  conectores de Gmail, Google Drive, Google Agenda, GitHub, Figma, Vercel e
  Supabase disponíveis. Exemplos de pedidos que já funcionam:
  - "Resuma os e-mails não lidos de hoje."
  - "Procure no meu Drive a planilha X e me diga o total."
  - "Marque na minha agenda uma reunião amanhã às 15h."
- Próximo passo sugerido: escolher uma tarefa repetitiva sua e testar com um
  conector.
- Dúvida em aberto: o vídeo em si não foi assistido; só a legenda e os
  comentários foram lidos.

## Fontes

1. [Reel de @eu.adrian_g.s no Instagram](https://www.instagram.com/reel/Depdep9BQR7/) — acessado em 2026-11-03 (somente legenda e comentários)
2. [Claude Docs — MCP / conectores](https://claude.com/docs/connectors/building/mcp) — acessado em 2026-11-03
3. [DEV Community — Claude Connectors Explained](https://dev.to/arshtechpro/claude-connectors-explained-how-to-give-claude-access-to-your-tools-471k) — acessado em 2026-11-03
4. [TestingCatalog — Anthropic unveils MCP](https://testingcatalog.com/model-context-protocol-anthropic-unveils-universal-ai-data-integration-framework) — acessado em 2026-11-03

## Material original

https://www.instagram.com/reel/Depdep9BQR7/?srtk=MTFrcW9ld2k4NjFwdw==

Legenda: "Deixe o Claude fazer o trabalho dele… e veja o resultado acontecer. Comenta aqui que eu te mando o PROMPT ✅"

## Histórico

- 2026-11-03 — criada

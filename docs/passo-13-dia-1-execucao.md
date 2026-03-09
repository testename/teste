# Passo 13 — Execução prática do Dia 1 (início do site)

## Objetivo do Dia 1
Deixar o projeto com estrutura pronta e a tela de chat funcionando localmente.

## Stack escolhida (MVP)
- Front-end: Next.js (App Router)
- Back-end: Next.js API Route (temporário no Dia 1)
- Persistência: sem banco no Dia 1 (mock em memória)

---

## Etapa 1 — Criar projeto base
1. Criar app Next.js com TypeScript.
2. Validar que o projeto sobe localmente.
3. Ajustar nome do produto no layout.

**Resultado esperado:** página inicial carregando no navegador.

---

## Etapa 2 — Montar layout tipo chat
Criar os blocos:
- Header simples com nome do produto
- Área central com lista de mensagens
- Input fixo na parte inferior
- Botão de enviar

Estados visuais mínimos:
- enviando
- processando
- erro

**Resultado esperado:** interface semelhante ao fluxo de chat.

---

## Etapa 3 — Criar endpoint local de chat
Criar rota:
- `POST /api/chat`

Payload de entrada:
- `sessionId`
- `message`

Resposta inicial (mock):
- `reply`
- `provider` (ex.: `mock`)
- `latencyMs`

**Resultado esperado:** front-end envia mensagem e recebe resposta da API.

---

## Etapa 4 — Integrar front-end com API
No envio da mensagem:
1. Inserir mensagem do usuário na lista
2. Mostrar estado "processando"
3. Chamar `POST /api/chat`
4. Renderizar resposta do assistente
5. Remover estado de carregamento

**Resultado esperado:** conversa completa funcionando ponta a ponta no ambiente local.

---

## Etapa 5 — Preparar integração real (próximo dia)
Adicionar arquivo `.env.example` com chaves futuras:
- `OPENAI_API_KEY`
- `OLLAMA_BASE_URL`
- `N8N_WEBHOOK_URL`

**Resultado esperado:** projeto pronto para conectar IA real no Dia 2.

---

## Critérios de conclusão do Dia 1
- Aplicação sobe sem erro
- Chat responde via API local
- Interface responsiva básica
- Estrutura pronta para integrar ChatGPT/n8n/Ollama

---

## Estrutura de pastas sugerida
```txt
src/
  app/
    page.tsx
    api/chat/route.ts
  components/
    chat/
      chat-layout.tsx
      message-list.tsx
      chat-input.tsx
  lib/
    chat/
      client.ts
```

---

## Entregável final do Dia 1
Um protótipo navegável do seu site em estilo chat, já enviando e recebendo mensagens pela API local.

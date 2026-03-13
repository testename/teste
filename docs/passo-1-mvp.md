# Passo 1 — Definição do MVP

## Objetivo desta etapa
Definir a **primeira versão utilizável** da plataforma (MVP), com escopo pequeno, validável e pronto para evolução.

## Proposta de MVP (V1)
A V1 deve entregar apenas o essencial:

1. Tela principal em formato de chat (estilo ChatGPT)
2. Campo para o usuário enviar pedidos em texto
3. Backend com endpoint de chat (`POST /chat`)
4. Resposta automática usando 1 fluxo principal de IA
5. Histórico simples da conversa por sessão
6. Estados de interface: `enviando`, `processando`, `concluído`, `erro`

## O que entra no MVP
- Front-end básico de chat
- API de envio/retorno de mensagens
- Integração inicial com:
  - ChatGPT (modelo principal)
  - n8n (orquestração simples)
  - Ollama (fallback opcional)
- Persistência mínima (usuário/sessão/mensagens)

## O que não entra no MVP (agora)
- Multiagentes complexos
- Upload avançado de arquivos
- Painel administrativo completo
- Billing/assinatura
- Múltiplos templates de saída

## Critérios de sucesso do Passo 1
O Passo 1 estará concluído quando o time concordar e registrar:

- Escopo fechado da V1
- Lista de integrações obrigatórias
- Limites claros do que ficará para V2
- Meta de validação inicial (ex.: 10 usuários testando)

## Entregáveis desta etapa
1. Este documento de escopo
2. Lista de requisitos funcionais mínimos
3. Lista de requisitos não-funcionais mínimos

## Requisitos funcionais mínimos
- Usuário envia mensagem no chat
- Sistema retorna resposta textual
- Conversa fica salva na sessão
- Usuário consegue continuar o contexto da conversa

## Requisitos não-funcionais mínimos
- Tempo médio de resposta aceitável (meta inicial: até 15s)
- Tratamento de erro amigável ao usuário
- Logs básicos de requisição e falha
- Estrutura preparada para expansão

## Próximo passo (Passo 2)
Desenhar a arquitetura técnica (front-end, back-end, orquestrador, n8n e provedores de IA).

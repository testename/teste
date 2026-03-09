# Passo 5 — Orquestrador inteligente

## Objetivo
Implementar a lógica de decisão para escolher ferramentas por tipo de pedido.

## Responsabilidades
- Classificar intenção do usuário
- Quebrar pedidos complexos em subtarefas
- Escolher provedores (ChatGPT, Dify, EVO, Ollama)
- Gerenciar fallback quando houver falha
- Consolidar saída final ao usuário

## Estratégia inicial de roteamento
- Texto geral: ChatGPT
- Fluxos com integrações: n8n
- Dados sensíveis/local: Ollama
- Pipeline de agentes: Dify/EVO

## Entregáveis
- Módulo de decisão com regras explícitas
- Registro do provedor escolhido por requisição
- Resposta unificada independente da origem

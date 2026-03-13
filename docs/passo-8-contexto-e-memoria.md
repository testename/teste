# Passo 8 — Contexto e memória de conversa

## Objetivo
Garantir continuidade de diálogo e personalização por usuário.

## Dados mínimos a persistir
- Usuário
- Sessão
- Mensagens (user/assistant/system)
- Ferramenta usada
- Tempo de resposta
- Status da execução

## Regras de contexto
- Limite de tokens por janela de contexto
- Resumo automático de histórico longo
- Identificação de preferências do usuário

## Entregáveis
- Modelo de dados da conversa
- Estratégia de recuperação de contexto
- Política de retenção de histórico

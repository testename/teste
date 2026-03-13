# Passo 7 — Integrações com IA

## Objetivo
Conectar e padronizar o uso de ChatGPT, Dify AI, EVO AI e Ollama.

## Ordem de implementação sugerida
1. ChatGPT (motor principal)
2. Ollama (motor local/fallback)
3. Dify AI (workflows e agentes)
4. EVO AI (casos especializados)

## Padrão de integração
- Adaptador por provedor
- Timeout e retentativa por chamada
- Normalização da resposta para formato único

## Entregáveis
- Interfaces de provedor
- Chaves e variáveis de ambiente documentadas
- Testes de conexão por provedor

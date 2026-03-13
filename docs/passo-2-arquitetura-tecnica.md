# Passo 2 — Arquitetura técnica

## Objetivo
Definir a arquitetura de alto nível para garantir escalabilidade, manutenção e evolução.

## Blocos principais
1. **Front-end (Chat Web)**: interface principal do usuário.
2. **Backend API**: autenticação, sessões, histórico e orquestração.
3. **Orquestrador**: decide quais ferramentas e fluxos serão usados.
4. **n8n**: automações e integrações externas.
5. **Camada de IA**: ChatGPT, Dify AI, EVO AI, Ollama.
6. **Banco de dados**: usuários, sessões, mensagens, jobs, logs.
7. **Fila/Workers**: tarefas assíncronas longas.

## Fluxo macro
Usuário -> Front-end -> API -> Orquestrador -> (n8n/IA) -> API -> Front-end.

## Entregáveis
- Diagrama da arquitetura
- Definição de responsabilidades por serviço
- Estratégia de deploy inicial

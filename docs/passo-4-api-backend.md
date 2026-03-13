# Passo 4 — API e backend base

## Objetivo
Criar a base de serviços para receber mensagens, manter contexto e retornar respostas.

## Endpoints iniciais
- `POST /chat`: recebe prompt e devolve resposta
- `GET /chat/:sessionId/history`: retorna histórico da sessão
- `POST /chat/:sessionId/feedback`: feedback de qualidade (opcional)

## Regras mínimas
- Validação de payload
- Identificação de sessão e usuário
- Persistência das mensagens
- Tratamento padronizado de erros

## Entregáveis
- Contrato de API (OpenAPI/Swagger)
- Implementação dos endpoints do MVP
- Logs estruturados por requisição

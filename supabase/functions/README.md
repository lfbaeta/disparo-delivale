# Edge Functions

Secrets necessários no projeto Supabase:

- EVOLUTION_API_URL
- EVOLUTION_API_KEY
- GEMINI_API_KEY

Nunca salve esses valores no GitHub ou no frontend.

## Funções
- evolution-proxy: ações permitidas de status e envio de texto, autenticadas por usuário.
- gemini-reply: geração de resposta pelo Gemini, autenticada por usuário.

O webhook externo da Evolution deve ter autenticação própria antes de ser ativado em produção.

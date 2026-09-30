# Configuração final

A aplicação foi construída para que credenciais externas possam ser adicionadas depois sem alterar o frontend.

## Secrets do Supabase
Configure quando estiver pronto:

- EVOLUTION_API_URL
- EVOLUTION_API_KEY
- EVOLUTION_WEBHOOK_TOKEN
- GEMINI_API_KEY
- APP_OWNER_USER_ID

## Frontend / AI Studio
Variáveis públicas:

- VITE_SUPABASE_URL=https://qreuduvearykskaudogy.supabase.co
- VITE_SUPABASE_PUBLISHABLE_KEY=(chave publishable do projeto)

## Evolution
Configure o webhook da Evolution para chamar a função evolution-webhook e envie o header x-webhook-token com o mesmo valor de EVOLUTION_WEBHOOK_TOKEN.

## Comportamento sem credenciais
Dashboard, login, banco, listas, fila, configurações e cadastro de instâncias funcionam. Envio externo, recepção webhook e IA permanecem indisponíveis até os secrets serem preenchidos.

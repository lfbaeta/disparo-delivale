# Central Inteligente de WhatsApp — Delivale

Aplicação responsiva para operação centralizada de WhatsApp.

## Arquitetura
- React + TypeScript + Vite
- Supabase/Postgres para persistência centralizada
- Supabase Auth + RLS para acesso
- Edge Functions para chamadas protegidas à Evolution API e Gemini
- Webhook para mensagens recebidas
- Fila persistente com controle de instância, tentativas e estados

## Módulos
Dashboard, Envios, Listas, Conversas, IA, Evolution API, Instâncias e Configurações.

## Segurança
Somente URL e chave **publishable** do Supabase podem chegar ao navegador. Evolution API, Gemini e chave secret do Supabase ficam exclusivamente no backend.

## Desenvolvimento
```bash
npm install
npm run dev
npm run build
```

## Estado atual
Interface e fluxo de pré-envio implementados. Integrações reais permanecem bloqueadas até o banco dedicado e os secrets serem configurados, evitando disparos acidentais durante o desenvolvimento.

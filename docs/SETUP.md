# Setup do Workflow

## Credenciais necessárias
Criar no n8n:

- Google Sheets OAuth2
- OpenAI API
- Evolution API ou UZAPI
- Redis (opcional)

---

## Variáveis recomendadas
Defina como Environment ou direto nos nodes:

- `UZAPI_TOKEN`
- `INSTANCE_NAME`
- `GOOGLE_SHEET_ID_LEADS`
- `GOOGLE_SHEET_ID_CADENCIAS`

---

## Configurações importantes
- Delay produção: 5–7 minutos
- Limite diário: 50 envios
- Cron: Seg–Sex às 9h
- Status válidos:
  - vazio
  - Enviado1
  - Enviado2
  - Finalizado

---

## Teste seguro
Use:
- Número de teste
- Planilha duplicada
- Workflow desativado

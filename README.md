# 🦷 n8n – Campanha de Follow-up Odontológico com IA

Workflow profissional em **n8n** para automação de follow-up de pacientes,
utilizando **WhatsApp**, **IA (OpenAI)**, **RAG com Google Sheets** e controle
de cadência.

---

## 🎯 Objetivo
Automatizar o contato com pacientes que já realizaram procedimentos,
respeitando regras de cadência, personalização e limites operacionais,
evitando spam e falhas de envio.

---

## 🔄 Visão Geral do Fluxo


Trigger → Buscar Leads → Filtrar → Normalizar Telefone
→ Validar → Limitar Volume → Loop
→ Delay Inteligente → Switch de Cadência
→ IA (RAG) → Envio WhatsApp → Log no Sheets


## 🧩 Principais Funcionalidades
- ✅ Normalização de números brasileiros (fixo x móvel)
- ✅ Controle de cadência (1ª e 2ª mensagem)
- ✅ Geração de mensagens com IA (máx. 3 linhas)
- ✅ RAG com exemplos versionados em Google Sheets
- ✅ Delay aleatório entre envios (anti-bloqueio)
- ✅ Registro completo de status e data de envio
- ✅ Continuidade mesmo com erro individual

---

## ⚙️ Tecnologias
- **n8n**
- **OpenAI (LangChain Agent)**
- **Google Sheets**
- **WhatsApp API (Evolution / UZAPI)**
- **Redis (memória de conversa)**


1. Baixe `workflows/campanha_followup_janeiro.json`
2. No n8n: **Workflows → Import**
3. Configure credenciais (ver `docs/SETUP.md`)
4. Ajuste filtros (mês, limite, delay)
5. Teste manualmente
6. Ative o Cron

---

## 🔐 Segurança
Este repositório **NÃO contém**:
- Tokens
- API Keys
- Dados reais de pacientes

Veja `docs/SECURITY.md`.

---

## 📄 Licença
MIT

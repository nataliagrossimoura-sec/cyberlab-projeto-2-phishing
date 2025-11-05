# Análise 05 — TIM (Email promocional legítimo)
**Autora:** Natalia Grossi de Oliveira Costa de Moura  
**Data:** 05/11/2025  
**Arquivo de referência:** raw_emails/email_01_original.eml  
**Severidade:** Baixa  
**Tipo:** Newsletter / marketing

---

## 1. Resumo
Email promocional autêntico proveniente de plataforma de mailing. Conteúdo comercial (recarga / Pix).

## 2. Origem e Cabeçalhos
- Remetente: `tim@timpre.com.br`  
- Return-Path: `mail.tim.live.engagehub.com` (ESP legítimo)  
- SPF: Pass  
- DKIM: Pass  
- DMARC: Pass

## 3. Comportamento técnico
- Link leva a `https://timpre.com.br` — domínio consistente com campanha.  
- Layout e CTA esperados para campanha de marketing.

## 4. Conclusão & Recomendações
- ✅ Autêntico.  
- Nada a bloquear; arquivar como evidência.  
- Manter como baseline para comparação com emails spoofing.

## 5. Evidências
- `raw_emails/email_01_original.eml`  
- Screenshot: `email 01.png`

---

_Fim da Análise 05._

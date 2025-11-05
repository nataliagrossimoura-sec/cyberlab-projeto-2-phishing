# Análise 07 — Caixa Econômica (Phishing / Typosquatting)
**Autora:** Natalia Grossi de Oliveira Costa de Moura  
**Data:** 05/11/2025  
**Arquivo de referência:** raw_emails/email_03_original.eml  
**Severidade:** Alta  
**Tipo:** Typosquatting / credential harvesting

---

## 1. Resumo
Email que imita a Caixa alegando bloqueio de conta — link para `secure-cliente-cxbr.net` que captura credenciais bancárias.

## 2. Origem e Cabeçalhos
- Remetente aparenta ser `caixa@caixa.gov.br` mas Return-Path real: `mailer@contas-cliente-cx-br.com`  
- SPF: Fail  
- DKIM: None  
- DMARC: None

## 3. Comportamento técnico
- Técnica: typosquatting + linguagem de urgência para forçar clique.  
- Objetivo: roubar credenciais e possivelmente realizar BEC ou transfers.

## 4. IOCs
- Domínio malicioso: `secure-cliente-cxbr.net`  
- Return-Path fraudulento.

## 5. Classificação
- Phishing bancário — **Severidade: Alta**

## 6. Recomendações
1. Bloquear domínio/URL e IP.  
2. Inserir IOC no SIEM e nas regras de web proxy.  
3. Comunicar equipe financeira e usuários com contas sensíveis.

## 7. Evidências
- `raw_emails/email_03_original.eml`  
- Screenshot: `email 03.png`

---

_Fim da Análise 07._

# Análise 06 — AFIP (Phishing fiscal / spoofing)
**Autora:** Natalia Grossi de Oliveira Costa de Moura  
**Data:** 05/11/2025  
**Arquivo de referência:** raw_emails/email_02_original.eml (ou .txt)  
**Severidade:** Alta  
**Tipo:** Spoofing / engenharia social

---

## 1. Resumo
Email se passa pela autoridade fiscal (AFIP) e tenta induzir o usuário a abrir documento e possivelmente inserir informações. Técnica clássica de medo/urgência.

## 2. Origem e Cabeçalhos
- Aparente remetente: `afipconsultas@afip.gob.ar`  
- IP de origem observado: `5.223.58.40` (Alemanha)  
- SPF: None  
- DKIM: None  
- DMARC: Fail  
- Return-Path: `static.40.58.223.5.clients.your-server.de`

## 3. Comportamento técnico
- Link “Ver Documento Fiscal” aponta para servidor não-AFIP; possivelmente coleta de credenciais ou arquivo malicioso.  
- Mensagem utiliza linguagem institucional para gerar medo.

## 4. IOCs
- Sender IP: `5.223.58.40`  
- Fake return-path e domínio aparentes.

## 5. Classificação
- Phishing / Spoofing — **Severidade: Alta**

## 6. Recomendações
1. Bloquear IP e domínios associados.  
2. Reportar para provedor (abuse) e para CERT local.  
3. Comunicar usuários e instruir a não clicar.  
4. Preservar cabeçalhos originais e mensagem para análise forense.

## 7. Evidências
- `raw_emails/email_02_original.txt`  
- Screenshot: `email 02.png`  
- VT/scan correlacionado: `urlsacan_link02.png`

---

_Fim da Análise 06._

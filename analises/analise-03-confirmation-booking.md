# Análise 03 — confirmation055-booking.com (Phishing de reservas / cartão)
**Autora:** Natalia Grossi de Oliveira Costa de Moura  
**Data:** 05/11/2025  
**Arquivo de referência:** raw_emails/03_openphish_url_03.txt  
**Severidade:** Alta  
**Tipo:** Payment data harvesting / typosquatting

---

## 1. Resumo
Página imita Booking.com e coleta dados de cartão e reserva. Alta probabilidade de fraude financeira.

## 2. Origem e Cabeçalhos
- URL: `https://confirmation055-booking.com/YWZI9BURN`  
- Certificado TLS: válido e recente  
- VirusTotal: 22/98 (múltiplos vendors sinalizando phishing)

## 3. Comportamento técnico
- Replica visual de serviço de reservas com formulários que solicitam número do cartão.  
- Pós-submissão redireciona para armazenamento externo.  
- Usa typosquatting com sufixo numérico.

## 4. IOCs
- Domínio: `confirmation055-booking.com`  
- SPF/DKIM/DMARC quando associado ao email: None / None / Fail

## 5. Classificação & Severidade
- Phishing ativo com risco financeiro — **Severidade: Alta**

## 6. Recomendações
1. Bloquear domínio e URL em camadas de rede.  
2. Notificar time de fraude financeiro e instruir potenciais vítimas (se houver).  
3. Enviar IOC a registrador e CERT.  
4. Coletar HTML e possíveis POST endpoints e arquivar.

## 7. Evidências
- `raw_emails/03_openphish_url_03.txt`  
- VT screenshot: 22/98 (`urlsacan_link04.png`)

---

_Fim da Análise 03._

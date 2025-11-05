# Análise 04 — pay.mojdpd.si (Phishing de pagamento / sem TLS)
**Autora:** Natalia Grossi de Oliveira Costa de Moura  
**Data:** 05/11/2025  
**Arquivo de referência:** raw_emails/04_openphish_url_04.txt  
**Severidade:** Alta  
**Tipo:** Phishing — pagamento / redirecionamento

---

## 1. Resumo executivo
Página imita transportadora (DPD) pedindo pagamento de taxa de entrega. Usa HTTP (sem TLS) e redirecionamentos múltiplos — alto risco.

## 2. Origem e headers
- URL: `http://pay.mojdpd.si/Payment/DPD2001/16962033590894` (HTTP)  
- Hospedagem: IP possivelmente Eslovênia (ex.: 185.75.45.230)  
- VirusTotal: 17/98 detectores

## 3. Comportamento técnico
- Formulário de pagamento falso.  
- Sem HTTPS — tráfego em texto claro (alto risco de MITM).  
- Multiple-redirects para ocultar destino final.

## 4. IOCs
- Domínio: `mojdpd.si` e subdomínio `pay.*`  
- Headers do email (quando aplicados): SPF=None, DKIM=None, DMARC=Fail

## 5. Classificação
- Phishing com objetivo financeiro — **Severidade: Alta**

## 6. Recomendações
1. Bloquear URL/domínio em perimeter (proxy/firewall).  
2. Reportar a host/registrador e solicitar takedown.  
3. Alertar usuários e equipe de CSIRT.  
4. Se usuários clicaram, verificar logs proxy e hosts potencialmente afetados.

## 7. Evidências
- `raw_emails/04_openphish_url_04.txt`  
- VT screenshot: 17/98 (`urlsacan_link05.png`)

---

_Fim da Análise 04._

# Análise 02 — projblac.com (Login corporativo falso)
**Autora:** Natalia Grossi de Oliveira Costa de Moura  
**Data:** 05/11/2025  
**Arquivo de referência:** raw_emails/02_openphish_url_02.txt  
**Severidade:** Alta  
**Tipo:** Credential harvesting / page clone

---

## 1. Título e Contexto
Página de login clonado detectada via feed OpenPhish. Objetivo: captura de credenciais corporativas.

## 2. Origem e Cabeçalhos
- URL: `https://projblac.com/`  
- SSL/TLS: Let’s Encrypt (emitido recentemente)  
- VPS / Host: provedor genérico (país Europa Oriental)  
- VirusTotal: 11/98 (detected as phishing by multiple vendors)

## 3. Comportamento técnico
- Página replica portal corporativo (logotipos, layout).  
- Formulário de login faz `POST` para endpoint controlado pelo atacante (credential harvesting).  
- Técnica de evasão: certificado TLS válido + timing/low-volume para evitar bloqueios.

## 4. IOCs
- Domínio: `projblac.com`  
- Certificado: Let’s Encrypt (recente)  
- Auth headers (quando associado ao e-mail): SPF=None, DKIM=None, DMARC=Fail (indica mensagem distribuidora não autenticada)

## 5. Classificação
- Tipo: Phishing ativo — captura de credenciais  
- Severidade: Alta

## 6. Recomendação operativa
1. Bloquear domínio em proxy, firewall e gateway de email.  
2. Inserir IOC (domínio + URL) no SIEM e nas listas de bloqueio.  
3. Reportar para Google Safe Browsing e registrador do domínio.  
4. Coletar e preservar HTML completo da página (artefatos) para análise forense.  
5. Informar usuários/vítimas potenciais para mudar credenciais se inseridas e forçar MFA.

## 7. Evidências
- `raw_emails/02_openphish_url_02.txt`  
- Screenshot VirusTotal: 11/98 (`urlsacan_link03.png`)

---

_Fim da Análise 02._

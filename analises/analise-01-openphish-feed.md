# Análise 01 — OpenPhish Feed (Fonte de inteligência)
**Autora:** Natalia Grossi de Oliveira Costa de Moura  
**Data:** 05/11/2025  
**Arquivo de referência:** raw_emails/01_openphish_banco_2025-11-05.txt  
**Severidade:** Baixa  
**Tipo:** URL / Feed de inteligência

---

## 1. Resumo Executivo
Fonte legítima (OpenPhish) que publica feeds de URLs de phishing para análise. Não é um ataque direcionado ao remetente — é um repositório de amostras para pesquisa. Uso seguro: apenas em laboratório/sandbox.

## 2. Origem e Cabeçalhos
- URL analisada do feed: `https://openphish.com/phishing_feeds.html`  
- HTTP Status: 200 OK  
- Certificado TLS: válido (emitido para OpenPhish LLC)  
- VirusTotal: 0/98 detectores sinalizando o feed (o feed lista URLs externas que podem ser maliciosas)

## 3. Comportamento técnico
- Conteúdo: lista/arquivo texto com URLs coletadas e verificadas por OpenPhish.  
- A lista contém referências para sites maliciosos — **não** abrir links fora de ambiente controlado.  
- Objetivo do ativo: inteligência / coleta de amostras para analistas.

## 4. IOCs e evidências
- Domínio fonte: `openphish.com` (legítimo)  
- Arquivo: `raw_emails/01_openphish_banco_2025-11-05.txt`  
- Evidência adicional: screenshot VT/scan (incluir `urlsacan_link01.png`)

## 5. Classificação
- Tipo: Feed de Phishing (inteligência)  
- Severidade operacional: Baixa (para o feed), mas **cada URL listada deve ser tratada individualmente**.

## 6. Recomendações
1. Armazenar feed apenas em ambiente de laboratório (VM isolada).  
2. Importar somente IOCs validados para SIEM/Feeder com regras de sandboxing.  
3. Não clicar em URLs do feed sem sandbox.  
4. Documentar data e versão do feed quando usar como evidência.

---

_Fim da Análise 01._

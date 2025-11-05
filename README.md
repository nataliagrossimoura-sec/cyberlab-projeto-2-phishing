# cyberlab-projeto-2-phishing
Laboratório completo de análise e prevenção de ataques de phishing (coleta, análise técnica, user awareness e relatório executivo).
# 🧠 CYBERLAB — PROJETO 2: PHISHING  
**Laboratório Completo de Análise e Prevenção de Ataques de Phishing**

---

## 🛡️ Dados do Projeto

- **Título:** Análise e Prevenção de Ataques de Phishing  
- **Autora:** Natália Grossi de Oliveira Costa de Moura  
- **Local:** Belo Horizonte – MG  
- **Data:** Novembro de 2025  
- **Trilha:** Portfólio SOC / Analista de Segurança Cibernética  

---

## 📌 Sobre o Projeto

Este projeto faz parte do meu **laboratório de cibersegurança** e tem como objetivo **analisar tecnicamente** campanhas de phishing reais, **documentar vetores, cabeçalhos e domínios maliciosos**, e criar **materiais de conscientização corporativa** que transformam os achados técnicos em aprendizado prático.

O projeto está dividido em **quatro partes principais:**
1. 🧩 **Análises técnicas individuais (1–8)** — cada uma examinando um ataque real.  
2. 📊 **Checklist de Phishing** — modelo de verificação usado em investigações.  
3. 🧾 **Relatório Técnico de Análise e Prevenção** — documento consolidado e visual.  
4. 💡 **Plano de Conscientização para PMEs** — ação educativa derivada dos achados técnicos.

---

## 🧠 Estrutura do Repositório

cyberlab-projeto-2-phishing/
├── README.md
├── /analise
│ ├── analise_01.md
│ ├── analise_02.md
│ ├── analise_03.md
│ ├── analise_04.md
│ ├── analise_05.md
│ ├── analise_06.md
│ ├── analise_07.md
│ └── analise_08.md
├── /docs
│ ├── Checklist_Phishing.pdf
│ ├── Relatorio_Analise_e_Prevencao_de_Ataques_de_Phishing.pdf
│ ├── Plano_Conscientizacao_PMEs.pdf
│ └── Plano_Conscientizacao_PMEs.pptx
├── /conhecimento
│ └── (em construção)

---

## 🔍 Análises Técnicas (1–8)

Cada análise aborda uma amostra real coletada de fontes públicas e e-mails reais, com os seguintes componentes:

| Nº | Categoria | Tema | Técnica Identificada | Severidade | Relatório |
|----|------------|-------|----------------------|-------------|------------|
| 1 | Bancário | Falso acesso Itaú | Spoofing + Link Malicioso | Alta | [analise_01.md](analise/analise_01.md) |
| 2 | E-commerce | Pagamento em atraso | Engenharia Social | Média | [analise_02.md](analise/analise_02.md) |
| 3 | Governo | Multa DETRAN falsa | Domínio homógrafo | Alta | [analise_03.md](analise/analise_03.md) |
| 4 | Corporativo | Atualização de Senha | Spoof de domínio | Alta | [analise_04.md](analise/analise_04.md) |
| 5 | Entrega | Correios – Entrega Pendente | Encurtador + malware ZIP | Alta | [analise_05.md](analise/analise_05.md) |
| 6 | Financeiro | Nota Fiscal – NF-e | PDF malicioso | Alta | [analise_06.md](analise/analise_06.md) |
| 7 | Streaming | Assinatura Netflix | Phishing genérico | Média | [analise_07.md](analise/analise_07.md) |
| 8 | Tecnologia | Suporte Microsoft | Engenharia de autoridade | Média | [analise_08.md](analise/analise_08.md) |

Cada arquivo `.md` contém:
- Análise de cabeçalhos (SPF/DKIM/DMARC)  
- Rastreio de origem (Received Headers)  
- Inspeção de links (URLScan / VirusTotal)  
- Capturas de tela de e-mails e URLs  
- Avaliação de severidade e recomendações  

---

## ✅ Checklist de Phishing

📄 **Arquivo:** `/docs/Checklist_Phishing.pdf`

Um guia prático com perguntas de verificação rápida, para uso tanto em treinamentos quanto em triagem real.  
Inclui:

- Verificação de remetente e domínio  
- Sinais linguísticos e psicológicos (urgência, medo, autoridade)  
- Links, anexos e certificados SSL  
- Ações pós-identificação: reportar, isolar e responder  

---

## 🧾 Relatório Técnico de Análise e Prevenção de Ataques de Phishing

📂 **Local:** `/docs/Relatorio_Analise_e_Prevencao_de_Ataques_de_Phishing.pdf`

O relatório consolida os resultados das 8 análises, trazendo:
- Estatísticas e padrões por tipo de ataque  
- Indicadores observáveis (IOCs)  
- Recomendações para usuários e empresas  
- Fluxo de ataque (Kill Chain)  
- Frameworks utilizados (MITRE ATT&CK, NIST SP 800-61)  
- Métricas de mitigação e aprendizado  

---

## 💡 Plano de Conscientização de Segurança para PMEs

📘 **Local:** `/docs/Plano_Conscientizacao_PMEs.pdf`  
📊 **Versão em Apresentação:** `/docs/Plano_Conscientizacao_PMEs.pptx`

Criação de um programa anual de educação em segurança voltado a pequenas e médias empresas.  
Inclui cronograma de treinamento, métricas de sucesso, orçamento e recursos necessários.


---

## 🧩 Integração com o Laboratório "Entendendo o Phishing"

As análises deste projeto são complementares ao **Projeto 1 — Entendendo o Phishing**, que foca na coleta e classificação de e-mails e URLs.  
Os dados obtidos lá são utilizados aqui para:
- Montar as análises técnicas;  
- Alimentar a planilha de amostras (`project_phishing_entendendo_samples.csv`);  
- Criar simulações e cenários de conscientização.

---

## 🧠 Conhecimento (em desenvolvimento)

A pasta `/conhecimento/` será usada para incluir:
- Conceitos resumidos de engenharia social  
- Explicações sobre protocolos SPF, DKIM e DMARC  
- Guias de mitigação e resposta  

---

## 🧰 Ferramentas Utilizadas

- **Análise técnica:** MXToolbox, VirusTotal, URLScan.io, Any.Run  
- **Documentação:** Typora, Canva, draw.io  
- **Conscientização:** Canva, PowerPoint  
- **Coleta de amostras:** PhishTank, OpenPhish  
- **Referências:** APWG, Verizon DBIR, CERT.br, Microsoft, KnowBe4  

---

## 🎯 Impacto e Objetivo

- Demonstrar **capacidade de análise e documentação técnica** com base em amostras reais.  
- Traduzir achados técnicos em **planos de conscientização corporativa**.  
- Consolidar material de portfólio para **vagas de SOC e Analista de Segurança Cibernética**.  

---

✍️ **Natália Grossi de Oliveira Costa de Moura**  
Cibersegurança • Documentação Técnica • Laboratório Próprio  
📍 Belo Horizonte – MG | Novembro 2025

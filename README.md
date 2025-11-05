# cyberlab-projeto-2-phishing
Laboratório completo de análise e prevenção de ataques de phishing (coleta, análise técnica, user awareness e relatório executivo).
# 🛡️ PROJETO 2 – Laboratório de Cibersegurança
## Análise e Prevenção de Ataques de Phishing

**Autora:** Natalia Grossi de Oliveira Costa de Moura  
**Local:** Belo Horizonte – MG  
**Data:** Novembro de 2025  
**Trilha:** Portfólio SOC / Cybersecurity Analyst

---

## 📌 Sobre o projeto
Este projeto faz parte do meu laboratório de cibersegurança e tem como objetivo documentar, de forma técnica e prática, como os ataques de phishing são realizados hoje (2024–2025), por que continuam sendo o vetor nº 1 de incidentes e quais controles uma organização e um usuário podem aplicar para reduzir o risco.

O relatório completo foi escrito em formato profissional e pode ser usado em portfólio, entrevistas e como material de conscientização interna.

👉 **Relatório completo:** `docs/Relatorio_Analise_e_Prevencao_de_Ataques_de_Phishing.pdf`  

---

## 🧠 Sumário executivo
- Phishing foi responsável por **cerca de 36%** das violações de dados em 2024 (Verizon DBIR 2024).
- O APWG registrou **mais de 5 milhões de ataques de phishing no 1º semestre de 2024**, com aumento de 58% ano a ano.
- O fator humano continua sendo o elo mais fraco: organizações sem treinamento têm taxa de clique entre **25% e 40%**; após programas de conscientização, esse número cai para **menos de 5%**.
- Ataques direcionados (**spear phishing** e **whaling**) têm taxa de sucesso até **10x maior** que o phishing genérico.
- A defesa eficaz exige **camadas técnicas (SPF/DKIM/DMARC, e-mail gateway, bloqueio de domínios novos)** + **camada humana (treinamento, simulação, cultura de reporte)**.
- O projeto também descreve um **plano de resposta** para quando o usuário já clicou.

---

## 🏗 Estrutura do relatório
O relatório técnico está organizado assim:

1. **Introdução**
   - Conceito de phishing e engenharia social
   - Por que o phishing ainda funciona
   - Cenário 2024–2025 (Verizon, APWG, CERT.br)

2. **Tipos de Phishing**
   - Email phishing (genérico)
   - Spear phishing (direcionado)
   - Whaling (C-level)
   - Smishing (SMS)
   - Vishing (voz)
   - Clone phishing
   - Tabela comparativa por sofisticação, taxa de sucesso e alvo

3. **Anatomia de um Ataque (Kill Chain do Phishing)**
   - Reconnaissance (OSINT)
   - Elaboração da isca (domínio similar, página clone)
   - Entrega (bypass de gateways)
   - Exploração (clique, download, resposta)
   - Coleta e persistência

4. **Indicadores Técnicos**
   - Headers suspeitos
   - Domínios parecidos (typosquatting e homógrafos)
   - Certificados SSL falsos/recém-criados
   - Redirecionamentos múltiplos e encurtadores

5. **Estratégias de Prevenção**
   - **Camada técnica:** SPF, DKIM, DMARC, sandboxing, filtros com ML, bloqueio de domínios recém-registrados
   - **Camada humana:** treinamentos, simulações recorrentes, botão “reportar phishing”, cultura de segurança

6. **Plano de Resposta a Incidentes**
   - O que o usuário faz se clicou
   - O que o time de segurança faz para conter e investigar
   - Monitoramento por 72h

7. **Conclusão e recomendações**
   - Segurança como processo contínuo
   - Integração tecnologia + pessoas
   - Compartilhamento de IOCs

---

## 📊 Diagrama do fluxo do ataque

```text
[1. Reconhecimento / OSINT]
          |
          v
[2. Elaboração da isca]
(domínio similar, página clone,
mensagem com urgência/autoridade)
          |
          v
[3. Entrega]
(e-mail, SMS, WhatsApp ou ligação)
          |
          v
[4. Exploração]
(vítima clica / baixa / responde)
          |
          v
[5. Coleta de dados]
(credenciais capturadas, malware,
acesso inicial ao ambiente)

🛠 Ferramentas e referências sugeridas
Ferramentas: MXToolbox, VirusTotal, URLVoid/CheckShortURL, draw.io/Canva (diagramas)

Fontes sólidas:
APWG – Phishing Activity Trends Report, Q2 2024
Verizon – 2024 Data Breach Investigations Report (DBIR)
Google – Email Security Statistics 2024
CERT.br – Estatísticas de Incidentes de Segurança no Brasil, 2024
Microsoft – Digital Defense Report, 2024
KnowBe4 – Phishing by Industry Benchmarking Report, 2024

🧩 Como este projeto se encaixa no meu portfólio
Faz parte da minha série de 8 projetos práticos de cibersegurança.
Demonstra capacidade de análise, documentação técnica e tradução de ameaça para controle (habilidade muito pedida em vagas de SOC e Analista de Segurança).
Pode ser citado no LinkedIn e no currículo como:
“Elaboração de relatório técnico sobre análise e prevenção de ataques de phishing, com abordagem em camadas (técnica e humana), baseado em dados de 2024–2025 e referências APWG/Verizon.”

✍️ Natalia Grossi de Oliveira Costa de Moura
Cibersegurança • Documentação técnica • Laboratório próprio

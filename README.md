# 📊 IT Help Desk Operations — Análise Estratégica 2026

> **Análise exploratória de +25.000 tickets de suporte para identificar gargalos operacionais e propor melhorias na alocação de recursos.**

---

## 🗂️ Sobre o Projeto

Este projeto faz parte do meu portfólio em construção como Analista de Dados Jr. O objetivo foi ir além dos gráficos e responder perguntas reais de negócio:

- Quais departamentos concentram mais chamados críticos?
- A distribuição de prioridades está equilibrada com a capacidade da equipe?
- Onde estão os principais gargalos que afetam o SLA?

---

## 🔍 Perguntas de Negócio Respondidas

| # | Pergunta | Visualização |
|---|----------|-------------|
| 1 | Como se distribui o volume de tickets por prioridade? | Barplot — Prioridades |
| 2 | Quais departamentos geram mais demanda? | Barras horizontais |
| 3 | Há concentração de tickets críticos em setores específicos? | Stacked Bar Chart |
| 4 | Quais tags/palavras-chave dominam os tickets High Priority? | Análise de frequência |

---

## 📁 Estrutura do Repositório

```
helpdesk-ops-insights/
│
├── 📓 IT_TICKETS_Analysis.ipynb     ← Notebook principal (EDA completa)
├── 📊 presentation/
│   └── IT_HelpDesk_2026.pdf         ← Apresentação executiva (Google Slides)
├── 📈 dashboard/
│   └── looker_dashboard_link.md     ← Link do dashboard interativo
├── 🖼️ exports/
│   ├── slide3_prioridades.png
│   ├── slide4_departamentos.png
│   └── slide5_stacked_bar.png
└── 📄 README.md
```

---

## 🛠️ Stack Utilizada

| Ferramenta | Uso |
|-----------|-----|
| **Python 3** | Linguagem principal |
| **Pandas** | Limpeza e manipulação de dados |
| **Matplotlib** | Customização visual |
| **Seaborn** | Visualizações estatísticas |
| **Google Colab** | Ambiente de desenvolvimento |
| **Looker Studio** | Dashboard interativo |
| **Google Slides** | Apresentação executiva |

---

## 📊 Dataset

- **Fonte:** [IT Support Ticket Data — Kaggle](https://www.kaggle.com/datasets/parthpatil256/it-support-ticket-data)
- **Registros:** 25.000+ tickets
- **Colunas:** `Department`, `Priority`, `Tags`, `Body`
- **Prioridades:** High · Medium · Low

---

## 🔑 Principais Insights

> **1. Concentração de demanda:** Technical Support concentra o maior volume de tickets, especialmente críticos (High Priority), criando um gargalo estrutural.

> **2. Pressão no SLA:** 28% dos tickets são High Priority. Em um contexto de recursos compartilhados, isso compromete diretamente os acordos de nível de serviço.

> **3. Desequilíbrio por setor:** Departamentos como Human Resources e General Inquiry têm volume baixo mas concentração alta de prioridades críticas — risco invisível para a gestão.

---

## 📌 Como Executar

```bash
# 1. Clonar o repositório
git clone https://github.com/seu-usuario/helpdesk-ops-insights.git

# 2. Abrir no Google Colab
# Faça upload do .ipynb ou abra direto pelo link do Colab

# 3. Instalar dependência (se necessário)
pip install kagglehub
```

---

## 📈 Dashboard Interativo

🔗 [Acessar Dashboard no Looker Studio](#) ← *(link será adicionado)*

---

## 👩‍💻 Autora

**Niafre Guerra**
Analista de Dados em formação · Brasil

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](https://linkedin.com/in/seu-usuario)
[![Kaggle](https://img.shields.io/badge/Kaggle-Profile-blue?style=flat&logo=kaggle)](https://kaggle.com/seu-usuario)

---

## 🚀 Próximos Passos

- [ ] Análise de sentimento no campo `Body` dos tickets
- [ ] Modelo de classificação automática de prioridade (ML)
- [ ] Dashboard em Tableau como complemento

---

*Este projeto é parte do meu portfólio profissional. Feedbacks são bem-vindos!*

# IT Help Desk Operations — Análise Estratégica 2026

[![Python](https://img.shields.io/badge/Python-3.x-1B4F8C?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?style=flat-square&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualização-11557C?style=flat-square)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-Visualização-4C72B0?style=flat-square)](https://seaborn.pydata.org/)
[![Colab](https://img.shields.io/badge/Google_Colab-Notebook-F9AB00?style=flat-square&logo=googlecolab&logoColor=white)](https://colab.research.google.com/)
[![Dashboard](https://img.shields.io/badge/Dashboard-Em_Desenvolvimento-F0A500?style=flat-square&logo=looker&logoColor=white)](#dashboard)
[![Análise](https://img.shields.io/badge/Análise-Concluída-27AE60?style=flat-square)]()
[![Portfólio](https://img.shields.io/badge/Portfólio-Projeto_1-0D2B5E?style=flat-square)]()

> Análise exploratória de **29.651 tickets** de suporte de TI para identificar gargalos operacionais e propor melhorias na alocação de recursos.
>
> *Primeiro projeto do meu portfólio em Data Science — do dado bruto ao insight de negócio.*

---

## Sobre o Projeto

Este projeto responde 4 perguntas reais de negócio usando dados de Help Desk:

1. Como se distribui o volume de tickets por nível de prioridade?
2. Quais departamentos concentram mais chamados?
3. Há setores com alta taxa de tickets críticos, independente do volume total?
4. Quais palavras-chave dominam os chamados urgentes?

---

## Principais Descobertas

| Insight | Dado | Impacto |
|--------|------|---------|
| **Technical Support** concentra volume e criticidade | 29% do total + 58% dos tickets High Priority | Alto — gargalo estrutural |
| **Service Outages** — risco desproporcional | 1.157 tickets, mas 70,7% são High Priority | Crítico — invisível no volume |
| **3 departamentos** acima da média de risco | IT Support 47,3% · Tech Support 58,4% · Svc Outages 70,7% | Médio — requer SLAs próprios |
| **Padrões recorrentes** nos chamados críticos | Bug · Performance · Disruption dominam os High Priority | Oportunidade de automação |

---

## Visualizações

| # | Título | Tipo | Campo |
|---|--------|------|-------|
| 1 | Distribuição de Criticidade | Barplot vertical com % | `priority` |
| 2 | Concentração de Demanda por Setor | Barras horizontais | `department` |
| 3 | Mapa de Criticidade Operacional | Stacked bar chart | `department` × `priority` |
| 4 | Risco Oculto por Departamento | Barras com linha de média | `priority` / `department` |
| 5 | Top Tags — Geral vs High Priority | Duplo barplot horizontal | `tags` |

---

## Dashboard — Em Desenvolvimento <a name="dashboard"></a>

> **Looker Studio · Em construção 🚧**

O dashboard interativo está sendo desenvolvido no Looker Studio com filtros dinâmicos por departamento e prioridade. Link será adicionado quando publicado.

**Métricas planejadas:**
- Scorecards de total · High · Medium · Low + taxa média de criticidade
- Volume por departamento com filtro interativo
- Mix de prioridade (gráfico de rosca)
- Mapa de criticidade empilhado (stacked bar)
- Risco oculto com linha de corte na média (32,1%)
- Top tags dos chamados High Priority

---

## Stack

| Ferramenta | Uso |
|-----------|-----|
| Python 3 | Linguagem principal |
| Pandas | Limpeza e manipulação de dados |
| Matplotlib | Customização visual e exportação |
| Seaborn | Visualizações estatísticas |
| Google Colab | Ambiente de desenvolvimento |
| Looker Studio | Dashboard interativo *(em desenvolvimento)* |
| Google Slides | Apresentação executiva — 10 slides |

---

## Dataset

- **Fonte:** [IT Support Ticket Data — Kaggle](https://www.kaggle.com/datasets/parthpatil256/it-support-ticket-data)
- **Registros:** 29.651 tickets
- **Campos:** `Department` · `Priority` · `Tags` · `Body`
- **Prioridades:** High · Medium · Low
- **Departamentos:** 10 setores

---

## Estrutura do Repositório

```
helpdesk-ops-insights/
│
├── IT_TICKETS_Analysis_v2.ipynb                    ← Notebook principal (EDA completa)
├── Análise de Performance_Service Desk 2026.pdf    ← Apresentação executiva (10 slides)
└── README.md
```

---

## Como Executar

```bash
# Clonar o repositório
git clone https://github.com/niafredev/helpdesk-ops-insights.git
```

Depois abra `IT_TICKETS_Analysis_v2.ipynb` no [Google Colab](https://colab.research.google.com/) e execute todas as células com `Runtime → Executar tudo`.

---

## Recomendações da Análise

1. **Rebalancear a alocação no Technical Support** — maior volume e maior criticidade simultâneos exigem reforço ou triagem automatizada
2. **Criar SLAs diferenciados por departamento** — a média geral de 32,1% mascara situações de risco real
3. **Automatizar triagem dos chamados recorrentes** — Bug, Performance e Disruption são problemas sistemáticos com solução documentável
4. **Dashboard em tempo real** — monitoramento semanal de prioridade por departamento *(próximo passo)*

---

## Próximos Passos

- [ ] Publicar dashboard no Looker Studio
- [ ] Análise de sentimento no campo `Body` dos tickets (NLP)
- [ ] Modelo de classificação automática de prioridade (ML)

---

## Autora

**Niafre Guerra** — Analista de Dados em formação · Brasil

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Niafre_Guerra-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/niafre-guerra-561845330/)
[![Kaggle](https://img.shields.io/badge/Kaggle-niafredev-20BEFF?style=flat-square&logo=kaggle&logoColor=white)](https://www.kaggle.com/niafreguerra)
[![GitHub](https://img.shields.io/badge/GitHub-niafredev-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/niafredev)

---

*Este projeto nasceu do meu processo de aprendizado. Cada visualização foi pensada para contar uma história com os dados — não apenas mostrar um número. Feedbacks são muito bem-vindos!*

# Introdução prática a Machine Learning com scikit-learn

[![Abrir no Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/samuelfsd/intro-ml/blob/main/notebooks/01_introducao_ml.ipynb)

Plano de aula / material de estudo com uma revisão básica e prática de Machine Learning, para
alunos de graduação que estão começando na Iniciação Científica.

O foco é o **fluxo básico**, sem entrar em avaliação de modelos:

1. **Carregar** um dataset (CSV) e **visualizar** as features
2. **Tratar** os dados (colunas inúteis, duplicatas, valores faltando, outliers, texto → número)
3. **Separar** `X` e `y` e **dividir** em treino, teste e produção
4. **Treinar** modelos simples do scikit-learn: Regressão Linear, Árvore de Decisão e Floresta Aleatória
5. **Prever**: dados de teste, dados de "produção" e uma pessoa nova

## Plano de aula

| etapa | conteúdo | tempo sugerido |
|---|---|---|
| 0 | O que é um modelo? Regressão x classificação (conversa, fora do notebook) | 5 min |
| 1 | Carregar o dataset no formato do scikit-learn (`.data`, `.target`, `.feature_names`, `.target_names`) | 10 min |
| 2 | Visualizar as features (`info`, `describe`, histogramas, gráficos) | 10 min |
| 3 | Tratamento: colunas inúteis, duplicatas, faltantes, outliers, one-hot | 15 min |
| 4 | Separar `X` (entradas) e `y` (alvo) | 5 min |
| 5 | Divisão treino / teste / produção | 10 min |
| 6 | Treinar Regressão Linear, Árvore de Decisão e Floresta Aleatória | 10 min |
| 7–8 | Predições: teste, produção, pessoa nova, salvar/carregar o modelo | 15 min |
| — | Exercícios e próximos passos (métricas de avaliação) | — |

## Dataset

[maxfactor71/Employee_Performance_Salary](https://huggingface.co/datasets/maxfactor71/Employee_Performance_Salary)
(Hugging Face): ~1000 funcionários com idade, gênero, departamento, anos de experiência, nota de desempenho e salário.

O notebook lê o CSV direto da URL do Hugging Face. Uma cópia está em [`data/`](data/) para uso offline.

## Como rodar

**Google Colab (sem instalar nada):** clique no botão "Abrir no Colab" acima.

**Localmente, com [uv](https://docs.astral.sh/uv/):**

```bash
uv sync
uv run jupyter lab notebooks/01_introducao_ml.ipynb
```

## Estrutura

```
.
├── data/
│   └── employee_performance.csv     # cópia local do dataset
├── notebooks/
│   └── 01_introducao_ml.ipynb       # notebook da aula
├── pyproject.toml
└── uv.lock
```

## Próximos passos (para estudar depois)

- Métricas de avaliação de regressão: MAE, RMSE, R²
- Overfitting e underfitting
- Validação cruzada (`cross_val_score`)
- Documentação do scikit-learn: <https://scikit-learn.org/stable/getting_started.html>

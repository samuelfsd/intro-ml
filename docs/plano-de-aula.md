# Plano de aula

Revisão básica e prática de Machine Learning para alunos de graduação começando na Iniciação Científica.
O foco é o **fluxo básico**, sem entrar em avaliação de modelos.

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
| — | Exercícios e próximos passos | — |

## Próximos passos (para estudar depois)

- Métricas de avaliação de regressão: MAE, RMSE, R²
- Overfitting e underfitting
- Validação cruzada (`cross_val_score`)
- Documentação do scikit-learn: <https://scikit-learn.org/stable/getting_started.html>

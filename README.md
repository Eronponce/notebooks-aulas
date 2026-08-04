# Notebooks das aulas

Blocos práticos das disciplinas, publicados aqui para abrirem direto no Google Colab a partir dos slides. Cada notebook é autocontido: roda de cima para baixo, sem depender de arquivo externo, e usa semente fixa para que todo mundo veja os mesmos números.

## Otimizações em Machine Learning

Disciplina CIA@1036 — Técnicas Avançadas de Machine Learning.

| Notebook | O que demonstra |
|:---------|:----------------|
| [U1 · Aula 01 — a curva em U](https://colab.research.google.com/github/Eronponce/notebooks-aulas/blob/main/otimizacoes-em-machine-learning/u1_bloco_pratico_aula01_curva_em_u.ipynb) | Erro de treino cai sempre; o de validação desenha um U. O sobreajuste visto de perto. |
| [U1 · Aula 02 — métricas sob desbalanceamento](https://colab.research.google.com/github/Eronponce/notebooks-aulas/blob/main/otimizacoes-em-machine-learning/u1_bloco_pratico_aula02_metricas_desbalanceamento.ipynb) | Três modelos com acurácia parecida e qualidade radicalmente diferente. |
| [U2 · Aula 01 — SMOTE dentro e fora do pipeline](https://colab.research.google.com/github/Eronponce/notebooks-aulas/blob/main/otimizacoes-em-machine-learning/u2_bloco_pratico_aula01_smote_vazamento.ipynb) | O vazamento não melhora o modelo, infla o termômetro: 0,858 prometido contra 0,502 entregue. |
| [U2 · Aula 02 — Grid vs Random sob nested CV](https://colab.research.google.com/github/Eronponce/notebooks-aulas/blob/main/otimizacoes-em-machine-learning/u2_bloco_pratico_aula02_grid_vs_random.ipynb) | Empate técnico com um terço do orçamento, e o selection bias medido ao vivo. |
| [U3 · Aula 01 — TPE vs Random no Optuna](https://colab.research.google.com/github/Eronponce/notebooks-aulas/blob/main/otimizacoes-em-machine-learning/u3_bloco_pratico_aula01_tpe_vs_random.ipynb) | Mesmo troféu, comportamentos opostos: o TPE termina dentro da região boa, o Random continua borrifando. |
| [U3 · Aula 02 — o campeonato de recursos](https://colab.research.google.com/github/Eronponce/notebooks-aulas/blob/main/otimizacoes-em-machine-learning/u3_bloco_pratico_aula02_halving_vs_random.ipynb) | Funil 40 → 14 → 5: mesma qualidade, um terço do tempo. |
| [U4 · Aula 01 — CASH artesanal com Optuna](https://colab.research.google.com/github/Eronponce/notebooks-aulas/blob/main/otimizacoes-em-machine-learning/u4_bloco_pratico_aula01_cash_artesanal.ipynb) | A busca escolhe o algoritmo. O "simples demais" venceu os dois favoritos. |
| [U4 · Aula 02 — as 20 sementes](https://colab.research.google.com/github/Eronponce/notebooks-aulas/blob/main/otimizacoes-em-machine-learning/u4_bloco_pratico_aula02_20_sementes.ipynb) | Doze pontos de F1 de diferença sem mexer no modelo, só no sorteio dos dados. |

### Dependências

Tudo roda com o que o Colab já traz, com uma exceção: os notebooks da Unidade 2 usam `imbalanced-learn`. Se faltar, instale na primeira célula:

```python
!pip install -q imbalanced-learn optuna
```

O `optuna` é necessário nos notebooks das Unidades 3 e 4.

---

Os notebooks são gerados por script a partir do material-fonte da disciplina, então edições feitas aqui são sobrescritas na próxima geração. Para mudar o conteúdo, mude o material-fonte.

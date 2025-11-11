# Análise de Sentimentos — IMDb, Yelp e Amazon

Este projeto compara o desempenho de diferentes modelos de aprendizado de máquina na **classificação de sentimentos** (positivos e negativos) em três bases balanceadas: IMDb, Yelp e Amazon Reviews.

---

## 🧠 Modelos Utilizados
- **Regressão Logística (LR)**
- **XGBoost (XGB)**

As bases foram vetorizadas com **TF-IDF** e avaliadas com as métricas padrão de classificação.

---

## 📊 Métricas Principais

| Base  | Modelo | Acurácia | Precisão | Recall | F1 | AUC-ROC | AUC-PR |
|:------|:--------|:---------:|:---------:|:--------:|:--------:|:--------:|
| IMDb  | LR | 0.832 | 0.841 | 0.875 | 0.856 | 0.912 | 0.921 |
| IMDb  | XGB | 0.801 | 0.816 | 0.858 | 0.837 | 0.882 | 0.890 |
| Yelp  | LR | 0.816 | 0.821 | 0.888 | 0.814 | 0.897 | 0.907 |
| Yelp  | XGB | 0.782 | 0.801 | 0.852 | 0.825 | 0.837 | 0.850 |
| Amazon | LR | 0.841 | 0.850 | 0.880 | 0.861 | 0.910 | 0.918 |
| Amazon | XGB | 0.805 | 0.820 | 0.856 | 0.835 | 0.871 | 0.885 |

---

## 📈 Visualizações

Os gráficos de comparação (Curva ROC e Curva Precision-Recall) estão disponíveis na pasta `outputs/`.

---

## 🧩 Conclusões

- A **Regressão Logística** apresentou melhor equilíbrio entre precisão e recall em todas as bases.  
- O **XGBoost** teve bom desempenho, mas menor calibração probabilística.  
- Como as bases são **balanceadas**, o AUC-ROC foi a métrica mais representativa.  
- A LR é o modelo **mais consistente** e **mais interpretável** para este cenário.

---

## 📁 Estrutura do Projeto

analise-sentimentos/
├── data/
├── notebooks/
├── outputs/
└── README.md

✳️ *Projeto desenvolvido em Python com Scikit-learn, XGBoost e Matplotlib.*

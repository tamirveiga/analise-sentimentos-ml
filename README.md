# 💬 Análise de Sentimentos — IMDb, Yelp e Amazon

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-Data%20Science-orange?logo=scikitlearn)
![XGBoost](https://img.shields.io/badge/XGBoost-ML-green)

---

## 🧠 Descrição do Projeto

Este projeto compara o desempenho de diferentes **modelos de aprendizado de máquina** na **classificação de sentimentos** (positivos e negativos) em três bases de dados **balanceadas**:  
📚 *IMDb, Yelp* e *Amazon Reviews*.

As bases foram vetorizadas com **TF-IDF** e avaliadas com as métricas padrão de classificação.

---

## ⚙️ Modelos Utilizados

- **Regressão Logística (LR)**
- **XGBoost (XGB)**

Esses modelos foram escolhidos por apresentarem bom equilíbrio entre desempenho e interpretabilidade em tarefas de *NLP (Processamento de Linguagem Natural)*.

---

## 📊 Métricas Principais

| Base   | Modelo | Acurácia | Precisão | Recall | F1 | AUC-ROC | AUC-PR |
|:-------|:--------|:---------:|:---------:|:--------:|:--------:|:--------:|:--------:|
| **IMDb**  | LR  | **0.832** | **0.841** | 0.875 | **0.856** | **0.912** | **0.921** |
| IMDb  | XGB | 0.801 | 0.816 | 0.858 | 0.837 | 0.882 | 0.890 |
| **Yelp**  | LR  | **0.816** | **0.821** | 0.888 | **0.814** | **0.897** | **0.907** |
| Yelp  | XGB | 0.782 | 0.801 | 0.852 | 0.825 | 0.837 | 0.850 |
| **Amazon** | LR  | **0.841** | **0.850** | 0.880 | **0.861** | **0.910** | **0.918** |
| Amazon | XGB | 0.805 | 0.820 | 0.856 | 0.835 | 0.871 | 0.885 |

---

## 📈 Visualizações

Os gráficos de comparação (**Curva ROC** e **Curva Precision-Recall**) estão disponíveis na pasta [`outputs/`](outputs/).

Exemplo de gráficos gerados:
- Comparação entre modelos (ROC e PR)
- Distribuição de probabilidades
- Avaliação das métricas principais

---

## 🧩 Conclusões

- ✅ A **Regressão Logística (LR)** apresentou **melhor equilíbrio** entre precisão e recall em todas as bases.  
- ⚙️ O **XGBoost (XGB)** teve desempenho competitivo, porém com **probabilidades menos calibradas**.  
- ⚖️ Como as bases são **balanceadas**, o **AUC-ROC** é a métrica mais representativa.  
- 💡 A **LR** é o modelo **mais consistente e interpretável** neste cenário.  

---

## 🗂️ Estrutura do Projeto

```bash
analise-sentimentos/
│
├── data/
│   ├── imdb.csv
│   ├── amazon.csv
│   └── yelp.csv
│
├── notebooks/
│   ├── baseImdb.ipynb
│   ├── baseAmazon.ipynb
│   └── baseYelp.ipynb
│
├── outputs/
│   ├── imdb_curvas.png
│   ├── amazon_curvas.png
│   └── yelp_curvas.png
│
└── README.md
```

---

📘 **Tecnologias utilizadas:**  
Python · Scikit-learn · XGBoost · Matplotlib

✳️ *Projeto desenvolvido para comparação de modelos de classificação de sentimentos em bases balanceadas.*

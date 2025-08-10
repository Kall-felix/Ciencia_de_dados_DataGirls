## 📊 Previsão de rotatividade de funcionários (Variável alvo = Attrition)

Este projeto aplica **Machine Learning** para prever a probabilidade de um colaborador deixar a empresa, gerando **insights para o RH** e apoiando estratégias de retenção.

---

## 🎯 Objetivos do projeto
- Construir modelos preditivos para identificar colaboradores com alto risco de saída.
- Entender quais fatores tem mais influência na decisão de um funcionário na questão do desligamento.
- Fornecer recomendações práticas para reduzir a rotatividade.

---

## 🛠 Tecnologias utilizadas
- **Python 3.x**
- **Pandas / NumPy** – Manipulação e análise de dados
- **Matplotlib / Seaborn** – Visualização
- **Scikit-learn** – Modelagem estatística e Machine Learning
- **XGBoost** – Modelo gradient boosting
- **SHAP** – Interpretabilidade de modelos

---

## 📈 Modelos avaliados
Três algoritmos foram testados:

| Modelo                  | Acurácia | Recall (Saídas) | ROC AUC |
|-------------------------|----------|-------------------|---------|
| Logistic Regression     | 87,3%    | 51,4%              | 0.758   |
| Random Forest           | 84,8%    | 20,0%              | 0.766   |
| XGBoost                 | 84,3%    | 31,4%              | 0.696   |

> Saídas = Funcionários que saíram.

---

## 🔍 Principais insights (SHAP)
A análise de interpretabilidade indicou que os fatores mais relevantes para prever a saída foram:
- **StockOptionLevel** – Os funcionários que tem menos ações da empresa estão associados a maior risco de saída.
- **OverTime** – Excesso de horas extras aumenta a probabilidade de desligamento.
- **DistanceFromHome** – Longas distâncias de deslocamento também resultam no aumento do risco de saída.

---

## 💡 Aprendizados do projeto
- A **Logistic Regression** apresentou melhor equilíbrio entre acurácia e recall para a classe de saída.
- O **recall para a Saídas** (quem saiu) ainda é um desafio, sendo necessário alguns ajustes no balanceamento de classes.
- O uso do **SHAP** foi fundamental para traduzir resultados técnicos em insights claros para o RH, melhorando a visualização e compreensão dos resultados da análise.

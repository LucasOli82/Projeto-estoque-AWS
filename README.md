# 📊 Avaliação do Modelo de Previsão de Estoque

Este repositório contém um modelo de **Machine Learning** desenvolvido para prever a variável **`QUANTIDADE_ESTOQUE`** em Determinado dia do mês. A seguir estão descritas as principais **métricas utilizadas para avaliar o desempenho do modelo**, bem como a interpretação prática de cada uma.

---

## 🔧 Status do Modelo

* **Model Status:** Quick Build
* **Métrica de Otimização:** MSE (Mean Squared Error)

---

## 📈 Métricas de Avaliação

### 🔹 RMSE (Root Mean Squared Error)

**Valor:** `26.756`

O RMSE representa a **raiz quadrada do erro médio ao quadrado**, expressando o erro do modelo **na mesma unidade da variável prevista**.

#### 📌 Interpretação:

Em média, as previsões do modelo diferem do valor real de **QUANTIDADE_ESTOQUE em aproximadamente ±26,8 unidades**.

Exemplo:

* Estoque real: 100 unidades
* Previsão do modelo: cerca de 73 a 127 unidades

👉 Quanto **menor o RMSE**, maior a precisão do modelo.

---

### 🔹 MSE (Mean Squared Error)

**Valor:** `715.859`

O MSE calcula a **média dos erros ao quadrado** entre os valores previstos e os valores reais.

#### 📌 Características:

* Penaliza erros grandes com mais intensidade
* É amplamente utilizado como **métrica de otimização** durante o treinamento do modelo
* Serve principalmente para **comparar diferentes modelos**

Relação entre as métricas:

```
RMSE = √MSE
√715.859 ≈ 26.756
```

---

## 🎯 Métrica de Otimização

Durante o treinamento, o modelo foi ajustado para **minimizar o MSE (715.859)**. Isso significa que o algoritmo buscou reduzir ao máximo os erros maiores, priorizando previsões mais estáveis.

---

## 🧠 Avaliação Geral do Desempenho

A qualidade do modelo depende do **contexto do negócio**:

* Para estoques médios de **centenas ou milhares de unidades**, um erro médio de 27 unidades é considerado **baixo**.
* Para estoques médios **inferiores a 100 unidades**, esse erro pode ser **relevante**.

Portanto, o modelo apresenta uma **precisão moderada**, sendo adequado para cenários onde pequenas variações de estoque são aceitáveis.

---


## 📌 Conclusão

O modelo é capaz de prever a **QUANTIDADE_ESTOQUE** com um erro médio aceitável para muitos cenários práticos. As métricas apresentadas fornecem uma base sólida para avaliação, comparação e evolução do modelo.

---

📁 *Este README tem como objetivo documentar e facilitar o entendimento das métricas de avaliação do modelo para fins acadêmicos, profissionais ou de portfólio.*

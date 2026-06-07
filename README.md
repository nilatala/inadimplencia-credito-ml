# 📊 Classificação de Inadimplência de Clientes de Cartão de Crédito

## 📌 Sobre o Projeto

Este projeto tem como objetivo prever a inadimplência de clientes de cartão de crédito utilizando técnicas de análise de dados e machine learning.

A partir do dataset **Default of Credit Card Clients**, foram realizadas etapas de exploração, tratamento, preparação dos dados, modelagem e avaliação de desempenho, comparando diferentes algoritmos de classificação e analisando o impacto do ajuste do limiar de decisão nas métricas do modelo.

---

## 🎯 Objetivo

Desenvolver modelos capazes de identificar clientes com maior probabilidade de inadimplência, fornecendo suporte para decisões relacionadas à concessão de crédito, definição de limites e estratégias de mitigação de risco.

---

## 📂 Dataset

**Fonte:** Default of Credit Card Clients Dataset

**Quantidade de registros:** 30.000 clientes

### Variável alvo

- `default.payment.next.month`
  - `0` = Cliente adimplente
  - `1` = Cliente inadimplente

A base contém informações cadastrais, financeiras e comportamentais dos clientes, incluindo:

- Limite de crédito
- Histórico de pagamentos
- Valores de faturas
- Valores pagos
- Idade
- Escolaridade
- Estado civil

---

## 🛠️ Tecnologias Utilizadas

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![Google Colab](https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)

---

## 🔍 Etapas do Projeto

### 1. Análise Exploratória dos Dados (EDA)

Foram realizadas análises estatísticas e visuais para compreender:

- Distribuição da variável alvo
- Perfil dos clientes
- Distribuição dos limites de crédito
- Possíveis inconsistências nos dados

### Principais observações

- Taxa de inadimplência de aproximadamente 22%
- Base desbalanceada
- Valores inconsistentes em algumas variáveis categóricas
- Presença de valores negativos em faturas

---

### 2. Tratamento e Preparação dos Dados

Foram realizados:

- Correção de categorias inconsistentes
- Tratamento de valores negativos
- Separação entre variáveis preditoras e variável alvo
- Divisão em conjuntos de treino e teste
- Padronização dos dados para regressão logística

---

### 3. Modelagem

Foram desenvolvidos dois modelos de classificação:

#### Regressão Logística

Utilizada como modelo baseline devido à sua simplicidade e interpretabilidade.

#### Random Forest

Modelo baseado em árvores de decisão, capaz de capturar relações não lineares entre as variáveis.

---

### 4. Avaliação dos Modelos

Os modelos foram avaliados utilizando:

- Matriz de Confusão
- Precisão (Precision)
- Recall
- F1-Score
- Curva ROC
- AUC-ROC
- Curva Precision-Recall

---

### 5. Ajuste de Limiar de Decisão

Além da avaliação tradicional, foi realizada uma análise do impacto do limiar de decisão na Regressão Logística.

Foram testados diferentes thresholds para avaliar o trade-off entre:

- Precisão
- Recall
- F1-Score

Essa etapa demonstra como um modelo pode ser ajustado de acordo com os objetivos de negócio.

---

## 📈 Principais Resultados

- O Random Forest apresentou melhor desempenho geral na identificação de clientes inadimplentes.
- O histórico de pagamentos mostrou forte relação com a ocorrência de inadimplência.
- O ajuste do limiar de decisão permitiu adaptar o comportamento do modelo conforme a estratégia da instituição financeira.
- O equilíbrio entre precisão e recall foi observado em limiares próximos de 0,5–0,6.

---

## 💼 Aplicação de Negócio

Modelos de classificação de inadimplência podem auxiliar instituições financeiras em atividades como:

- Concessão de crédito
- Definição de limites
- Gestão de risco
- Monitoramento de carteiras
- Estratégias de cobrança preventiva

---

## 🚀 Próximos Passos

- Testar modelos como XGBoost e LightGBM
- Aplicar técnicas de balanceamento de classes (SMOTE)
- Realizar tuning de hiperparâmetros
- Implementar análise de importância das variáveis
- Construir dashboard para acompanhamento dos indicadores

---

## 📁 Estrutura do Projeto

```text
📦 Classificacao_Inadimplencia_Cartao_Credito
 ┣ 📜 README.md
 ┣ 📓 Classificacao_Inadimplencia.ipynb
 ┣ 📊 imagens/
 ┗ 📁 dados/
```

---

## 👩‍💻 Autora

**Elizabeth S. Thomaz**

📌 Projeto desenvolvido para fins de estudo e aprimoramento de habilidades em Análise de Dados, Machine Learning e Modelagem Preditiva.

🔗 LinkedIn: www.linkedin.com/in/elizabeth-thomaz-a91440157

🔗 GitHub: https://github.com/nilatala

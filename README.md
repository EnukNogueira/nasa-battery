# NASA Battery Dataset — Análise de Degradação de Baterias

Projeto em desenvolvimento.

---

## Sobre o projeto

Este projeto utiliza o dataset de baterias da NASA (Battery Data Set), que registra ciclos de carga e descarga de baterias de íon de lítio sob diferentes condições operacionais. O objetivo é explorar padrões de degradação, prever a capacidade da bateria ao longo dos ciclos de uso e comparar modelos de regressão para identificar a abordagem mais eficaz.

> **Status:** Em desenvolvimento. Limpeza dos dados, engenharia de atributos e a primeira rodada de modelagem preditiva já estão implementadas.

---

## Estrutura do repositório

```
nasa-battery/
├── battery_dataset/        # Arquivos de dados brutos da NASA
├── clean_date.ipynb        # Notebook de limpeza e tratamento inicial
├── modeling.ipynb          # Notebook de feature engineering e modelagem preditiva
└── README.md
```

---

## O que já foi feito

- **Limpeza e tratamento dos dados**: filtragem dos registros de descarga, conversão de tipos e remoção de valores nulos.
- **Engenharia de atributos**: criação da coluna `ciclo`, numerando sequencialmente as descargas de cada bateria para representar sua "idade" ao longo do uso.
- **Visualização da curva de degradação**: plotagem da capacidade da bateria ao longo dos ciclos de descarga.
- **Modelagem preditiva**: comparação de três modelos de regressão do scikit-learn para prever a capacidade da bateria a partir do ciclo e da temperatura ambiente:
  - Random Forest Regressor
  - Linear Regression
  - Decision Tree Regressor
- **Avaliação de modelos**: métricas de erro (RMSE, MAE e R²) calculadas para cada modelo, permitindo comparar desempenho.

---

## Tecnologias utilizadas

- **Python 3**
- **Pandas** — manipulação e limpeza de dados
- **NumPy** — operações numéricas
- **Matplotlib** — visualização de dados
- **Scikit-learn** — modelagem preditiva (Random Forest, Linear Regression, Decision Tree) e métricas de avaliação
- **Jupyter Notebook** — ambiente de desenvolvimento

---

## Próximos passos

- [ ] Ajuste de hiperparâmetros dos modelos para melhorar o desempenho
- [ ] Identificação do ponto de fim de vida útil (capacidade < 70% do valor nominal)
- [ ] Documentação comparativa final dos três modelos com conclusões sobre qual se ajusta melhor ao problema

---

## Fonte dos dados

Dataset público disponibilizado pela NASA:
[NASA Battery Dataset — Prognostics Center of Excellence](https://www.nasa.gov/intelligent-systems-division/discovery-and-systems-health/pcoe/pcoe-data-set-repository/)

---

## Autor

**Enuk Nogueira** — Estudante de Análise e Desenvolvimento de Sistemas, com foco em Análise de Dados

[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/enuknogueira/)
[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/EnukNogueira)

# NASA Battery Dataset — Análise de Degradação de Baterias

Projeto de análise de dados e Machine Learning utilizando o NASA Battery Dataset para estudar a degradação da capacidade de baterias de íon-lítio ao longo dos ciclos de uso.

O projeto está sendo desenvolvido em etapas, passando pelo tratamento dos dados, análise exploratória, engenharia de atributos, modelagem preditiva, validação dos modelos e, posteriormente, criação de uma aplicação interativa em Dash.

---

## Sobre o projeto

O dataset registra ciclos de carga e descarga de baterias de íon-lítio submetidas a diferentes condições de operação.

O objetivo principal é analisar como a capacidade das baterias se comporta ao longo dos ciclos e avaliar modelos de Machine Learning capazes de prever essa capacidade.

Além da análise da degradação, o projeto busca comparar diferentes abordagens de regressão e entender quais modelos apresentam melhor desempenho para esse problema.

---

## Estrutura do repositório

- `battery_dataset/` — dados utilizados no projeto
- `sklearn_battery.ipynb` — tratamento, análise e modelagem
- `README.md` — documentação do projeto

---

## Etapas do projeto

### 1. Tratamento dos dados

- [x] Carregamento dos dados
- [x] Organização dos arquivos do dataset
- [x] Tratamento dos registros de descarga
- [x] Conversão dos tipos de dados
- [x] Tratamento de valores ausentes
- [x] Organização das informações por bateria e ciclo

### 2. Engenharia de atributos

- [x] Criação da variável `ciclo`
- [x] Identificação da bateria
- [x] Preparação das variáveis utilizadas nos modelos
- [x] Definição da capacidade como variável alvo

### 3. Análise exploratória

- [x] Análise da capacidade das baterias ao longo dos ciclos
- [x] Visualização das curvas de degradação
- [x] Análise da relação entre ciclo e capacidade
- [x] Análise da temperatura ambiente
- [ ] Aprofundamento da análise das características das baterias

### 4. Machine Learning

Foram utilizados inicialmente três modelos de regressão:

- [x] Linear Regression
- [x] Decision Tree Regressor
- [x] Random Forest Regressor
- [ ] XGBoost Regressor

Os modelos são utilizados para prever a capacidade da bateria com base nas variáveis disponíveis no conjunto de dados.

### 5. Validação dos modelos

- [x] Separação dos dados para treinamento e avaliação
- [x] GroupKFold Cross-Validation
- [x] Avaliação utilizando RMSE
- [x] Avaliação utilizando MAE
- [x] Avaliação utilizando R²
- [x] Comparação inicial dos modelos
- [x] Ajuste de hiperparâmetros
- [ ] Comparação final incluindo XGBoost

O uso de `GroupKFold` foi adotado para evitar que dados da mesma bateria sejam distribuídos de maneira inadequada entre treinamento e validação.

---

## Resultados iniciais

Os primeiros testes foram realizados utilizando Linear Regression, Decision Tree Regressor e Random Forest Regressor.

Os resultados iniciais mostraram desempenho semelhante entre Random Forest e Decision Tree, enquanto a Regressão Linear apresentou um comportamento diferente na previsão da capacidade.

Os resultados serão revisados após a inclusão do XGBoost e da comparação final entre os modelos.

---

## Análise de degradação

Uma das próximas etapas é aprofundar a análise da degradação individual das baterias.

A análise deverá comparar as baterias para identificar:

- maior degradação;
- menor degradação;
- comportamento da capacidade ao longo dos ciclos;
- diferenças entre as baterias;
- possível relação entre condições de operação e degradação.

Também será analisado o ponto de fim de vida útil das baterias, considerando o limite de capacidade definido para o estudo.

- [ ] Identificar o ponto de fim de vida útil
- [ ] Calcular a degradação individual das baterias
- [ ] Comparar maior e menor degradação
- [ ] Analisar diferenças entre baterias
- [ ] Documentar os principais resultados

---

## Dashboard

Após a conclusão da etapa de Machine Learning, o projeto será transformado em uma aplicação interativa utilizando Dash e Plotly.

O dashboard deverá permitir explorar os principais resultados da análise, incluindo:

- capacidade ao longo dos ciclos;
- curvas de degradação;
- comparação entre baterias;
- indicadores de degradação;
- resultados dos modelos;
- métricas de avaliação;
- previsões de capacidade.

### Etapas

- [ ] Estudar Dash
- [ ] Estudar Plotly
- [ ] Estruturar a aplicação
- [ ] Criar visualizações interativas
- [ ] Integrar os resultados do Machine Learning
- [ ] Finalizar o dashboard
- [ ] Documentar a aplicação

---

## Tecnologias utilizadas

- **Python 3**
- **Pandas** — manipulação e tratamento dos dados
- **NumPy** — operações numéricas
- **Matplotlib** — visualização exploratória
- **Scikit-learn** — Machine Learning e avaliação dos modelos
- **Jupyter Notebook** — desenvolvimento e documentação
- **XGBoost** — próximo modelo a ser testado
- **Dash** — aplicação interativa
- **Plotly** — visualizações interativas

---

## Próximas etapas

A sequência planejada para conclusão do projeto é:

Análise dos resultados atuais  
↓  
XGBoost  
↓  
Comparação dos modelos  
↓  
Avaliação final  
↓  
Análise aprofundada da degradação  
↓  
Identificação do fim de vida útil  
↓  
Documentação dos resultados  
↓  
Estudo de Dash e Plotly  
↓  
Dashboard interativo  
↓  
Documentação final

---

## Fonte dos dados

Dataset público disponibilizado pelo NASA Prognostics Center of Excellence:

[NASA Battery Dataset — Prognostics Center of Excellence](https://www.nasa.gov/intelligent-systems-division/discovery-and-systems-health/pcoe/pcoe-data-set-repository/)

---

## Autor

**Enuk Nogueira**

Estudante de Análise e Desenvolvimento de Sistemas pela PUCPR, com foco em Análise de Dados e Ciência de Dados.

[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/enuknogueira/)

[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/EnukNogueira)

# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Este é um projeto de previsão de estoque inteligente na AWS com SageMaker Canvas. Neste projeto usarei o SageMaker Canvas para criar previsões de estoque baseadas em Machine Learning (ML).

## 🎯 Objetivos Deste Desafio de Projeto (Lab)

![image](https://github.com/digitalinnovationone/lab-aws-sagemaker-canvas-estoque/assets/730492/72f5c21f-5562-491e-aa42-2885a3184650)

## 🚀 Passo a Passo

### 1. Selecionar Dataset

-   Selecionei um dos datasets presentes neste repositório, no caso foi o "dataset-1000-com-preco-promocional-e-renovacao-estoque", que contém id do produto,
data do evento, preço, flag promocional e a quantidade do estoque.
-   Após escolher o dataset, fiz o upload no SageMaker Canvas para iniciar o treinamento do Machine Learning (ML).

### 2. Construir/Treinar

-   Ao importar o dataset, configurei a coluna de preços como alvo de previsão.
-   Em seguida configurei as outras variáveis de entrada e escolhi o modelo de previsão.
-   Escolhi o Standard build que é o método mais demorado de treino para previsões mais precisas.

### 3. Analisar

-   Após o treinamento, examine as métricas de performance do modelo.
-   Verifique as principais características que influenciam as previsões.
-   Faça ajustes no modelo se necessário e re-treine até obter um desempenho satisfatório.

### 4. Prever

-   Use o modelo treinado para fazer previsões de estoque.
-   Exporte os resultados e analise as previsões geradas.
-   Documente suas conclusões e qualquer insight obtido a partir das previsões.

## 🤔 Dúvidas?

Esperamos que esta experiência tenha sido enriquecedora e que você tenha aprendido mais sobre Machine Learning aplicado a problemas reais. Se tiver alguma dúvida, não hesite em abrir uma issue neste repositório ou entrar em contato com a equipe da DIO.

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

![image](https://github.com/user-attachments/assets/03f0584e-cf27-4a3f-b930-9a8a9dee4376)

-   Ao importar o dataset, configurei a coluna de preços como alvo de previsão.
-   Em seguida configurei as outras variáveis de entrada e escolhi o modelo de previsão.
-   Escolhi o Standard build que é o método mais demorado de treino para previsões mais precisas.

### 3. Analisar

![image](https://github.com/user-attachments/assets/e1d673f9-bf03-4220-9c7b-fe5ddeae8aa7)

-   Avg. wQL calcula a diferença entre os valores previstos e os valores reais.
-   MAPE calcula a porcentagem de erros de todos os pontos de tempo.
-   WAPE semelhante ao MAPE, mas os erros são ponderados de acordo com a importância ou frequência de cada informação.
-   RMSE é a raiz quadrada da média dos quadrados das diferenças entre os valores previstos e os valores reais. O RMSE é sensível a grandes erros, o que pode ser útil se erros grandes forem particularmente indesejáveis no seu contexto.
-   MASE compara o erro absoluto médio do seu modelo com o erro absoluto médio de um modelo de benchmark simples (como a média histórica ou a previsão de um passo anterior).
-   Todas essas métricas significam que quanto mais perto de zero, mais precisa é a previsão.
-   Abaixo verificamos as principais caracteristicas que influenciaram a previsão. A FLAG_PROMOCAO e a principal sendo a QUANTIDADE_ESTOQUE.

### 4. Prever

![image](https://github.com/user-attachments/assets/45c790d2-cd76-4928-bdea-26257eebad3a)

-   Escolhi o item 1021 para criar previsões e criar um gráfico.
-   Em azul está os resultados passados, em rosa está o pior caso previsto, em verde está uma previsão neutra e em amarelo o melhor caso previsto.
-   Um exemplo de insight neste caso é que podemos ter certeza que no dia 2024-02-10 o valor será o mesmo idependente da pior ou melhor previsão.

### 5. Conclusão

Este projeto mostra um método fácil e rápido de ensinar um Machine Learning (ML) com um método no-code e criar previsões e insights de maneiras diferentes baseado no dataset apresentado.

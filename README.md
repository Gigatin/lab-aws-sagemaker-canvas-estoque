# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Bem-vindo ao desafio de projeto "Previsão de Estoque Inteligente na AWS com SageMaker Canvas. Neste Lab DIO, você aprenderá a usar o SageMaker Canvas para criar previsões de estoque baseadas em Machine Learning (ML). 


## 🎯 Objetivos Deste Desafio de Projeto (Lab)

![image](https://github.com/digitalinnovationone/lab-aws-sagemaker-canvas-estoque/assets/730492/72f5c21f-5562-491e-aa42-2885a3184650)




# Previsão de Estoque Inteligente na AWS

Este repositório contém o desafio de projeto "Previsão de Estoque Inteligente na AWS com SageMaker Canvas", oferecido pela DIO.

## 🚀 Passo a Passo (Desafio de Projeto)

### 1. Seleção do Dataset
O dataset utilizado para o treinamento do modelo de Machine Learning está disponível no repositório da DIO, na pasta `datasets`.

### 2. Construção e Treinamento
- Configuramos o **QUANTIDADE_ESTOQUE** como target e o **ID_PRODUTO** como ITEM ID.
- O modelo foi treinado utilizando o modo Quick Build.

### 3. Análise
- Ajustamos o modelo para melhorar as métricas de desempenho. Os melhores resultados obtidos com o modo Quick Build foram:
  - **Avg. wQL**: 0.344
  - **MAPE**: 0.936
  - **WAPE**: 0.569
  - **RMSE**: 34.950
  - **MASE**: 0.832
- Apesar de ainda estarem altos, optei por continuar com esses resultados.
- Os principais fatores de impacto identificados foram o preço e os feriados, com aproximadamente 51% e 12% de influência, respectivamente.

### 4. Previsão
- Utilizando o modelo treinado, obtivemos as previsões finais.
- Observações sobre os resultados:
  - **Item III** e **Item IV** apresentaram um estoque elevado, sugerindo que não é necessário comprar mais desses itens no momento.
  - **Item V** mostrou uma baixa no estoque, indicando a necessidade de compra adicional.
- As previsões são refletidas pelas linhas:
  - **P10 (Linha Rosa)**: Cenário negativo.
  - **P50 (Linha Verde)**: Cenário neutro.
  - **P90 (Linha Amarela)**: Cenário positivo.
![image](https://github.com/user-attachments/assets/32a1f97a-1ea2-4f76-97b6-ab012b1fe2b0)

![image](https://github.com/user-attachments/assets/f38d6a75-19ad-4788-a69e-ec0d0fe179a8)



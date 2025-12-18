# Trabalho Final – Machine Learning 1  
**Aluno:** Marcello Borges Miranda  
**Curso:** Machine Learning 1 – Adatech  

## Descrição do Projeto

Este projeto utiliza dados do *World Happiness Report* para aplicar técnicas de
Machine Learning com o objetivo de analisar fatores associados ao nível de felicidade
dos países.

O dataset contém informações como PIB per capita, suporte social, expectativa de vida,
liberdade, generosidade e percepção de corrupção, coletadas entre os anos de 2015 e 2022.

## Estratégia adotada

Como o índice de felicidade é originalmente uma variável contínua, o problema foi
transformado em uma tarefa de classificação binária. Para isso, foi criada a variável
`Score_binary`, baseada na mediana do índice de felicidade (`Score`).

Além disso, dados de diferentes anos para um mesmo país foram tratados como registros
independentes (País-Ano), permitindo a construção de um dataframe final com mais de
1000 instâncias.

## Etapas do Projeto

- Importação das bibliotecas
- Carregamento e padronização dos dados
- Análise exploratória
- Criação do target binário
- Pré-processamento com Pipeline
- Treinamento de modelos de classificação
- Avaliação e comparação de desempenho
- Análise de explicabilidade (extra)

## Modelos Utilizados

- Regressão Logística
- K-Nearest Neighbors (KNN)
- Random Forest

## Avaliação

Os modelos foram avaliados utilizando:
- Matriz de Confusão
- Relatório de Classificação
- Curva ROC e métrica AUC

O modelo Random Forest apresentou o melhor desempenho geral.

## Dataset

Fonte:  
https://www.kaggle.com/datasets/unsdsn/world-happiness

## Estrutura do Repositório

- `notebook.ipynb` – Notebook principal do projeto
- `data/` – Arquivos CSV do dataset
- `README.md`
- `requirements.txt`


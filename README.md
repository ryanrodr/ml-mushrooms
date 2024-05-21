## **Classificação de cogumelos com Machine Learning 🍄**

O conjunto de dados foi escolhido no Kaggle e contém diversas espécies de cogumelos e suas respectivas características como diâmetro da tampa, forma da tampa, altura do caule, cor do caule e entre outras informações descritivas que evidenciam se é comestivel (0) ou venenoso (1). 

O desafio consiste em implementar um modelo de classificação binária que possa reconhecer os padrões do conjunto de dados e consiga generalizar para novos dados, classificando se é comestivel ou venenoso.

Link do Dataset: [Mushroom Dataset (Binary Classification)](https://www.kaggle.com/datasets/prishasawhney/mushroom-dataset/data)

### Introdução e primeiros passos do projeto:

Esse conjunto de dados já passou por um processo de limpeza e preparação dos dados, e isso me permitiu focar na implementação e validação dos modelos com Scikit-Learn. Dentre os processos necessários para execução dos algoritmos eu precisei:

- Separar os dados entre **X** sendo as **Features** e **Y** sendo a variável **Target**.
- Realizei a normalização dos dados com **StandardScaler**.
- Separei os dados em Treino e Teste com **train_test_split**.

### Definindo um modelo:

#### **DecisionTreeClassifier**
Modelo supervisionado de aprendizado de máquina baseado em Árvores de Decisão. É utilizado para Classificação de observações, onde cada característica do dado resulta em um possível resultado e isso vai se estendendo recursivamente até chegar em todas as decisões possíveis.
- Validando o modelo com uma Matriz de Confusão:
  
![DTC](https://github.com/ryanrodr/ml-mushrooms/blob/main/imagens/MatrizConfusaoDTC.png)


#### **KNeighborsClassifier**
Modelo supervisionado de aprendizado de máquina que utiliza medidas de similaridade em um conjunto de dados para reconhecimento de padrões. Ele realiza a Classificação das observações identificando os k-vizinhos mais próximos.
- Validando o modelo com uma Matriz de Confusão:

![KNN](https://github.com/ryanrodr/ml-mushrooms/blob/main/imagens/MatrizConfusaoKNN.png)

### Conclusão
Os resultados da Matriz de Confusão identificam que o melhor modelo é o **KNeighborsClassifier** por ter uma taxa de Falsos Negativos menor que o **DecisionTreeClassifier**. Uma das métricas do projeto é focar na classificação dos cogumelos venenosos minimizando a quantidade de erros.
- KNN classificou 86 cogumelos como comestiveis que na verdade eram venenosos
- Acurácia do modelo KNeighborsClassifier - 98.68%
- DTC classificou 194 cogumelos como comestiveis que na verdade eram venenosos
- Acurácia do modelo DecisionTreeClassifier - 97.32%

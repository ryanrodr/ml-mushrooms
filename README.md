### **Classificação de cogumelos com Machine Learning 🍄**

O conjunto de dados foi escolhido no Kaggle e contém diversas espécies de cogumelos e suas respectivas características como diâmetro da tampa, forma da tampa, altura do caule, cor do caule e entre outras informações descritivas que evidenciam se é comestivel (0) ou venenoso (1).

Link do Dataset: [Mushroom Dataset (Binary Classification)](https://www.kaggle.com/datasets/prishasawhney/mushroom-dataset/data)

O desafio consiste em implementar um modelo de classificação binária que possa reconhecer os padrões do conjunto de dados e consiga generalizar para novos dados, classificando se é comestivel ou venenoso. Separei os dados em 70% para treinamento e 30% teste e escolhi dois modelos, sendo o **KNeighborsClassifier** e o **DecisionTreeClassifier.** Utilizei métricas para validação como matriz de confusão e acurácia do pacote `sklearn.metrics`.

**DecisionTreeClassifier** é um modelo supervisionado de aprendizado de máquina baseado em Árvores de Decisão. É utilizado para Classificação de observações, onde cada característica do dado resulta em um possível resultado e isso vai se estendendo recursivamente até chegar em todas as decisões possíveis. O modelo em questão chegou em uma acurácia dos dados de teste em **97.37%**.

**KNeighborsClassifier** é um modelo supervisionado de aprendizado de máquina que utiliza medidas de similaridade em um conjunto de dados para reconhecimento de padrões. Ele realiza a Classificação das observações identificando os k-vizinhos mais próximos. KNN chegou em uma acurácia de **98.68%**.
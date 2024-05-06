### **Classificação de cogumelos com Machine Learning 🍄**

O conjunto de dados foi escolhido no Kaggle e já passou por um processo de limpeza e preparação dos dados, o que facilitou na implementação dos algoritmos. O dataset em questão contém diversas espécies de cogumelos e suas respectivas características como diâmetro da tampa, forma da tampa, altura do caule, cor do caule e entre outras características descritivas, também temos a classe alvo que determina se a espécie é comestivel (0) ou se é venenosa (1).

Link do Dataset: [Mushroom Dataset (Binary Classification)](https://www.kaggle.com/datasets/prishasawhney/mushroom-dataset/data)

O desafio consiste em implementar um modelo de classificação binária que possa reconhecer os padrões do conjunto de dados e consiga generalizar para novos dados se determinada espécie é comestivel ou venenosa. Separei os dados em 70% para treinamento e 30% para teste e escolhi dois modelos para classificação, sendo o **KNeighborsClassifier** e o **DecisionTreeClassifier.** Utilizei métricas para validação como matriz de confusão e acurácia do pacote `sklearn.metrics`.

**DecisionTreeClassifier** é um modelo supervisionado de aprendizado de máquina baseado em Árvores de Decisão. É utilizado para Classificação de observações, onde cada característica do dado resulta em um possível resultado e isso vai se estendendo recursivamente até chegar em todas as decisões possíveis. O modelo em questão chegou em uma acurácia dos dados de teste em **97.37%**.

**KNeighborsClassifier** é um modelo supervisionado de aprendizado de máquina que utiliza medidas de similaridade em um conjunto de dados para reconhecimento de padrões. Ele realiza a Classificação das observações identificando os k-vizinhos mais próximos. KNN chegou em uma acurácia de **98.68%**.
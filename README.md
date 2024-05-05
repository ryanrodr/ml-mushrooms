# ml-mushrooms
#### **Classificação de cogumelos venenosos com ML**

**Modelo - KNeighborsClassifier da Scikit-Learn**

Dataset - [Mushroom Dataset (Binary Classification)](https://www.kaggle.com/datasets/prishasawhney/mushroom-dataset/data)

O desafio do projeto seria desenvolver um modelo de machine learning para classificação binária de um conjunto de dados sobre cogumelos e suas características, que possa prever se é comestível (0) ou venenoso (1) para novos dados. O dataset utilizado já foi pré-processado com diversas técnicas de limpeza e preparação, o que facilitou na implementação do algoritmo.

Utilizei o modelo KNeighborsClassifier com a métrica de distância Euclidiana para identificar os K-vizinhos mais próximos. O modelo atingiu uma acurácia de 98,68% para os dados de teste.
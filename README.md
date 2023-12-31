# Artificial-Neural-Networks-From-Scratch

Artificial Neural Networks (ANNs) are computational models inspired by the human brain's neural structure. They consist of interconnected layers of artificial neurons that process input data and learn from it to make predictions. ANNs are widely used for various tasks, such as classification, regression, and pattern recognition, thanks to their ability to learn complex relationships in data through a process called training, which involves adjusting the connections (weights) between neurons.

[ArtificialNeuralNetworksBank-Note](ArtificialNeuralNetworksBank-Note.ipynb) is trained on [Bank-Note Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/00267/data_banknote_authentication.txt) It has three layers of neurons: input layer containing 4 neurons corresponding to features, hidden layer containing 4 neurons, and finally output layer containing two neurons corresponding to target classes( encoded as: 0 and 1). During training, all the weights and biases are updated after processing single training sample and the method is called stochastic training. The update rule uses learning rate of 0.1 and momentum factor of 0.001. The code is run for 20 epochs (i.e. each training example is called 20 times). The activation function is softmax of the form f(x1, x2, x3, x4) = [exp(x1)/(exp(x1)+exp(x2)+exp(x3)+exp(x4)) , exp(x2)/(exp(x1)+exp(x2)+exp(x3)+exp(x4)), exp(x3)/(exp(x1)+exp(x2)+exp(x3)+exp(x4)), exp(x4)/(exp(x1)+exp(x2)+exp(x3)+exp(x4))]. Since softmax already normalizes features, there is no need for explicit normalization.

The dataset is divided into 5 folds and scores are measured taking each fold as dataset. There is also a plot of epoch vs. Loss mean during training.

Results for Fold 1, Fold 2, Fold 3, Fold 4 and Fold 5, respectively are:                                                                                               

![alt text](Bank-NoteFold1.png)   

![alt text](Bank-NoteFold2.png)

![alt text](Bank-NoteFold3.png)

![alt text](Bank-NoteFold4.png)

![alt text](Bank-NoteFold5.png)

Scores:

![alt text](Bank-NoteScores.png)

[ArtificialNeuralNetworksIris.ipynb](ArtificialNeuralNetworksIris.ipynb) is trained on Iris Dataset from sklearn. It has three layers of neurons: input layer containing 4 neurons corresponding to features (sepal length, sepal width, petal length, petal width), hidden layer containing 5 neurons, and finally output layer containing three neurons corresponding to target classes( encoded as: Setosa-0, Versicolor-1, and Virginica-2). During training, all the weights and biases are updated after processing single training sample and the method is called stochastic training. The update rule uses learning rate of 0.1 and momentum factor of 0.001. The code is run for 150 epochs. The activation function is sigmoid of the form f(x) = 1 / 1 + exp(-x). Its range is between 0 and 1.

The dataset is divided into 5 folds and scores are measured taking each fold as dataset. Dataset was normalized and encoded beforehand. The result are as follows:

![alt text](IrisDataset1.png)

![alt text](IrisDataset2.png)

![alt text](IrisDataset3.png)

![alt text](IrisDataset4.png)

![alt text](IrisDataset5.png)

![alt text](IrisDatasetScores.png)


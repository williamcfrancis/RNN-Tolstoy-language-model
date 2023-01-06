# RNN langauge model
Pytorch implementation of a recurrent neural network for predicting the next character in a given sentence. 

## Dataset
The training dataset used here is the book War and Peace by Leo Tolstoy.
The text file of the book can be downloaded from [HERE](https://raw.githubusercontent.com/mmcky/nyu-econ-370/master/notebooks/data/book-war-and-peace.txt)

## Methodology
Each character is converted into its one-hot encoding. An RNN is then trained with one hidden layer which predicts the one-hot vector of the next characteras output, given the past sequence. This corresponds to the operations.
![image](https://user-images.githubusercontent.com/38180831/205384906-37d1f1df-38c4-4a3e-b8f2-e98096c68fde.png)

Here I predict softmax output logits yˆt ∈ R over the entire vocabulary. The loss is simply the cross-entropy loss of predicting the correct next character.

## Results
![image](https://user-images.githubusercontent.com/38180831/205385524-ad45909e-9e1a-4dff-bc0c-185d9695b158.png)
![image](https://user-images.githubusercontent.com/38180831/205385566-6e3d711d-47a4-4e93-9472-f04e35274eac.png)

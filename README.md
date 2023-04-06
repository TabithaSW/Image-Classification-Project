MODEL ACCURACY AND EVALUATION INFORMATION 


ResNet_Model.ipynb contains the second model, it is a ResNet50 model with sparse cross entropy for the loss function, adam algorithm for the optimization, and random transformations to each individual image as it is passed to the model. (Tabitha's Model)

Accuracy for ResNet train and test: 94% Test, 97% Train,

- Train Result Accuracy, Loss and Accuracy: [0.26725998520851135, 0.9760624170303345]
- Test Accuracy, Loss and Accuracy: [0.5889386534690857, 0.9484072923660278]

tensorflow_classification.ipynb contains the first model, it is a custom tf.keras.Sequential model with ReLU and Max Pooling Layers. (Koya's Model)

Accuracy for custom train and test: 95% Test, 99% Train

- Train Result Accuracy, Loss and Accuracy: [0.010305597446858883, 0.9938234686851501]
- Test Accuracy, Loss and Accuracy: [0.16977623105049133, 0.9524737596511841]

tensorflow_InceptionV3.ipynb contains the last model, it is a similar to ResNet except Inception focuses on computational cost, ResNet focuses on computational accuracy. We used Adam algorithm for optimization and sparse cross entropy again for loss. (Nick's Model)

Accuracy for Inception train and test: 95% Test, 98% Train

- Train Result Accuracy, Loss and Accuracy: [0.0291230920702219, 0.9872484803199768]
- Test Accuracy, Loss and Accuracy: [0.12433519214391708, 0.9503558278083801]

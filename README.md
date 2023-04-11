MODEL ACCURACY AND EVALUATION INFORMATION 

-------------------------------------------------------------------------------

ResNet_Model.ipynb contains the second model, it is a ResNet50 model with sparse cross entropy for the loss function, adam algorithm for the optimization, and random transformations to each individual image as it is passed to the model. (Tabitha's Model)

Accuracy was measured using Tensorflow Keras Accuracy Metric, described as:

- Calculates how often predictions equal labels. This metric creates two local variables, total and count that are used to compute the frequency with which y_pred matches y_true. This frequency is ultimately returned as binary accuracy: an idempotent operation that simply divides total by count.

Accuracy for ResNet train and test: 94% Test, 97% Train,

- Train Result Accuracy, Loss and Accuracy: [0.26725998520851135, 0.9760624170303345]
- Test Accuracy, Loss and Accuracy: [0.5889386534690857, 0.9484072923660278]

--------------------------------------------------------------------------------

tensorflow_classification.ipynb contains the first model, it is a custom tf.keras.Sequential model with ReLU and Max Pooling Layers. (Koya's Model)

Accuracy for custom train and test: 95% Test, 99% Train

Accuracy was measured using Tensorflow Keras Accuracy Metric, described as:

- Calculates how often predictions equal labels. This metric creates two local variables, total and count that are used to compute the frequency with which y_pred matches y_true. This frequency is ultimately returned as binary accuracy: an idempotent operation that simply divides total by count.

- Train Result Accuracy, Loss and Accuracy: [0.010305597446858883, 0.9938234686851501]
- Test Accuracy, Loss and Accuracy: [0.16977623105049133, 0.9524737596511841]

--------------------------------------------------------------------------------

tensorflow_InceptionV3.ipynb contains the third model, it is a similar to ResNet except Inception focuses on computational cost, ResNet focuses on computational accuracy. We used Adam algorithm for optimization and sparse cross entropy again for loss. (Nick's Model)

Accuracy for Inception train and test: 95% Test, 98% Train

Accuracy was measured using Tensorflow Keras Accuracy Metric, described as:

- Calculates how often predictions equal labels. This metric creates two local variables, total and count that are used to compute the frequency with which y_pred matches y_true. This frequency is ultimately returned as binary accuracy: an idempotent operation that simply divides total by count.

- Train Result Accuracy, Loss and Accuracy: [0.0291230920702219, 0.9872484803199768]
- Test Accuracy, Loss and Accuracy: [0.12433519214391708, 0.9503558278083801]

---------------------------------------------------------------------------------

CLIP_Model.ipynb contains the last model. CLIP consists of seperate encoder models for image and text data. The CLIPTokenizerFast is used to encode the text prompts. The CLIPProcessor uses a pretrained model for encode both text prompts and true images.

There is no additional training required for this model.

The accuracy was measured using the probabilities returned from the model. The plot of accuracy vs test runs is drawn.

---------------------------------------------------------------------------------
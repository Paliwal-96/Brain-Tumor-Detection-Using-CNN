# Published Research Paper :   

https://ieeexplore.ieee.org/document/10486347


## ABSTRACT

Diagnosing a brain tumor takes a long time and relies heavily on the radiologist’s abilities and experience. The amount of data that must be handled has increased dramatically as the number of patients has increased, making old procedures both costly and ineffective. Recently, digital medical images have been essential for detecting numerous illnesses. It is additionally used for training and research. The 
need for electronic medical images is growing dramatically. The old method of manually evaluating medical imaging is time-consuming, inaccurate, and prone to human error. Over the medical diseases, the brain tumor has become a serious issue, ranking 4th among the major causes of death in India. Many researchers investigated a variety of algorithms for detecting and classifying brain tumors that were both accurate and fast. Deep Learning (DL) approaches have recently been popular in developing automated systems capable of accurately diagnosing or segmenting brain tumors in less time. DL enables a pre-trained Convolutional 
Neural Network (CNN) model for medical images, specifically for classifying brain cancers. The proposed Brain Tumor Classification Model based on CNN (BCM-CNN) is a CNN hyperparameters optimization. There are primarily two types of hyperparameters: (i) hyperparameters that determine the underlying network structure; (ii) a hyperparameter that is responsible for training the network. 

## The Proposed architecture for the whole model is below:

![1](https://github.com/Paliwal-96/Brain-Tumor-Detection-Using-CNN/assets/100425990/090f0b1f-b342-4e40-96ab-7b2f0ab5a9f5)



### Our proposed block diagram for automated binary and multiclass brain tumor detection is shown in the above diagram. The architecture starts with image extraction and loading labels from the dataset. The extracted images then need to be preprocessed before splitting them into training, validation, and test set. Finally, our proposed CNN architecture is applied to the dataset being processed.

#### About the Architecture Employed:

Each input x (image) has a shape of (240, 240, 3) and is given as input into the neural network. And, it is processed through the following layers:

1.	A Zero Padding layer having a pool size of (2, 2).
2.	A convolutional layer having 32 filters, with a filter size of (7, 7) and a stride equal to 1.
3.	A batch normalization layer to normalize pixel values to enhance computation.
4.	A ReLU activation layer.
5.	A Max Pooling layer having f=4 and s=4.
6.	A Max Pooling layer having f=4 and s=4, same as earlier.
7.	A flattening layer to flatten the 3-dimensional matrix into a one-dimensional vector.
8.	A Dense (output unit) fully connected layer having one neuron having a sigmoid activation (because, it being a binary classification job).
   
#### Reason behind the use of this architecture !

Initially, we attempted transfer learning using ResNet50 and VGG-16 models. However, due to the complexity of these models relative to our dataset size, overfitting became a significant issue. While data augmentation could potentially mitigate this problem, our computational resources were constrained by a 10th generation Intel i5 CPU and 8 GB RAM. Therefore, we opted to explore simpler architectures and train them from scratch. Surprisingly, this approach proved successful, demonstrating the effectiveness of matching model complexity to available computational resources.


## Conclusion:

The main objective of the current study was to develop deep learning network namely a CNN model to classify MRI images into two classes of brain tumors one as malignant tumor and other one class of healthy brain with no tumor. The applied image dataset was publicly available at Kaggle and was contrast-enhanced magnetic resonance imaging (MRI) images.


The proposed CNN model reached the accuracy of following on different samples of datasets, which is as follows:

Accuracy of the best model on the testing data:

Test Loss = 0.39058661460876465

Test Accuracy = 0.9032257795333862

The results of this study demonstrate that our proposed network have an immeasurable generalization and high execution speed; therefore, they can be applied as effective decision-support agents for radiologists in medical diagnostics.

#### Thank You !!! :)

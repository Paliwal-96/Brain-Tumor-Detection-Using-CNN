# Published Research Paper :   

https://ieeexplore.ieee.org/document/10486347


## ABSTRACT

Diagnosing a brain tumor takes a long time and relies heavily on the radiologist’s abilities and experience. The amount of data that must be handled has increased dramatically as the number of patients has increased, making old procedures both costly and ineffective. Recently, digital medical images have been essential for detecting numerous illnesses. It is additionally used for training and research. The 
need for electronic medical images is growing dramatically. The old method of manually evaluating medical imaging is time-consuming, inaccurate, and prone to human error. Over the medical diseases, the brain tumor has become a serious issue, ranking 4th among the major causes of death in India. Many researchers investigated a variety of algorithms for detecting and classifying brain tumors that were both accurate and fast. Deep Learning (DL) approaches have recently been popular in developing automated systems capable of accurately diagnosing or segmenting brain tumors in less time. DL enables a pre-trained Convolutional 
Neural Network (CNN) model for medical images, specifically for classifying brain cancers. The proposed Brain Tumor Classification Model based on CNN (BCM-CNN) is a CNN hyperparameters optimization. There are primarily two types of hyperparameters: (i) hyperparameters that determine the underlying network structure; (ii) a hyperparameter that is responsible for training the network. 

## The Proposed architecture for the whole model is below:

![1](https://github.com/Paliwal-96/Brain-Tumor-Detection-Using-CNN/assets/100425990/090f0b1f-b342-4e40-96ab-7b2f0ab5a9f5)



### Our proposed block diagram for automated binary and multiclass brain tumor detection is shown in the above diagram. The architecture starts with image extraction and loading labels from the dataset. The extracted images then need to be preprocessed before splitting them into training, validation, and test set. Finally, our proposed CNN  architectures are applied to the employed datasets.

#### Understanding the architecture:

Each input x (image) has a shape of (240, 240, 3) and is fed into the neural network. And, it goes through the following layers:

1.	A Zero Padding layer with a pool size of (2, 2).
2.	A convolutional layer with 32 filters, with a filter size of (7, 7) and a stride equal to 1.
3.	A batch normalization layer to normalize pixel values to speed up computation.
4.	A ReLU activation layer.
5.	A Max Pooling layer with f=4 and s=4.
6.	A Max Pooling layer with f=4 and s=4, same as before.
7.	A flatten layer in order to flatten the 3-dimensional matrix into a one-dimensional vector.
8.	A Dense (output unit) fully connected layer with one neuron with a sigmoid activation (since this is a binary classification task).
   
#### Why this architecture?

Firstly, We applied transfer learning using a ResNet50 and vgg-16, but these models were too complex to the data size and were overfitting. Of course, you may get good results applying transfer learning with these models using data augmentation. But, We are using training on a computer with 10th generation Intel i7 CPU and 16 GB memory. So, We had to take into consideration computational complexity and memory limitations.
So why not try a simpler architecture and train it from scratch. And it worked :)

## Conclusion:

The main objective of the current study was to develop deep learning network namely a CNN model to classify MRI images into two classes of brain tumors one as malignant tumor and other one class of healthy brain with no tumor. The applied image dataset was publicly available at Kaggle and was contrast-enhanced magnetic resonance imaging (MRI) images.


The proposed CNN model reached the accuracy of following on different samples of datasets, which is as follows:

Accuracy of the best model on the testing data:

Test Loss = 0.39058661460876465

Test Accuracy = 0.9032257795333862

The results of this study demonstrate that our proposed network have an immeasurable generalization and high execution speed; therefore, they can be applied as effective decision-support agents for radiologists in medical diagnostics.


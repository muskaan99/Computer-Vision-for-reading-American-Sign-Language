# Computer Vision For American Sign Language
## Dataset
Download the dataset from [here](https://www.kaggle.com/datasets/grassknoted/asl-alphabet) 

Download the real-world test dataset created by us from [here](https://www.kaggle.com/datasets/muskaan3299/self-generated-test-set)

Refer [Installation_instructions.md] file for more details on installation process (https://github.com/muskaan99/Computer-Vision-for-reading-American-Sign-Language/blob/main/Installation_instructions.md)

## Abstract
Despite the widespread use of sign language in recent years, it remains difficult for non-sign language speakers to
communicate with sign language speakers. In recent years, advances in Computer Vision and Deep Learning have
demonstrated promising progress in the fields of motion and gesture recognition. This would help enable communication
with the hearing-impaired. We propose to create a model to read the American Sign Language using a dataset
containing images from 29 classes. The training dataset contains 26 handshapes corresponding to the 26 letters of
the alphabet and 3 other shapes to demonstrate Space, Delete and Nothing. We perform a comparison between
multiple models with different architectures and model parameters to be able to determine the model that performs
best on both, the provided dataset as well as on real world data.

## Challenges
• Generating Test Data: Since the test dataset for the problem is very small, we had to generate our own test
data to determine each model’s performance and accuracy on real world data. The images have to be taken with
varying backgrounds to enable diversity. Other pre-processing techniques such as cropping are also required to
be able to eliminate unwanted details in the image. Since there are many output classes, it is time consuming
to manually capture multiple images for each class.

• Size of the Training Dataset: Since the training data consists of 69,600 200x200 RGB images, it takes a
significant amount of time for the model to learn from each image for around 40 epochs. Using a CPU alone
would cause the execution times to be much longer, hence, GPUs are required for the task.

## Conclusion

We see that MobileNet-V2 performs best on both the test datasets. It misclassifies one image from the provided test data and is able to manage an impressive accuracy of 51% on the real world test data. None of the other models are able to achieve more than 30% on the self generated data. This could be because there was no similar training data provided to the models due to which they are unable to accurately decipher the hand gestures. Our CNN model is also able to provide a reasonably good accuracy on the self generated test data as compared to the other models. The Resnet pretrained model is unsuccessful in interpreting the same data, but it compares with CNN in predicting the original test data.We see that our Neural Network is able to comprehend the original test data very well (almost similar to CNN
accuracy), but it performs poorly on the real world data, since it can only decipher 3 of the given 87 images. Since neural networks always find the easiest way to solve a problem, we need to include maximum diversity in our dataset and maximize the coverage (by training on extremely difficult examples) to be able to achieve appreciable accuracies on real world data.
![image](https://user-images.githubusercontent.com/68809236/168027244-840b779c-6fbd-4bd4-9629-e405df4a6f65.png)


## Future Work
• Generate better and larger variety of images for both training and test data

• Build further on the model by providing live transcription of captured video feed. This transcription can then
be used to produce speech.


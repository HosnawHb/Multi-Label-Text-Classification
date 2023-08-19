# Multi Label Text Classification
👋 Welcome to my GitHub project! </br >

## Data
- In this project I worked with PerSICK dataset which contains three thousand rows and three columns. Each line contains two sentences, sentence1 and sentence2, and the degree of similarity between these two sentences is determined by score. </br>
 For more detailed information about this dataset, you can check out [PerSICK dataset](https://github.com/Ledengary/COPER/blob/main/Datasets/PerSICK.csv). </br>

## Purpose
- The purpose of this project was to deal with Data Labeling, Multi-label Recurrent Neural Classification, Text Processing and Classification Networks.
## Description
In this project, I will be working with a dataset containing pairs of sentences. Each pair consists of sentence1 and sentence2, and the degree of similarity between them is measured by a score.</br >
The goal of this project is to perform textual similarity detection, where the neural network determines the degree of similarity between two sentences. To tackle this task, two general approaches can be used: </br >

1️⃣ Regression method: This approach involves predicting a precise numerical value using a neural network.  </br >

2️⃣ Classification method: This approach involves dividing similarity into categories (1 to 5) and predicting the category using a neural network.  </br >

For this project, we will adopt the classification method. The scores indicating the similarity between sentence pairs will be rounded to convert the numerical similarity into categorical similarity. </br>
Upon closer examination of the dataset, it's observed that the sentence pairs predominantly revolve around specific topics such as children, cats/dogs, men/women, and other general subjects. </br>
Therefore, in addition to predicting the similarity category, our goal is to classify the pairs based on their subject. The subject categories that our model will classify them into are as follows: </br >
- Man/Boy
- Woman/Girl
- Child/Children
- Animals
- Other
- N/A (for cases where the subject of the two sentences is not the same or indistinguishable)

The PerSICK dataset doesn't provide columns based on the subject of the sentences. Hence, it's our responsibility to extract this information. We can leverage the Dependency parsing technique from well-known Persian language processing libraries like Parsivar and Hazm to accomplish this task.
<div align="center"><img src="https://github.com/HosnawHb/Multi-Label-Text-Classification/blob/main/Model.png?raw=true"width="60%"/></div> </br >

To summarize, this project involves accomplishing two tasks simultaneously: </br>
classifying the degree of similarity and determining the subject of a pair of input sentences. To achieve this, we will employ multi-label classification.</br>
The neural network will take two separate inputs for each sentence and predict 11 labels. Five of the labels correspond to the similarity degree categories (1 to 5), while the remaining six labels represent different subject categories (animals, children, other, etc.). The neural network will learn to predict one label from the similarity degree categories and another label from the active subject categories.</br> </br>

## Team Members
[Hosna Habibi](https://github.com/HosnawHb) </br>
[Pooya Kavosh](https://github.com/Jarvis017) </br>

Please refer to the code in the repository for a step-by-step guide on implementing the neural network, training the model, and evaluating its performance.









# HLAT Dataset
This is the HLAT Dataset proposed in paper Exploring Human-like Attention Supervision in Visual Question Answering.
which has been accepted by AAAI-2018. [paper](https://arxiv.org/abs/1709.06308)

In this work, we propose a Human Attention Network (HAN) to predict the attention map for a given image-question pair.

Here we provide the .h5 file of attention maps for both the VQA1.0 and the VQA2.0 dataset.
Using the attention maps to improve the performance of VQA is quite easy. 
We did it through adding the attention supervision to the attention-based model.
For more details, please refer to our paper: 


The .h5 file of attention maps can be found here:


The .h5 file format has the following data structure: 
{
"pre_attmap" : attention maps for all question id 
}
Which means that in each .h5 file, there is only one dict, whose key is named as "pre_attmap". The order of the attention maps is as same as the order of the question ids in the file. Therefore it is easy to get the attention maps for the question-image pairs if you know the order of the question id in the .json file provided by the VQA official web set. http://visualqa.org/download.html

For VQA1.0 dataset, there are:
369,861 attention maps for questions in the trainval set 
244,302 attention maps for questions in the testing set
 60,864 attention maps for questions in the test-dev set

For VQA2.0 dataset, there are:
658,111 attention maps for questions in the trainval set 
447,793 attention maps for questions in the testing set
107,394 attention maps for questions in the test-dev set





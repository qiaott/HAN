HLAT Dataset

In our work, we propose a Human Attention Network (HAN) to predict the attention map for a given image-question pair.
Here we provide the .h5 file of attention maps for both the VQA1.0 and the VQA2.0 dataset.
Using the attention maps to improve the performence of VQA is quite easy. We did it through adding the attention supervison to the attention-based model.
For more details, please refer to our paper: 

You can download .h5 file of attention maps from here:


The .h5 file format has the following data structure: 
{
"pre_attmap" : attention maps for all questionid 
}
Which means that in each .h5 file, there is only one dict, whose key is named as "pre_attmap".


For VQA1.0 dataset, we provide:
369,861 attention maps for questions in the trainval set 
244,302 attention maps for questions in the testing set
 60,864 attention maps for questions in the test-dev set

For VQA2.0 dataset, we provide:
658,111 attention maps for questions in the trainval set 
447,793 attention maps for questions in the testing set
107,394	attention maps for questions in the test-dev set


The order of the attention maps is as same as the order of the question ids in the file.
Therefore it is easy to get the attention maps for the question-image pairs if you know the order of the question id in the .json file(e.g.,MultipleChoice_mscoco_train2014_questions.json) provided by the VQA official webset.


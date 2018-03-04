# Exploring Human-like Attention Supervision in Visual Question Answering
Here we provide HLAT Dataset proposed in paper [Exploring Human-like Attention Supervision in Visual Question Answering](https://arxiv.org/abs/1709.06308), which has been accepted by AAAI-2018. 

In this work, we propose a Human Attention Network (HAN) to predict the attention map for a given image-question pair.
![The framework of HAN](https://github.com/qiaott/HAN/blob/master/images/han_framework.jpg)

There are some examples that generated by the HAN.
![Examples of HAN](https://github.com/qiaott/HAN/blob/master/images/han_examples.jpg)

We improve the performance of attention-based VQA models by adding human-like attention supervision.
![The structure of attention supervision](https://github.com/qiaott/HAN/blob/master/images/supervised_model.jpg)

Our method shows good performance in improving the accuracy of VQA, especially in counting problem, *e.g.How many candles are on the table?* For more details, please refer to our paper.

## HLAT Dataset

Here we provide the .h5 file of attention maps for both the VQA1.0 and the VQA2.0 dataset.
Using our attention maps to improve the performance of VQA is quite easy. 
We did it through adding the attention supervision to the attention-based model.

#### The *.h5 file* of attention maps can be found [here]()

The *.h5 file* format has the following data structure: 
{
*__"pre_attmap" : attention maps for all question id__*
}
Which means that in each *.h5 file*, there is only one dict, whose key is named as *__"pre_attmap"__*. The order of the attention maps is as same as the order of the question ids in the file. Therefore we use the order of question ids to get the attention maps for the question-image pairs. the order of question id follows the VQA 1.0 and VQA 2.0 official datasets[website](http://visualqa.org/download.html).


### For VQA1.0 dataset, there are:
* 369,861 attention maps for questions in the trainval set 
* 244,302 attention maps for questions in the testing set
* 60,864 attention maps for questions in the test-dev set

### For VQA2.0 dataset, there are:
+ 658,111 attention maps for questions in the trainval set 
+ 447,793 attention maps for questions in the testing set
+ 107,394 attention maps for questions in the test-dev set

## VQA-HAT Dataset
Here we also provide the link of the VQA-HAT Dataset, which is from paper [Human Attention in Visual Question Answering:
Do Humans and Deep Networks Look at the Same Regions?](https://arxiv.org/abs/1606.03556).

## Cite
We would be very appreciate if you cite our work.

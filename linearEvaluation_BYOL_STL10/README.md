Link to Paper
https://arxiv.org/abs/2006.07733

Link to data
https://cs.stanford.edu/~acoates/stl10/

## 실행 환경
 V100 GPU 
## experiment info
 - linear classifiers trained on the (frozen) representations learned by BYOL
 - 위 방법은 일반적으로 linear classification protocol이라 불리고 BYOL paper의 pg.6의 Linear evaluation 방식
batch size -> 
optimizer -> Adam
## result
 accuracy(top-1) 7
 ![image](https://user-images.githubusercontent.com/46518769/138544200-075bc35f-fee4-42b5-a2e1-a4505e77be2e.png)

 customized code of https://github.com/Spijkervet/BYOL for STL10 

cf)
Evaluate our model
A popular way to evaluate a SSL method in computer vision or for that fact any other pre-training method as such is to learn a linear classifier on the frozen features of the trained backbone model and evaluate the classifier on unseen images. Other methods often include fine-tuning on the source dataset or even a target dataset with 5% or 10% labels present. You can use the backbone we just trained for any downstream task such as image classification (like we do here) or segmentation or detection, where the backbone models are usually pre-trained with supervised learning.
(출처. https://colab.research.google.com/github/keras-team/keras-io/blob/master/examples/vision/ipynb/nnclr.ipynb#scrollTo=8KUnJ7loOY_t) 

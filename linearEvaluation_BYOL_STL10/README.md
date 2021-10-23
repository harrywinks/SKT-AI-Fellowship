Link to Paper
https://arxiv.org/abs/2006.07733

Link to data
https://cs.stanford.edu/~acoates/stl10/

## 실행 환경
 V100 GPU 
## experiment info
 - linear classifiers trained on the (frozen) representations learned by BYOL
 - 위 방법은 일반적으로 linear classification protocol이라 불리고 BYOL paper의 pg.6의 Linear evaluation 방식
## result
 accuracy 
 ![image](https://user-images.githubusercontent.com/46518769/138544200-075bc35f-fee4-42b5-a2e1-a4505e77be2e.png)

 customized code of https://github.com/Spijkervet/BYOL for STL10 

![birdtag](https://github.com/madivanhorn/Few_Shot_FGVC/blob/main/assets/Kentucky_Warbler_ex.jpg)


# Few-Shot Fine-Grained Visual Classification using Coarse-Grained Supervision

Fine-grained visual classification tasks are both difficult to solve, due to the subtle class distinctions inherent to the problem, and highly desirable to be automated due to the high cost of employing skilled human experts capable of performing the classification. Current best practices for training a high performing classification model for difficult vision problems necessitates the collection of large training datasets. For fine-grained domains, this subsequently requires the involvement of highly skilled human experts, a prohibitively expensive cost for some applications. In this work, we explore few-shot fine-grained visual classification using strong supervision from coarse-grained models. We assume that generic detection, segmentation, and keypoint localization models are at our  disposal, as none of these models require expert curated training data. We then use the outputs of these models to simplify the fine-grained visual classification problem by removing nuisance variables such as object location, occlusion, and pose. Using an off-the-shelf pretrained ResNet50 feature extractor, our experiments on the CUB200 dataset show that we can increase top-1 accuracy using 1 training image for each class from 0.18 to 0.27. Using 5 training images our method improves top-1 accuracy from 0.42 to 0.54. We also run experiments that compare ImageNet pretrained features to iNaturalist pretrained features. Using an iNaturalist pretrained model and our strong preprocessing methods, we see an improvement to 0.56 top-1 accuracy using 1 image for each class, a 3x improvement over the simple ImageNet feature baseline.

## Obtaining Pretrained ResNet50
Please refer to ["Benchmarking Representation Learning for Natural World Collections."](https://github.com/visipedia/newt/blob/main/benchmark/README.md) 

## Dataset
Download CUB200-2011 [here](http://www.vision.caltech.edu/visipedia/CUB-200-2011.html)

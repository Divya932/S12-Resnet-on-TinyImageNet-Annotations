# S12-Resnet-on-TinyImageNet-Annotations
Repo describing Application of Resnet18 on TinyImagenet Dataset and Annotations on a 50 dog dataset


## Assignment A:

**Train ResNet18 on TINY IMAGENET dataset. (70/30 split) for 50 Epochs. Target 50%+ Validation Accuracy.**
Train and val data are shuffled and divided into 70:30 ratio giving 77,000 train and 33,000 test images.  

**Transforms Applied:**  
1. HorizontalFlip(0.7)  
2. PadIfNeeded(70,70)  
3. RandomCrop(64,64)  
4. Rotate(30)  
5. Normalize  
6. Cutout(0.7)  

**Scheduler**  
One Cycle LR  

**Results**  
Model reaches 57.69% Test Accuracy in 30 epochs.  

## Assignment B:
Downloaded 50 images of dogs. 
Use this (Links to an external site.) to annotate bounding boxes around the dogs.
Download JSON file. 
Describe the contents of this JSON file in FULL details (you don't need to describe all 10 instances, anyone would work). 
Refer to this tutorial (Links to an external site.). Find out the best total numbers of clusters. Upload link to your Colab File uploaded to GitHub. 

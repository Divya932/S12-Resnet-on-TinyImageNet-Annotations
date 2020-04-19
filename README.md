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
Downloaded 50 images of dogs. Find images [here](https://github.com/Divya932/S12-Resnet-on-TinyImageNet-Annotations/tree/master/Ass%20S12_B/Dogs_data)   
The dogs in these images are then annotated using VGG Tool Annotator.   
The contents of its JSON file are described [here](https://github.com/Divya932/S12-Resnet-on-TinyImageNet-Annotations/blob/master/JSON%20Description)  

The Kmeans clusters formed are here:
![Clusters](https://github.com/Divya932/S12-Resnet-on-TinyImageNet-Annotations/blob/master/Ass%20S12_B/Clusters.png)  

The best total numbers of clusters found using Kmeans and elbow method are 3, for these bounding boxes.  
![Elbow](https://github.com/Divya932/S12-Resnet-on-TinyImageNet-Annotations/blob/master/Ass%20S12_B/elbow.png)

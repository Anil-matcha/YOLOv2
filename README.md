# YOLOv2

# Used code from https://github.com/experiencor/keras-yolo2 to train yolov2

# Things to be done to make it work

  Always start with pre-trained weights from imagenet (Tried training from scratch but always results in exploding gradients probably due   to less data size i.e 5000 images compared to huge imagenet data size)
  
  Generator anchors for the dataset, otherwise will lead to slow convergence
  
  Warmup batches need to be present to stabilize the training(not sure of the reason), used 3 in this case
  
  Freeze all the layers of the feature extractor and train only on output layers, otherwise gradient will again explode and give nan

  

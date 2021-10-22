#  Sensor Fusion and Tracking - Object Detection

## Section 1 : Compute Lidar Point-Cloud from Range Image
### Visualize range image channels (ID_S1_EX1)

![](img/range_image.png)

### Visualize lidar point-cloud (ID_S1_EX2)

![](img/pcl_image.png)

## Section 2 : Create Birds-Eye View from Lidar PCL
### Convert sensor coordinates to BEV-map coordinates (ID_S2_EX1)

![](img/bev_image.png)

### Compute intensity layer of the BEV map (ID_S2_EX2)

![](img/intensity_image.png)

### Compute height layer of the BEV map (ID_S2_EX3)

![](img/height_image.png)

## Section 3 : Model-based Object Detection in BEV Image

![](img/fpn_resnet_result.png)

## Section 4 : Performance Evaluation for Object Detection
### DarkNet
Precision = 0.9292604501607717, Recall = 0.9444444444444444

![](img/performance_evaluation_darknet.png)

### FPN-ResNet
Precision = 1.0, Recall = 0.8562091503267973

![](img/performance_evaluation_fpn_resnet.png)

## Answer Questions
### Find and display 10 examples of vehicles with varying degrees of visibility
- 3 vehicles driving in opposite direction with high visibility

![](img/pcl1.png)

- 3 vehicles driving in opposite direction with low visibility

![](img/pcl2.png)

- 3 vehicles driving in same direction with high visibility (1 car with trailer in front of the ego vehicle and 2 cars behind the ego vehicle) 

![](img/pcl3.png)

- 4 vehicles on the right side with high visibility

![](img/pcl4.png)

- 4 vehicles on the left side with very low visibility

![](img/pcl5.png)

### Identify stable vehicle features in the point-cloud
Bumpers (both front and rear) and windshields are clearly visible in most cases. This could be because of their large reflective surface and their materials.

![](img/feature1.png)

![](img/feature2.png)

![](img/feature3.png)
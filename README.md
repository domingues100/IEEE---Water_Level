# Deep Learning and object detection for water level measurement using patterned visual markers

All the code was developed in Python:

1. Class.ipynb: This file contains the classification code. It needs to be run first, as it will generate the k-fold files used in the other scripts.
2. Regress.ipynb: This file contains the regression code. Remember to use the same folders with the k-fold data obtained from the previous step.
3. OD_RCNN.ipynb: This is the object detection code for Faster R-CNN. Run this first and use the same split data in the subsequent object detection code.
4. OD_RETINANET.ipynb: This is the object detection code for RetinaNet. Ensure you use the same test/train .csv file in this code.
5. SN1.ipynb: This is the code for the first Siamese Network. It is shorter because it uses the same k-fold folders, and the network is a classification model adapted as a Siamese Network. The training step is the same as in Class.ipynb, so you can use the same weights and folders in the testing step presented in this file.
6. SN2.ipynb: This is the code for the second Siamese Network. It is necessary to train this model five times, saving the weights and the test/train.csv each time. During the testing step, you'll need to run it five different times and save the results. More information is provided in the file.

## Dataset

The images originally used are located inside the "pool dataset" folder this repo: https://github.com/domingues100/Water-Level-Detection-Datasets, along with the original .json file. Additionally, the file converted to CSV is in this repository under the name "instances_default.csv."



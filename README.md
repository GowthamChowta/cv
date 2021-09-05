# Object Segmentation

Object Segmentation or Image segmentation is termed as categorizing each pixel value of an image to a particular class.

Data contains 4000+ images of Indian roads and the corresponding class x-y co-ordinates of each image. <br> Link to the dataset :<a href="https://drive.google.com/file/d/1iQ93IWVdR6dZ6W7RahbLq166u-6ADelJ/view?usp=sharing">Data</a>


The notebook object segmentation.ipynb has UNet and CANet (Chaing context and Aggregation network)

1) UNET -  Architechture:
![image](https://user-images.githubusercontent.com/58596028/132141468-df95e72b-f38c-4a89-a472-8ba94e921e00.png) Ref: https://arxiv.org/pdf/1505.04597.pdf

In the notebook I am applying transfer learning on UNet model with image net weights as it takes lot of memory and computation power to train from scratch. <br>
For improving the speed, we can freeze the encoder weights and train only the decoder part.

2) CANet (Attention-guided Chained Context Aggregation for Semantic Segmentation) - Architechture: 
![image](https://user-images.githubusercontent.com/58596028/132141553-68a609a8-7080-48b4-badf-90e2d0a53931.png)
(Exact version is not implemented, minor changes were made to the architechture )
Input and output: <br>
![image](https://user-images.githubusercontent.com/58596028/132141399-304399d4-ae38-4512-b573-28f1d7ce8f78.png)



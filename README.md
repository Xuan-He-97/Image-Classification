# Image-Classification

In this project, we collect image data of four buildings/objects in Shanghai and Guangzhou. Each class contains 100~150 photos of building/objects taken from different angles and distances. This notebook trains a model to recognize these classes. The notebook is initially run on the [google colab](https://colab.research.google.com). The data is stored and downloaded on the [google drive](https://drive.google.com/file/d/1rj-RaymLVMJoZOrkxa2wt0h2-EoPrDVL/view?usp=sharing). You can download the data by simply requesting access to it.

Main steps in this notebook:

I. Upload data

II. Preprocess data

(a) split train and validation data
(b) preprocess and generate image data batch
III. Recognize objects by training on a small dataset

IV. Use data augmentation to gain higher accuracy

V. Export the model and run it in the browser

## Result

Applying simple CNN model to the data gives us validation accuracy of 93%.
Data augmentation increases the prediction accuracy from 93% to 99.3%.
For each class, we pick one picture and show the results of prediction.

![alt text](https://user-images.githubusercontent.com/79208856/113706860-ba411e00-9711-11eb-9e44-8b8e9f29fc4f.png)

![alt text](https://user-images.githubusercontent.com/79208856/113706875-bd3c0e80-9711-11eb-9ea0-953b07876123.png)

Training and validation of accuracy and loss are given in the picture below, which shows the result of the first 150 epoches of training process. 

![alt text](https://user-images.githubusercontent.com/79208856/113706292-18213600-9711-11eb-9eca-7788b2662948.png)

After the 60th epoch, the training and validation curve both becomes stable. Thus we pick the model trained at 59th epoch to make predictions. 
The model is also uploaded on the [gituhub page](https://xuan-he-97.github.io/index.html) where you can upload an image and make prediction by yourself. You can download data from [shared google drive file](https://drive.google.com/file/d/1rj-RaymLVMJoZOrkxa2wt0h2-EoPrDVL/view?usp=sharing).

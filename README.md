# Image-Classification

In this project, we collect image data of four buildings/objects in Shanghai and Guangzhou. Each class contains 100~150 photos of building/objects taken from different angles and distances. This notebook trains a model to recognize these classes. The notebook is initially run on the google colab. The data is stored and downloaded on the google drive. You can download the data by simply requesting access to it.

Main steps in this notebook:

I. Upload data

II. Preprocess data

(a) split train and validation data
(b) preprocess and generate image data batch
III. Recognize objects by training on a small dataset

IV. Use data augmentation to gain higher accuracy

V. Export the model and run it in the browser

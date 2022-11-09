
# Explainable AI Assignment 1: Projection Space Exploration

## Feature Visualization

In machine learning (ML), we constantly seek to gain insights into the data, such as familiarizing ourselves with the training samples or improving our comprehension of the label distribution. We use a variety of data visualization techniques to do that.

Usually, we have to examine a number of data properties at once. For instance, the data in traditional ML may have thousands of labels. We must first comprehend the data's structure and the significance of these qualities in order to choose the best model.

Compared to standard ML, the dimensionality increases in deep learning. On the one hand, there aren't usually many labels in the datasets we work with. For instance, in classification, there is only ever one class label that corresponds to a picture. Neural Nets, on the other hand, handle data in a complicated manner using their millions of parameters and several layers. We might need to view the inner feature maps or parameter values to understand what's happening inside the network, which would require working with multidimensional data once more.

We can only understand 1-, 2-, or 3-dimensional plots since we are 3D creatures. A collection of techniques known as Dimensionality Reduction methods can be used to view multidimensional data in smaller dimensions.

## General Information Submission

**Group Members**

| Student ID    | First Name  | Last Name      | E-Mail                    |  Workload [%] |
| --------------|-------------|----------------|----------------------     |---------------|
| 11942036      | Abdul Basit | Banbhan        |abdul.banbhan@jku.at       |25%           |
| 12126769      | Hala        | Al-Jarajrah    |k12126769@students.jku.at  |25%           |
| 51903451      | Mohamed     | ELharty        |m.elharty@outlook.com      |25%           |
| 12130348      | Nader       | Essam          |k12130348@students.jku.at  |25%           |

### Dataset

The dataset used is an image dataset used for microscopy image classification. The dataset is acquired from a previous course, AI in Life Sciences. The dataset consists of 9632 training images with 9 classes. However, only 7890 images are used for training and the rest is used for testing. 
The goal is to analyze the learning process of the model and to visualize the features. The Deep Learning (DL) training algorithms and its influence on the explainability of neural network models are investigated. The overall aim is to visualize flow of information within the deep NN using factors that can be interpreted by humans, even if the underlying model uses more complex factors, which enables generation of human interpretable explanations.

  ![00001_combined](https://user-images.githubusercontent.com/27974341/200887456-c65751ab-76b9-4031-9e1b-43c210fd2708.png) 
  ![00002_combined](https://user-images.githubusercontent.com/27974341/200887547-638ba8af-aab1-4783-bb43-66abbf9e2b81.png)
  ![00015_combined](https://user-images.githubusercontent.com/27974341/200888625-2f97207e-3b16-44a6-8408-b885b9d02f1c.png)
  ![00016_combined](https://user-images.githubusercontent.com/27974341/200888630-b7d1746d-e7ca-4a23-b900-a32f36e5e8c9.png)
  ![00003_combined](https://user-images.githubusercontent.com/27974341/200887689-2b480e00-0690-46c9-a049-4332644cb487.png) 
  ![00005_combined](https://user-images.githubusercontent.com/27974341/200887828-ec44919f-2dcb-4342-9a44-6f8d9cfecd02.png)  ![00006_combined](https://user-images.githubusercontent.com/27974341/200887957-6ed20200-811a-4e3a-aa87-9f8a9c5dce12.png) ![00008_combined](https://user-images.githubusercontent.com/27974341/200888030-bef7281d-8c80-4b97-a7a6-acaf8a7a122a.png) ![00017_combined](https://user-images.githubusercontent.com/27974341/200888975-f4f0bdbb-9268-423c-8994-91f346c868ce.png)
![00018_combined](https://user-images.githubusercontent.com/27974341/200888979-e50f336b-968a-44d5-81c4-941373dbb2d4.png)
![00019_combined](https://user-images.githubusercontent.com/27974341/200888986-7b402524-bb59-4819-acb7-aa79a3394927.png)
![00020_combined](https://user-images.githubusercontent.com/27974341/200888990-fd09f49d-a532-4296-8a5a-e26ccae41935.png) 

![00023_combined](https://user-images.githubusercontent.com/27974341/200888999-89e33d47-53dc-456e-9959-6212cc42de12.png) ![00024_combined](https://user-images.githubusercontent.com/27974341/200889003-f946fbea-a522-47f7-a0b1-3f4668183dc3.png) ![00025_combined](https://user-images.githubusercontent.com/27974341/200889006-ccea8e04-9c9e-4788-90ce-1f7b2ffe2499.png) ![00009_combined](https://user-images.githubusercontent.com/27974341/200888067-8111517b-d1eb-45bc-82ed-6bef884df12a.png) ![00010_combined](https://user-images.githubusercontent.com/27974341/200888338-99de5b2d-fd5b-49cf-9c96-b03707fcb904.png) ![00011_combined](https://user-images.githubusercontent.com/27974341/200888344-3cae1beb-9db6-4ffd-b8e7-5965e7af6651.png) ![00012_combined](https://user-images.githubusercontent.com/27974341/200888479-6534f006-7414-4ed5-8a1f-7f880cd92913.png) ![00013_combined](https://user-images.githubusercontent.com/27974341/200888486-c2409a09-01b2-4999-a3e1-b947cc23572f.png) ![00014_combined](https://user-images.githubusercontent.com/27974341/200888490-959dd30f-8202-4f3d-84bc-77068f6dd1a0.png) 
![00026_combined](https://user-images.githubusercontent.com/27974341/200889618-b05f08e5-28d0-4ace-bf57-b143b3dbc79c.png) ![00027_combined](https://user-images.githubusercontent.com/27974341/200889623-b17a6e26-ea6a-4071-8529-07e1a0d36def.png) ![00028_combined](https://user-images.githubusercontent.com/27974341/200889624-6db74dfe-3c4e-4a14-9c9b-3c12b2686858.png) 
In this data, we visualize the learning process of the model. The inter-epoch trajectory of the model learning is the main focus. Initially, the network has random weights and learns features from data. As the epochs proceed, the model learns and is able to use the learned features and use the updated weights to better the classification results. The model hidden layer features are visualized and should be seen with better and more obvious formation of clusters. 

To download the dataset use the following command:

```
wget https://apps.ml.jku.at/challenge/data/datasets/cell_id/images_test.tar
wget https://apps.ml.jku.at/challenge/data/datasets/cell_id/images_train.tar
wget https://apps.ml.jku.at/challenge/data/datasets/cell_id/y_train.csv
```


## Results
TODO: 
- What can be seen in the projection(s)?
- Was it what you expected? If not what did you expect?
- Can you confirm prior hypotheses from the projection?
- Did you get any unexpected insights?

### Animation of PCA over 10 epochs
https://user-images.githubusercontent.com/27974341/200884531-98989a0b-725f-4ca0-9386-16bd78396d98.mp4

### Animation of t-SNE with matric euclidean over 10 epochs
https://user-images.githubusercontent.com/27974341/200884943-15c042b2-37df-49ce-8a0b-e08d7202a164.mp4


### Animation of UMAP with matric euclidean over 10 epochs
https://user-images.githubusercontent.com/27974341/200885153-d6e06296-4ca5-4b81-8f1c-9284b271a2dd.mp4


## Final Submission

* Make sure that you pushed your GitHub repository and not just committed it locally.
* Sending us an email with the code is not necessary.
* Update the *environment.yml* file if you need additional libraries, otherwise the code is not executeable.
* Create a single, clearly named notebook with your solution, e.g. solution.ipynb.
* Save your final executed notebook as html (File > Download as > HTML) and add them to your repository.


## Development Environment

Checkout this repo and change into the folder:
```
git clone https://github.com/jku-icg-classroom/xai_proj_space_2022-<GROUP_NAME>.git
cd xai_proj_space_2022-the-ai-explainers
```

Load the conda environment from the shared `environment.yml` file:
```
conda env create -f environment.yml
conda activate xai_proj_space
```

> Hint: For more information on Anaconda and enviroments take a look at the README in our [tutorial repository](https://github.com/JKU-ICG/python-visualization-tutorial).

Then launch Jupyter Lab:
```
jupyter lab
```

Go to http://localhost:8888/ and open the *template* notebook.

Alternatively, you can also work with [binder](https://mybinder.org/), [deepnote](https://deepnote.com/), [colab](https://colab.research.google.com/), or any other service as long as the notebook runs in the standard Jupyter environment.

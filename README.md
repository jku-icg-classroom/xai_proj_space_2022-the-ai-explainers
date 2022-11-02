
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
| 11942036      | Abdul Basit | Banbhan        |abdul.banbhan@jku.at       |TODO           |
| 12126769      | Hala        | Al-Jarajrah    |k12126769@students.jku.at  |TODO           |
| 51903451      | Mohamed     | ELharty        |m.elharty@outlook.com      |TODO           |
| 12130348      | Nader       | Essam          |k12130348@students.jku.at  |TODO           |

### Dataset
Please add your dataset to the repository (or provide a link if it is too large) and answer the following questions about it:

* Which dataset are you using? What is it about?
* Where did you get this dataset from (i.e., source of the dataset)? How was the dataset generated?
* What is dataset size in terms of nodes, items, rows, columns, ...?
* What do you want to analyze?
* What are you expecting to see?

TODO


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
cd xai_proj_space_2022-<GROUP_NAME>
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

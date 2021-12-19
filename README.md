**If the notebook fails to load, please use [this](https://deepnote.com/viewer/github/mwstrand/Identifying-hentaigana-w-unsupervised-learning/blob/main/Hentaigana%20Analysis.ipynb) viewer**

The Kuzushiji-49 dataset contains 232,365 Japanese characters in the training data alone. The original author of this dataset states there may be mulitiple ways of writing certain characters (called Hentaigana, a typical feature of ancient Japanese writing). 

It is the interest of this project to identify and extract these different writing styles to see if prior knowledge of these differences will lead to more accurate classification. Specifically, we employ unsupervised clustering methods, including K-means, Guassian Mixture, and t-SNE. Accuracy is gauged using Pycart, which streamlines the modeling process and allows the convienent comparison of many models accross a range of metrics. 

This project was inspired by my machine learning course and my goal is to improve my understanding of unsupervised learning methods and working with large datasets.

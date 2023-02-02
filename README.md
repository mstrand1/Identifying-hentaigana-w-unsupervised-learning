**If the notebook fails to load, please use [this](https://deepnote.com/viewer/github/mwstrand/Identifying-hentaigana-w-unsupervised-learning/blob/main/Hentaigana%20Analysis.ipynb) viewer**

The Kuzushiji-49 dataset contains 232,365 Japanese characters in the training data alone. The original author of this dataset states there may be mulitiple ways of writing certain characters (called Hentaigana, a typical feature of ancient Japanese writing). However, data labels do not account for these different styles and collapse all the Hentaigana into 1 label. Training data for a computer vision program would therefore likely have more difficulty learning a label if it covers two very different styles of writing the same character.

It is the interest of this project to identify and extract these different writing styles to see if prior knowledge of these differences will lead to more accurate classification. I employ unsupervised clustering methods pipeline, including K-means, Guassian Mixture, and t-SNE. Specifically, I experiment with tuning the parameters of the t-SNE to better visualize the high-dimensional patterns in the images. Since t-SNE is not invertible, I simultaneously tune other, invertile, clustering methods for a best-guess match to t-SNE, in an attempt to capture stand-out clusters which may be Hentaigana. Accuracy is gauged using Pycart, which streamlines the modeling process and allows the convienent comparison of many models accross a range of metrics. 

This project was inspired by my undergraduate machine learning course and my goal is to improve my understanding of unsupervised learning methods and working with large datasets.

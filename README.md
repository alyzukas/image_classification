# Image Classification Project
Author: Alyssa Zukas <br>
Date: 2025-11-05

---


## Project Overview 

- **Introduction:** The purpose of the assignment is to perform work using the FastAI library and transfer learning to train a deep neural network to perform image classification using a data set from Kaggle. 

- **Domain Problem:** We want to develop a model to classify a bike based off of what it can see an image, into one of the following riding styles: Cross Country, Downhill, Enduro, Trail or Dirt Jumper.

- **Analytic Approach:** 
Since we will use labeled images of various bike categories to train a classifier how to predict bike types... we will be taking a predictive approach throughout this analysis.

- ### Main Source of Analysis
  - `bike_classification_analysis.ipynb` – main Colab notebook

 
### How to open
1. Click the **Open in Colab** badge below, or  
2. Download the `.ipynb` and open in Colab manually.


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1XsKqzbFj9eyMXD0FSJzkqPlVqSbCiW9T#scrollTo=g-Qcoom6f7ZE)

Please view the offical Google Powerpoint Deck [here](https://docs.google.com/presentation/d/1Ftzd1qzBMiUxn6lP-fI9CnoDlOWj28Pl_XpmsOq2cbY/edit?slide=id.gc6f9e470d_0_0#slide=id.gc6f9e470d_0_0).

---
## Project Structure

```
├── image_classification_template           # Google Colab Notebook and Python Scripts
├── image_classification_presentation       # Generated reports and visualizations
├── requirements.txt                        # Dependencies
└── README.md                               # Project documentation
```
---

## Data Sources

- This project utilizes one Kaggle folder: [Bike Ads (images, prices, specifications)](https://www.google.com/url?q=https%3A%2F%2Fwww.kaggle.com%2Fdatasets%2Ftysonpo%2Fbike-ads-images-prices-specifications)

  - Denoted in this notebook as `bike_ads`, this data set contains information from 10,052 bicycle advertisements in June 2020. Such as the ad title, main image, condition, and specification details (brand, color, frame, size, etc.) of the bike in the images.

  - Imported from the Kaggle data set, Bike Ads, we will use the images and specification attributes to train our model to classify bike types and riding styles.

  - The dataset is available for commercial/research purposes under a Creative Commons Corporation - [CC0 1.0 Universal License](https://www.google.com/url?q=https%3A%2F%2Fcreativecommons.org%2Fpublicdomain%2Fzero%2F1.0%2F). There is no copyright for this data. 

---

## Analysis

Google Colab Notebook

---

## Results 
Some of the images used to test the model are tough bikes to catagorize, even for a human being who knows a lot about bikes.
I knew that teaching a model to classify riding styles of a bike based off a set of visual variables would be hard - but I am actually surprised at what the model was able to output.

Overall, there are a lot of characteristics that go into defining the "riding style" of a bike.... and as you can tell... the way a bike is marketed is not always the riding style that it is mostly used for.

Things like geometry, wheel size, suspension, etc. all make a difference in the way the bike rides, and many riders purchase a bike marketed towards one type of riding style, yet use it for a completely different one. 
<br>
<br>
Based off the outputs, I do see how the model is classifying these bikes and I believe it did a fantastic job a analyzing these features to predict the riding style of the bike in each image, even if the "bike type" was not labeled the same!



---

## Authors 

- Alyssa Zukas - [@alyzukas](https://github.com/alyzukas)

---

## License

The dataset is available for commercial/research purposes under a [Creative Commons Corporation - CC0 1.0 Universal License](https://www.google.com/url?q=https%3A%2F%2Fcreativecommons.org%2Fpublicdomain%2Fzero%2F1.0%2F). 

---

## Tools and Libraries Used

This project leverages a combination of Python libraries for data processing, visualization, and deep learning:

- **Kagglehub**: For downloading datasets directly from Kaggle into Google Colab.
- **Json**:  For parsing and processing structured data from JSON files.
- **Pandas**:  For cleaning, merging, and manipulating tabular data.
- **Matplotlib.pyplot**: For creating static visualizations and plotting model results.
- **Seaborn**: For statistical data visualization and probability plots.
- **Os**: For file and directory operations.
- **Requests**: For retrieving and downloading image data from URLs.
- **Tqdm**: For displaying progress bars during data download and preprocessing loops.
- **FastAI**: For training and testing the model - mainly the vision_learner and Classification Interpretation features


## Acknowledgements
    
- Tutorials or papers referenced: DATA 5100 Class modules
- Inspiration or collaborators: Dr Fischer







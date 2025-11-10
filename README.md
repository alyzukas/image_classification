# Image Classification Project
Author: Alyssa Zukas <br>
Date: 2025-11-05


### How to open
1. Click the **Open in Colab** badge below, or  
2. Download the `.ipynb` and open in Colab manually.


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1XsKqzbFj9eyMXD0FSJzkqPlVqSbCiW9T#scrollTo=g-Qcoom6f7ZE)

Please view the offical Google Powerpoint Deck [here](https://docs.google.com/presentation/d/1Ftzd1qzBMiUxn6lP-fI9CnoDlOWj28Pl_XpmsOq2cbY/edit?slide=id.gc6f9e470d_0_0#slide=id.gc6f9e470d_0_0)

---


## Project Overview 

- **Introduction:** The purpose of the assignment is to perform work using the FastAI library and transfer learning to train a deep neural network to perform image classification using a data set from Kaggle. 

- **Domain Problem:** We want to develop a model to classify a bike based off of what it can see an image, into one of the following riding styles: Cross Country, Downhill, Enduro, Trail or Dirt Jumper.

- **Analytic Approach:** 
Since we will use labeled images of various bike categories to train a classifier how to predict bike types... we will be taking a predictive approach throughout this analysis.

- ### Main Source of Analysis
  - `image_classification_template.ipynb` – main Colab notebook

---
## Project Structure

```
├── image_classification_template     # Google Colab Notebook and Python Scripts
├── image_classification_presentation      # Generated reports and visualizations
├── requirements.txt                  # Dependencies
└── README.md                         # Project documentation
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
Some of the images used above are tough bikes to catagorize, even for a human being who knows a lot about bikes.
I knew that teaching a modle to classify riding styles of a bike based off a set of visual variables would be hard - but I am actually surprised at what the model was able to output.
<br>
<br>
For example:

- In Image 1, it is a fair analysis that the model put this as both cross_country and trail... because this is a popular bike used for both cross country and trail riding!

- In Image 2, altough this bike is marketed as an enduro bike, many riders actually do use this as a dirt_jumper... so again, the models display was actually not "inaccurate", and I am very impressed that it was able to pick up on this.

- In Image 3, the model shows higher confidence in trail riding style.. and this is accurate! The modle displaying some efforts towards the other catagories makes sense - as the bikes fork (front suspension) is usually used for enduro bikes. This tells me that the model was able to pick up on these idfferences while still taking the other details into consideration.

- In Image 4, this image used is of a very new bike in the market. So new that only professional riders get access to it as of now. The model predicted this as an enduro bike, and although that is not how this bike is marketed as, many of the prefessional riders assigned to test-riding this bike are saying that it rides more like an enduro bike.

Overall, there are a lot of characteristics that go into the "riding style" of a bike.... and as you can tell... the way a bike is marketed is not always the riding style that it is mostly used for.
<br>
<br>
Things like geometry, wheel size, suspension, etc. all makr a difference in the way the bike rides, thus a lot of bike companies are tending to interchange these features to make hybrid-like bikes. I guess you can call this a marketing tactic.
<br>
<br>
Based off of the outputs, I do see how the model is classifying these bikes and I believe it did a fantastic job a analyzing these features to predict the riding style of the bike in each image!
Expanding this analysis further by analyzing this across multiple years allows us to pick up any potential trends. 


---

## Authors 

- Alyssa Zukas - [@alyzukas](https://github.com/alyzukas)

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Tools and Libraries Used

This project leverages a combination of Python libraries for data processing, visualization, and deep learning:

- **kagglehub** – for downloading datasets directly from Kaggle into Google Colab.
- **json** – for parsing and processing structured data from JSON files.
- **pandas** – for cleaning, merging, and manipulating tabular data.
- **matplotlib.pyplot** – for creating static visualizations and plotting model results.
- **seaborn** – for statistical data visualization and probability plots.
- **os** – for file and directory operations.
- **requests** – for retrieving and downloading image data from URLs.
- **tqdm** – for displaying progress bars during data download and preprocessing loops.
- **fastai.v**


## Acknowledgements
    
- Tutorials or papers referenced: DATA 5100 Class modules
- Inspiration or collaborators: Dr Fischer







# Benchmarking cosmetics by ingredients
<figure>
  <img src="https://github.com/xaviermmi/academic-projects/assets/122324304/ebf73918-2a96-4f61-8a26-2f210c9f0fe0" alt="title">
  <figcaption>Photo de <a href="https://unsplash.com/fr/@mikelina5?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">michela ampolo</a> sur <a href="https://unsplash.com/fr/photos/7tDGb3HrITg?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a></figcaption>
</figure>
  

## 1. Introduction
<p>Whenever I want to try a new cosmetic item, it's so difficult to choose. It's actually more than difficult. It's sometimes scary because new items that I've never tried end up giving me skin trouble. We know the information we need is on the back of each product, but it's really hard to interpret those ingredient lists unless you're a chemist. You may be able to relate to this situation.</p>
<p><img src="https://github.com/xaviermmi/academic-projects/assets/122324304/0f29a3d9-f7b7-4ea3-9afd-88002051c27b"
 style="width:800px;height:600px;"></p>
<p>So instead of buying and hoping for the best, why don't we use data science to help us predict which products may be good fits for us?

## 2. Project instructions
In this notebook, we are going to create a content-based recommendation system where the 'content' will be the chemical components of cosmetics. Specifically, we will process ingredient lists for 1472 cosmetics on Sephora via <a href="https://en.wikipedia.org/wiki/Word_embedding">word embedding</a>, then visualize ingredient similarity using a machine learning method called t-SNE and an interactive visualization library called Bokeh. Let's inspect our data first.</p>

## 3. Dataset
<p>We'll use the file "cosmetics.csv" located in the "datasets" subdirectory.
  
## 4. Skills
<p>This project is showcasing some text mining, unsupervised learning and datavisualization techniques : 
<ul>
<li>text mining : we'll tokenize the ingredients info and build a Document-Term Matrix (also called DTM)
<li>unsupervised learning : we'll use a dimensionality reduction technique (called T-SNE) to drastically shrink the number of features from 2233 to only 2 features
<li>dataviz : we'll use Bokeh to dynamically observe our resulting 2 features, including a hover-tool to catch important info (like item name, brand, price, etc.)</li>
</ul>

## 5.Notebook structure
The structure of this notebook is as follows:</p>
<ul>
<li>We'll first take a quick look at the dataset to observe categories and usefull features (actually a mix of numeric and text features)
<li>We'll then subset the dataframe to focus on a specific category
<li>Next we'll build an empty DTM (Document-Term Matrix) by tokenizing ingredients and listing unique product names
<li>then build a custom one-hot encoding function to catches ingredients frequency to fill-in the DTM
<li>The T-SNE model will then by applied to the matrix, resulting in a 2-dimensions resultant
<li>Finally, Bokeh will allow us to show this 2-dim result in a dynamic graph with tooltips indicating main product characteristics usefull for products benchmark</li>
</ul>

## 6.Result
![example_product_tsne](https://github.com/xaviermmi/academic-projects/assets/122324304/0e9f90c1-4206-455d-b31f-130e73d5dc65)


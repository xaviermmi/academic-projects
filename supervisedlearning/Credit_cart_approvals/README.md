# Predicting credict card approvals
<figure style="font-size:12px;height:1000px">
  <img src="https://github.com/xaviermmi/academic-projects/assets/122324304/9fd785d3-e44a-4683-9949-182260fe7fe0" alt="amex-card-unsplash">
  <figcaption>Photo by <a href="https://unsplash.com/@cardmapr?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">CardMapr.nl</a> on <a href="https://unsplash.com/photos/i-t4zL1Nqc0?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a></figcaption>
</figure>


## 1. Introduction
<p>Commercial banks receive <em>a lot</em> of applications for credit cards. Many of them get rejected for many reasons, like high loan balances, low income levels, or too many inquiries on an individual's credit report, for example.</p>
<p>Manually analyzing these applications is mundane, error-prone, and time-consuming (and time is money!). Luckily, this task can be automated with the power of machine learning and pretty much every commercial bank does so nowadays.</p>

## 2. Project instructions
In this notebook, we will build an automatic credit card approval predictor using machine learning techniques, just like the real banks do.

## 3. Dataset
<p>We'll use the <a href="http://archive.ics.uci.edu/ml/datasets/credit+approval">Credit Card Approval dataset</a> from the UCI Machine Learning Repository.
<p>Important note : 
Since this data is confidential, the contributor of the dataset has anonymized the feature names.</p>
  
## 4. Skills
<p>This project is showcasing some supervized machine learning techniques mainly focused on preprocessing and classification, using a logistic regression algorithm.</p>
<p>In terms of code, we use :
<ol>
<li><code>pandas</code> for data manipulation, summary statistics and basic preprocessing (oh-encoder, simple imputation)
<li><code>numpy</code> for handling missing values
<li><code>scikit-learn</code> for :
  <ul>
  <li>filtering (test/train sets) and preprocessing (scaling) our dataset
  <li>building and evaluating our linear model (logistic regression)
  <li>running a cross-validation and defining the best parameters for our model</li>
  </ul>
</li></ol></p>

## 5.Notebook structure
The structure of this notebook is as follows:</p>
<ul>
<li>First, we will start off by loading and viewing the dataset.
<li>We will see that the dataset has a mixture of both numerical and non-numerical features, that it contains values from different ranges, plus that it contains a number of missing entries.
<li>We will have to preprocess the dataset to ensure the machine learning model we choose can make good predictions.
<li>After our data is in good shape, we will build a machine learning model that can predict if an individual's application for a credit card will be accepted.
<li>Finally we will apply a grid-search cross-validation to optimize our model</li>
</ul>

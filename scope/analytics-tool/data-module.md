---
description: Data analytics functions.
icon: chart-mixed
---

# Data Module

## Upload and organize data

Besides [hands-on practice](../exercise-platform.md#hands-on-datasets-practice), you can also analyze your own data by uploading your own datasets in CSV format.

{% hint style="warning" %}
**Note**: Both public datasets and uploaded datasets share the same excel-like interface.
{% endhint %}

1.  Click "New Dataset" button.

    <figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption><p>My Datasets</p></figcaption></figure>
2.  In the pop-up window, enter the dataset name you prefer and upload your dataset.

    _**It may cause up to 1 minute to upload your dataset.**_

    <div align="left"><figure><img src="../../.gitbook/assets/1748026606610.png" alt=""><figcaption><p>Click to upload</p></figcaption></figure></div>
3.  &#x20;Once your dataset is uploaded, you can find it under "My Datasets" section.

    <figure><img src="../../.gitbook/assets/1748547749532.png" alt=""><figcaption><p>Uploaded file</p></figcaption></figure>

## Data Analysis

After selecting an appropriate dataset, we are ready for data analysis. We'll take "Titanic" dataset as an example.

We have 4 different steps for data analysis in our tool — Data Preporcessing, Data Processing, Model and Results. Let's look through them one by one.

### Data Preprocessing

#### Detail

We present the data you want to analyze in an excel-like interface, where you can finalize the data type for each column. We have 3 different data types:

1. Integer:
2. Category:
3. Float:

In Titanic dataset, we want to make column "survived" categorical data, as indicated below:

<figure><img src="../../.gitbook/assets/1748570560856.png" alt=""><figcaption><p>Change data type</p></figcaption></figure>

If you have plenty of columns, and you want to do batch processing, you can simply click "Batch process" button <img src="../../.gitbook/assets/1748559604509.png" alt="" data-size="line">on the top right corner, then you can select target type (Integer, Category or Float) and pattern (hover on the info icon <img src="../../.gitbook/assets/1748560485074.png" alt="" data-size="line"> for the explanation).

<figure><img src="../../.gitbook/assets/1748554152761.png" alt=""><figcaption><p>Batch process</p></figcaption></figure>

#### Summary

When you click "Summary" tab, you can also get the summary of the data, including basic information of the data, distribution of numerical and categorical features, etc.

<figure><img src="../../.gitbook/assets/1748554492304.png" alt=""><figcaption><p>Data summary</p></figcaption></figure>

### Data Processing

#### Prediction Label

In Titanic dataset, we want to predict if a person is survived or not, so we select "survived" as the prediction label. The column "survived" will be locked by green color.

<figure><img src="../../.gitbook/assets/1748571180495.png" alt=""><figcaption><p>Prediction label</p></figcaption></figure>

#### Ignored Features

You can select any features you would like to ignore in your data, or if you want to keep all the features, just skip this step. In Titanic dataset, we take features of "sibsp" and "embarked" as an example. The corresponding columns become disabled.

<figure><img src="../../.gitbook/assets/1748578195312.png" alt=""><figcaption><p>Ignored Features</p></figcaption></figure>

#### Missing Data

There are 3 different ways to handle missing values — mean, median and KNN (K-nearest neighbors), you can select based on your own needs.  We take mean as an example.

{% hint style="warning" %}
Note: these 3 methods only work on numerical data. If you want to take care of categorical data, you want to consider it as a category, and tale care of it under [Categorical Encoding Method](data-module.md#categorical-encoding-method).
{% endhint %}

<figure><img src="../../.gitbook/assets/1748579789842.png" alt=""><figcaption><p>Handle missing data</p></figcaption></figure>

#### Categorical Encoding Method&#x20;

For all the categorical data, you can encode them by 2 options — label encoding and onehot encoding.&#x20;

Label encoding:

<figure><img src="../../.gitbook/assets/1748580674472.png" alt=""><figcaption><p>Label  encoding</p></figcaption></figure>

Onehot encoding:

<figure><img src="../../.gitbook/assets/1748582141608.png" alt=""><figcaption><p>Onehot encoding</p></figcaption></figure>

_We take onehot encoding as an example._

#### Numerical Normalization

You can choose to use either minmax or standard normalization method to normalize your data.

Minmax:

<figure><img src="../../.gitbook/assets/1748582536341.png" alt=""><figcaption><p>Minmax</p></figcaption></figure>

Standard:

<figure><img src="../../.gitbook/assets/1748582665951.png" alt=""><figcaption><p>Standard</p></figcaption></figure>

_We take minmax as an example._

{% hint style="info" %}
At any time, you can return to the previous step and adjust your selections.

After all the data processing tasks, you can now proceed to the _Model_ section by simply clicking "Next" button.
{% endhint %}

## Models

### Supervised Learning

#### Supervised Learning Classification



<figure><img src="../../.gitbook/assets/1748629242751.png" alt=""><figcaption><p>Supervised learning classification models</p></figcaption></figure>

#### Supervised Learning Regression

<figure><img src="../../.gitbook/assets/1748630122939.png" alt=""><figcaption></figcaption></figure>

### Unsupervised learning

<figure><img src="../../.gitbook/assets/1748629716273.png" alt=""><figcaption><p>Unsupervised learning models</p></figcaption></figure>

### Visualization

In the _Model_ section, you can choose to visualize your data using one of three major models—PCA, t-SNE, and UMAP (highlighted in the red dashed rectangle). See image below:

<figure><img src="../../.gitbook/assets/1748629954281.png" alt=""><figcaption><p>Visualization models</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/1739425318841.png" alt=""><figcaption><p>Visualize data</p></figcaption></figure>

## Results

After selecting your preferred models, you can proceed to the _Results_ section, where you can see the details of Performance, Feature Coefficients and Feature Importance.

### Results for Supervised Learning

<figure><img src="../../.gitbook/assets/1739426462470.png" alt=""><figcaption><p>Supervised learning results</p></figcaption></figure>

### Results for Unsupervised Learning

We also offer various unsupervised learning models, see the image below:

<figure><img src="../../.gitbook/assets/1739426518189.png" alt=""><figcaption><p>Unsupervised learning models</p></figcaption></figure>

Similarly, after selecting your preferred models, you can proceed to the _Results_ section, where you can see the clustering details.

<figure><img src="../../.gitbook/assets/1739426702806.png" alt=""><figcaption><p>Unsupervised learning results</p></figcaption></figure>

### Results for Visualization


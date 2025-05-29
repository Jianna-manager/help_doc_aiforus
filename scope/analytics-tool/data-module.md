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

We present the data you want to analyze in an excel-like interface, where you can finalize the data type for each column. We have 3 different data types as shown in the picture below:

1. Integer:
2. Category:
3. Float:

<figure><img src="../../.gitbook/assets/1748551959580.png" alt=""><figcaption><p>Change data type</p></figcaption></figure>

If you have plenty of columns, you can simply click "Batch process" button <img src="../../.gitbook/assets/1748559604509.png" alt="" data-size="line">on the top right corner, then you can select target type (Integer, Category or Float) and pattern (hover on the info icon <img src="../../.gitbook/assets/1748560485074.png" alt="" data-size="line"> for the explanation).

<figure><img src="../../.gitbook/assets/1748554152761.png" alt=""><figcaption><p>Batch process</p></figcaption></figure>

#### Summary

When you click "Summary" tab, you can also get the summary of the data, including basic information of the data, distribution of numerical and categorical features, etc.

<figure><img src="../../.gitbook/assets/1748554492304.png" alt=""><figcaption><p>Data summary</p></figcaption></figure>

### Data Processing

#### Prediction Label

1.  For example, we choose "survived" as prediction label, shown as image below.

    <figure><img src="../../.gitbook/assets/1739422730001.png" alt=""><figcaption><p>Prediction label</p></figcaption></figure>

#### Ignore Features

You can select any features you would like to ignore.

<figure><img src="../../.gitbook/assets/1739423227256.png" alt=""><figcaption><p>Ignore Features</p></figcaption></figure>

#### Missing Data

There are 3 different ways to handle missing values — Mean, median and KNN (K-nearest neighbors), you can select based on your own needs.

<figure><img src="../../.gitbook/assets/1739423485234.png" alt=""><figcaption><p>Handle Missing Values</p></figcaption></figure>

#### Categorical Encoding Method&#x20;

For all the categorical data, you can encode them by 2 options — label encoding and onehot encoding, as shown below.

<figure><img src="../../.gitbook/assets/1739424021316.png" alt=""><figcaption><p>Encode Categorical Data</p></figcaption></figure>

#### Numerical Normalization

You can choose to use either minmax or standard method to normalize your data.

<figure><img src="../../.gitbook/assets/1739424261927.png" alt=""><figcaption><p>Normalize Standardize Data</p></figcaption></figure>

<mark style="color:red;">**Note:**</mark>

In this case, "survived" is a categorical label, so you want to make sure the "TYPE" of this feature is "Category". You can achieve this by selecting "Category" in the dropdown list under "survived" <img src="../../.gitbook/assets/1739423779697.png" alt="" data-size="line">.

At any time, you can return to the previous step and adjust your selections.

After all the data processing tasks, you can now proceed to the _Model_ section by simply clicking "Next" button.

## Visualize data

In the _Model_ section, you can choose to visualize your data using one of three major models—PCA, t-SNE, and UMAP (highlighted in the red dashed rectangle). See image below:

<figure><img src="../../.gitbook/assets/1739425318841.png" alt=""><figcaption><p>Visualize data</p></figcaption></figure>

## Implement supervised/unsupervised learning

### Supervised learning

We offer various supervised learning models, see the image below:

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption><p>Supervised learning models</p></figcaption></figure>

After selecting your preferred models, you can proceed to the _Results_ section, where you can see the details of Performance, Feature Coefficients and Feature Importance.

<figure><img src="../../.gitbook/assets/1739426462470.png" alt=""><figcaption><p>Supervised learning results</p></figcaption></figure>

### Unsupervised learning

We also offer various unsupervised learning models, see the image below:

<figure><img src="../../.gitbook/assets/1739426518189.png" alt=""><figcaption><p>Unsupervised learning models</p></figcaption></figure>

Similarly, after selecting your preferred models, you can proceed to the _Results_ section, where you can see the clustering details.

<figure><img src="../../.gitbook/assets/1739426702806.png" alt=""><figcaption><p>Unsupervised learning results</p></figcaption></figure>

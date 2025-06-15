---
description: Step-by-step explanation of visualization.
---

# Use Case: Visualization

## Models

<figure><img src="../../../.gitbook/assets/image (3).png" alt=""><figcaption><p>Visualization models</p></figcaption></figure>

Visualization methods are also within unsupervised learning realm, we provide three widely used **dimensionality reduction techniques**. These techniques reduce the number of features (dimensions) in a dataset while **preserving meaningful structure**.

*   PCA (Principal Component Analysis)

    A **linear** dimensionality reduction method that transforms features into new variables (called **principal components**) that capture the most **variance** in the data.

    * Good for linearly correlated features
    * Mathematically interpretable
    * Can miss complex, non-linear structures
*   t-SNE (t-distributed Stochastic Neighbor Embedding)

    A **non-linear** method for visualizing high-dimensional data in 2D or 3D by focusing on **local similarities** (neighborhoods).

    * Excellent for **visual clustering**
    * Not good for preserving global structure
    * Cannot be used to transform new data (non-parametric)
*   UMAP (Uniform Manifold Approximation and Projection)

    A **non-linear** technique like t-SNE but **faster, scalable**, and preserves more **global structure**.

    * Fast and scalable
    * Can be used to transform new data (unlike t-SNE)
    * Captures both **local and global** relationships

### Comparison

| Feature                           | PCA                            | t-SNE              | UMAP                         |
| --------------------------------- | ------------------------------ | ------------------ | ---------------------------- |
| Linear / Non-linear               | Linear                         | Non-linear         | Non-linear                   |
| Best use                          | Preprocessing, noise reduction | Data visualization | Visualization, preprocessing |
| Preserves global structure        | ✅ Yes                          | ❌ No               | ✅ Partial                    |
| Preserves local structure         | ⚠️ Partial                     | ✅ Excellent        | ✅ Excellent                  |
| Suitable for new data (transform) | ✅ Yes                          | ❌ No               | ✅ Yes                        |
| Computational speed               | ✅ Fast                         | ❌ Slow             | ✅ Fast                       |
| Interpretable output              | ✅ Yes (components)             | ❌ No               | ❌ No                         |

| Situation                                         | Recommended Method | Why?                                            |
| ------------------------------------------------- | ------------------ | ----------------------------------------------- |
| You want to reduce features before model training | PCA or UMAP        | PCA is interpretable; UMAP handles non-linear   |
| You want to **visualize clusters** in 2D/3D       | t-SNE or UMAP      | Both are designed for human-interpretable plots |
| You have **very high-dimensional, sparse data**   | UMAP               | More scalable than t-SNE                        |
| You need to apply the model to **new data**       | PCA or UMAP        | t-SNE cannot transform new inputs               |
| You want **interpretable features**               | PCA                | Components are mathematically meaningful        |

## Results

The results are shown below. You can select different methods, indicated in the red rectangle.

<figure><img src="../../../.gitbook/assets/1749358316928 (1).png" alt=""><figcaption><p>Visualization results</p></figcaption></figure>

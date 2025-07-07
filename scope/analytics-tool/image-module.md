---
description: Image recognition methods.
icon: image-landscape
---

# Image Module

We offer three image recognition methods: **Easy OCR**, **Object Detection**, and **Image Classification**. Try out all three and have fun exploring what each can do!

Using any of these methods is simple—just follow two steps — **Upload image** and **Click "Submit".**

## Easy OCR

**Easy OCR** is an open-source tool that uses Optical Character Recognition (OCR) technology to detect and extract text from images. It supports multiple languages and works well with a variety of image types.

In our tool, you can use Easy OCR to quickly and accurately recognize text within your uploaded images.

<figure><img src="../../.gitbook/assets/1748061136952.png" alt=""><figcaption><p>Easy OCR</p></figcaption></figure>

## Object Detection

**Object Detection** is a computer vision task that identifies and locates multiple objects within an image. It not only classifies objects (e.g., “car,” “dog,” “person”) but also draws bounding boxes around them to indicate their positions.

In our tool, you’ll receive an output image with bounding boxes and corresponding object labels clearly displayed.

<figure><img src="../../.gitbook/assets/1748061180630.png" alt=""><figcaption><p>Object Detection</p></figcaption></figure>

## Image Classification

**Image Classification** is the process of assigning a single label to an entire image based on its overall content. Unlike object detection, it doesn't identify the location of specific objects but instead categorizes the whole image into a predefined class.

In our tool, once you upload an image, you’ll receive the classification result along with the confidence percentages for each possible category.

<figure><img src="../../.gitbook/assets/1748061252655.png" alt=""><figcaption><p>Image Classification</p></figcaption></figure>

## Comparison Table

<table><thead><tr><th width="161.28564453125">Feature</th><th>EasyOCR</th><th>Object Detection</th><th>Image Classification</th></tr></thead><tbody><tr><td><strong>Purpose</strong></td><td>Extracts text from images</td><td>Identifies and locates multiple objects</td><td>Assigns a single label to the entire image</td></tr><tr><td><strong>Output</strong></td><td>Text (string)</td><td>Object labels + bounding boxes</td><td>Single class label</td></tr><tr><td><strong>Input</strong></td><td>Image with text</td><td>Image with multiple objects</td><td>Image representing one category</td></tr><tr><td><strong>Localization</strong></td><td>No (text is extracted, not located precisely)</td><td>Yes (each object is localized)</td><td>No (only whole-image classification)</td></tr><tr><td><strong>Typical Use Cases</strong></td><td>Reading documents, receipts, signs</td><td>Detecting cars, people, products</td><td>Sorting images by category (e.g., cat/dog)</td></tr></tbody></table>

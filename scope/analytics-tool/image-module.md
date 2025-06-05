---
description: Image recognition methods.
icon: image-landscape
---

# Image Module

We offer 3 different image recognition methods — Easy OCR, Object Detection and Image Classification. Please try all of the 3 methods and have fun with each of them!

There are only 2 simple steps needed when applying each method — **Upload image** and **Click "Submit".**

## Easy OCR

Easy OCR is an open-source tool that uses **Optical Character Recognition (OCR) technology** to detect and extract text from images. It supports **multiple languages**.

In our tool, we can help you recognize the text in the image.

<figure><img src="../../.gitbook/assets/1748061136952.png" alt=""><figcaption><p>Easy OCR</p></figcaption></figure>

## Object Detection

Object detection is a **computer vision task** that identifies and locates **multiple objects** within an image. It not only classifies objects (e.g., “car”, “dog”, “person”) but also draws **bounding boxes** around them to indicate their positions.

In our tool, we can provide you the image with bounding boxes, along with the object names.

<figure><img src="../../.gitbook/assets/1748061180630.png" alt=""><figcaption><p>Object Detection</p></figcaption></figure>

## Image Classification

Image classification is a process where a model assigns a **single label** to an entire image, based on its content. Unlike object detection, it does not locate specific objects but rather **categorizes** the whole image into a predefined class.

In out tool, after you upload an image, we can output the image classification result, along with the percentage for each possible outcome.

<figure><img src="../../.gitbook/assets/1748061252655.png" alt=""><figcaption><p>Image Classification</p></figcaption></figure>

## Comparison Table

<table><thead><tr><th width="161.28564453125">Feature</th><th>EasyOCR</th><th>Object Detection</th><th>Image Classification</th></tr></thead><tbody><tr><td><strong>Purpose</strong></td><td>Extracts text from images</td><td>Identifies and locates multiple objects</td><td>Assigns a single label to the entire image</td></tr><tr><td><strong>Output</strong></td><td>Text (string)</td><td>Object labels + bounding boxes</td><td>Single class label</td></tr><tr><td><strong>Input</strong></td><td>Image with text</td><td>Image with multiple objects</td><td>Image representing one category</td></tr><tr><td><strong>Localization</strong></td><td>No (text is extracted, not located precisely)</td><td>Yes (each object is localized)</td><td>No (only whole-image classification)</td></tr><tr><td><strong>Typical Use Cases</strong></td><td>Reading documents, receipts, signs</td><td>Detecting cars, people, products</td><td>Sorting images by category (e.g., cat/dog)</td></tr></tbody></table>

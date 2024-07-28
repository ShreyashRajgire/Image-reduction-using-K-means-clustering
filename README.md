# Image Compression with K-Means Clustering (R)

This project demonstrates image compression using k-means clustering, a powerful unsupervised machine learning algorithm for grouping similar data points. While this example focuses on image processing, k-means clustering has wide-ranging applications across various business domains.

## Technical Overview

This project uses k-means to reduce the number of colors in an image, effectively compressing its size. Here's how it works:

1. **Image Loading:** Reads a JPEG image and represents it as a data frame, where each row corresponds to a pixel and its RGB color values.
2. **Color Quantization with K-Means:** Applies k-means to group similar colors together in RGB space. Each cluster center represents a dominant color in the compressed image. The number of clusters ('k') controls the compression level.
3. **Image Reconstruction:**  Replaces each pixel's original color with the representative color of its assigned cluster, reconstructing the image with a reduced color palette. 

## Example Usage and Results

The code demonstrates this process using different 'k' values. The results illustrate the trade-off between compression and image quality.

**Original Image:**
![image](https://github.com/user-attachments/assets/ce56df34-7b42-4467-baf6-5499030ef31b)

| k = 3                     | k = 5                     | k = 8                     |
|-----------------------------|-----------------------------|-----------------------------|
| ![k=3](https://github.com/user-attachments/assets/42eb58bf-77a9-4409-89b7-0faa8cb01418) | ![k=5](https://github.com/user-attachments/assets/a01657b0-22ea-48e3-a628-75ae5d74a946) | ![k=8](https://github.com/user-attachments/assets/be44fb19-977a-4cd0-9e63-1b85faa1d6c7) |

## K-Means Clustering: Business Applications

Beyond image compression, k-means is a versatile tool for various business problems:

* **Customer Segmentation:** Group customers with similar behaviors for targeted marketing.
* **Anomaly Detection:** Identify unusual data points that might indicate fraud or errors.
* **Inventory Management:** Optimize inventory levels by clustering products with similar demand.
* **Document Analysis:** Group documents by topic for efficient search and analysis.
* **Recommendation Systems:**  Create personalized recommendations by clustering users with similar preferences. 

**And more:** K-means has applications in healthcare, finance, manufacturing, and many other industries.

# 🎨 Dominant-Color-Extraction-from-Images
This project extracts and visualizes the dominant colors in an image using KMeans clustering. The extracted colors are matched to the closest named colors from a CSV file containing color names and RGB values. The script dynamically estimates the number of clusters needed for KMeans based on the complexity of the image.
## Features
- Image Loading: Load and resize images for faster processing.
- Color Extraction: Extract and cluster dominant colors from images.
- Dynamic Clustering: Automatically estimate the optimal number of clusters based on image complexity.
- Color Matching: Match extracted colors to named colors from a reference CSV file.
- Visualization: Display dominant colors and their closest matches.
## Prerequisites
Ensure you have Python 3.x installed along with the following libraries:
- Pillow
- NumPy
- pandas
- matplotlib
- scikit-learn
- scipy

Install the required libraries using pip:
> pip install pillow numpy pandas matplotlib scikit-learn scipy

## Code Explanation
1. Image Loading and Resizing: The image is loaded and resized for faster processing.
2. Color Extraction: The image is converted into RGB values, and KMeans clustering is applied to identify dominant colors.
3. Dynamic Clustering: The number of clusters is estimated based on the number of pixels in the image. The function estimate_clusters_based_on_image calculates a suitable number of clusters.
4. Color Matching: The dominant colors are matched to the closest named colors in the CSV file using Euclidean distance.
5. Visualization: The dominant colors and their closest matches are displayed using Matplotlib.


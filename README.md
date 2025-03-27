# Context Based Image Retrieval
An intelligent image retrieval system powered by convolutional neural networks

## Project Description
This application enables users to find visually similar images from a database by using a query image. Leveraging advanced Computer Vision algorithms, the system analyzes image content and identifies matches based on visual features rather than metadata or tags.

## Technical Implementation
1. Utilizes a pre-trained CNN (VGG19) originally trained on ImageNet to process images
2. Extracts high-dimensional feature vectors from the penultimate layer (fc2) of the network
3. Applies dimensionality reduction via PCA to create compact image representations
4. Stores processed feature vectors and PCA model for efficient retrieval
5. At runtime, processes query images through the same pipeline
6. Computes Euclidean distance between query features and database features
7. Returns the top 5 most similar images based on feature similarity

## Getting Started
1. Install all required dependencies listed in requirements.txt
2. Place your image collection in the 'dataset' folder
3. Run the feature extraction script to process your image database
4. Launch the main application to start searching for similar images

## User Interface
- Use the 'select image' button to choose your query image
- Click 'view matches' to display the most similar images from your collection
- Results are displayed visually in the application window


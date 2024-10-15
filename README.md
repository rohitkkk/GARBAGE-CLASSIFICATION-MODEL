Deep CNN for Garbage Classification:

This project utilizes a Convolutional Neural Network (CNN) to automate the classification of waste images into "organic" and "recyclable" categories. It demonstrates the complete machine learning pipeline, from data preprocessing to model training, evaluation, and deployment, aiming to improve waste management and recycling efficiency.
Project Structure:

Download the dataset:

https://archive.ics.uci.edu/dataset/908/realwaste

Tools and Libraries:

The following tools and libraries were used to develop and run this project:

TensorFlow: Framework used to build and train the CNN model.
Google Colab: Cloud-based platform for running Jupyter notebooks with GPU acceleration.
OpenCV: For loading and preprocessing images (e.g., resizing, scaling).
NumPy: For array manipulations and numerical computations.
Matplotlib: For plotting and visualizations.
TensorBoard: Used for monitoring and visualizing training metrics (e.g., loss, accuracy).

Model Training and Evaluation:

The model is a CNN with the following architecture:

Convolutional Layers: Used for feature extraction.
MaxPooling Layers: For downsampling.
Dense (Fully Connected) Layers: To perform classification.
Activation Functions: ReLU for intermediate layers, sigmoid for the output layer.
The model is compiled with:

Optimizer: Adam
Loss Function: Binary Cross-Entropy
Metrics: Accuracy
Training details:

Epochs: 8
Batch Size: Adjustable in the code
Validation Split: The dataset is split into training (70%), validation (20%), and test (10%) sets.
The model is trained on Google Colab using a T4 GPU.

Results:

Accuracy:0.9458333253860474
Precision: 0.9670329689979553
Recall:0.8979591727256775

Visualisation of 8 epochs History:

![image](https://github.com/user-attachments/assets/7bf86a04-6cba-4d83-a0e0-aab73db4e94f)

![image](https://github.com/user-attachments/assets/abbb8dc8-3df6-4375-b8aa-9e833f6672ba)

Demo output:

![image](https://github.com/user-attachments/assets/7a73cdc4-6802-499a-9786-349dd1950246)


Deployment:

The trained model is saved as wasteclassifier103.h5 in the models/ directory. To make real-time predictions:

Load the model:
model = load_model('models/wasteclassifier103.h5')


References: 
- https://www.youtube.com/watch?v=jztwpsIzEGc&list=WL&index=22&pp=gAQBiAQB
- TensorFlow documentation
- OpenCV tutorials for image processing


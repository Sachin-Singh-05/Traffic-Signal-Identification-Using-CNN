Traffic Signal Classification using CNN

Project Overview :-

This project focuses on building a Convolutional Neural Network (CNN) to classify traffic signals from images.
The model learns visual patterns such as shapes, colors, and symbols to accurately identify different traffic signs.

Objectives :-

* Build a deep learning model for image classification
* Classify multiple traffic signal categories
* Evaluate model performance using accuracy and loss metrics
* Visualize training progress using graphs

Dataset :-
The dataset consists of traffic signal images and corresponding labels.

Structure

```
traffic_dataset/
│
├── DATA/          # Training images
├── TEST/          # Testing images
├── labels.csv     # Image labels
```

* Images are resized to *32x32 pixels*
* Labels are encoded using *one-hot encoding*

Model Architecture :-

The CNN model consists of:

* 3 Convolutional Layers (feature extraction)
* 3 MaxPooling Layers (dimensionality reduction)
* Flatten Layer
* Dense Layer (Fully Connected)
* Dropout Layer (to reduce overfitting)
* Output Layer (Softmax activation)

Technologies Used :-

* Python 
* TensorFlow / Keras
* NumPy
* Pandas
* Matplotlib
* OpenCV

How to Run :-
1. Clone the repository

```
git clone https://github.com/your-username/traffic-signal-classification.git
cd traffic-signal-classification
```

2. Install dependencies

```
pip install -r requirements.txt
```

3. Run the model

```
python main.py
```

---

Model Training :-

* Optimizer: Adam
* Loss Function: Categorical Crossentropy
* Epochs: 15
* Batch Size: 32

Results :-

The model performance is evaluated using:

* Training Accuracy : 92.65%
* Validation Accuracy : 98.93%
* Training Loss : 0.224
* Validation Loss : 0.0479

Sample Graphs :-

* Accuracy vs Epoch
* Loss vs Epoch

Model Analysis :-

* CNN layers extract features such as edges, shapes, and patterns
* Dense layers perform classification
* Dropout helps reduce overfitting

Output Example :-

The model predicts traffic signals such as:
* Stop
* Speed Limit
* No Entry
* Yield

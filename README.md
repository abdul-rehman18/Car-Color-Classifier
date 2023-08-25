# Vehicle-Color-Recognition-Using-CNN

The Vehicle-Color-Recognition is a Flask-based ML model that utilizes a trained deep learning model (CNN) to predict the color of cars in images. The model provides a user interface to upload car images and receive predictions for their colors. Additionally, it evaluates the model's performance on a provided test dataset and generates a confusion matrix to visualize the results.

# Prerequisites

To run the Vehicle-Color-Recognition model, you need to have the following installed:

- Python
- TensorFlow & Keras
- Flask
- numpy
- scikit-learn
- matplotlib
- seaborn

# Installation

1. Clone this repository to your local machine:

   ```git clone https://github.com/your-username/car-color-classifier.git```

2. Navigate to the project directory:

   ```cd car-color-classifier```

3. Install the required dependencies using pip:

   ```pip install -r requirements.txt```

## Usage

1. Start the Flask application by running the following command:

   ```python app.py```

2. Open a web browser and go to `http://localhost:5000` to access the application's user interface.

# Uploading Images

- Click on the "Choose File" button to upload an image of a car.
- Supported image formats: PNG, JPG, JPEG.
- Click the "Submit" button to initiate the color prediction.

# Viewing Predictions

- After uploading an image, the model will display the predicted color of the car.
- The prediction will be displayed along with the prediction confidence level.
- If the confidence level is below a certain threshold, the color will be labeled as "unknown."

# Confusion Matrix

- Evaluates the model's performance on a provided test dataset located in the `test/` directory.
- It generates a confusion matrix to visualize how well the model predicts different colors.
- The confusion matrix heatmap illustrates predicted versus true color labels.

# F1 Score and Accuracy

- The F1 score and accuracy of the model on the test dataset are calculated.
- The F1 score is a measure of the model's precision and recall, weighted by class frequency.
- The accuracy is the ratio of correctly predicted instances to the total number of instances.

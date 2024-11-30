# Real-time Gender and Age Prediction from Webcam

## Project Description
This project uses deep learning models to predict the gender and age of a person in real-time from webcam images. The model analyzes the image from the webcam, predicts the gender (Male/Female), and estimates the age, then displays the prediction results live.

## Requirements
To run this application, you need to install the following libraries and tools:

1. **Python 3.6+**
2. **Python Libraries**:
   - `opencv-python`
   - `keras`
   - `numpy`
   - `matplotlib`

## Installation

### Install Required Libraries
First, install the required libraries using `pip`. You can do this in your terminal or command prompt.

```bash
pip install opencv-python keras numpy matplotlib
Download Models
This application requires two pre-trained deep learning models:

Gender Model (gender_model.h5): Predicts the gender of the person in the image.
Age Model (age_model.h5): Predicts the age of the person in the image.
Make sure to download these models and save them in the appropriate folder along with the project's source code.

Usage
Run the Application
To run the application, simply call the display_video() function in your code. The application will open your webcam and display the live predictions of gender and age.

python
Copy code
display_video()
The application will show the webcam feed and display predictions for gender and age directly on the screen. You can stop the application by closing the image display window or breaking the loop in the code.

How It Works
Preprocess Input Image: The image from the webcam is processed and converted to grayscale to fit the model's input requirements.
Gender Prediction: The gender model will classify the person in the image as "Male" or "Female."
Age Prediction: The age model will estimate the person's age.
Display Results: The results will be shown on the webcam feed and printed in the console.
Notes
The model requires a fixed-size input image. Therefore, the image is resized and normalized before being passed to the model.
This application works well in a local Python environment with access to a webcam. If running on Google Colab, additional modifications may be needed to capture webcam images (such as using eval_js to fetch webcam images from the browser).
Future Improvements
Optimize the model for faster predictions in an online environment.
Add features for emotion analysis and other facial characteristics.
Author
Author: Vũ Hoài Nam
Email: 20212501@eaut.edu.vn
GitHub: https://github.com/vunameaut
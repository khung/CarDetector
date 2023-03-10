# Car Detector with ML Kit

## Objective
The goal of this project was to demonstrate that it is possible to create an object detector running on a mobile device that can detect different car models. ML Kit and its image classification APIs were chosen for this task. Google's ML Kit Vision Quickstart Sample App was used as the platform:
https://github.com/googlesamples/mlkit/tree/master/android/vision-quickstart

## Steps
1. Train the full TensorFlow model using transfer learning in [mlkit_model_training.ipynb](mlkit_model_training.ipynb). See the notebook for more details.
2. Convert the model to TFLite in [mlkit_model_convert.ipynb](mlkit_model_convert.ipynb). See the notebook for more details.
3. Clone the vision-quickstart project.
4. Open the project in Android Studio.
5. Copy the TFLite model object_labeler.tflite to assets/custom_models.
6. Build the app and deploy to your device.

## Running the model
1. Launch the MLKit-Vision app on your device.
2. Tap on "Run the ML Kit quickstart written in Kotlin".
3. Tap on CameraXSourceDemoActivity.
4. Point the device's camera at a car (can be a real car, a picture, or a video). If the car model is in the training set, the car should be classified almost immediately.

## Results
### Detecting a car in a picture
Aero777, CC BY-SA 3.0 <https://creativecommons.org/licenses/by-sa/3.0>, via Wikimedia Commons
![DetectInPicture](https://user-images.githubusercontent.com/963577/224446666-8cfa6cb8-2b09-434c-9a9b-ad38116941ef.png)

### Detecting a car in a video
Video snippet is from Consumer Reports website: https://www.consumerreports.org/video/view/cars/auto-test-track/1875312648/hummer-h2-2008-2009-road-test/
https://user-images.githubusercontent.com/963577/224446778-fc307ba3-cc99-4799-b103-03a6b70637e1.mp4

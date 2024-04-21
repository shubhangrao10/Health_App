
<p align="center">

<img src= "https://github.com/Dantusaikamal/Healthify/blob/main/assets/images/healthify-logo-light.png" width="150px" />

</p>

<p align="center"> Healthify - Heart Stroke Prediction using Machine Learning and Fitness trackers </p>


Every 40 seconds, someone in the United States has a stroke. Every 3.5 minutes, someone dies of stroke. Every year, more than 795,000 people in the United States have a stroke. About 610,000 of these are first or new strokes. The chances of survival are greater when emergency treatment begins quickly. Moreover, up to 50% of all strokes are preventable. Hence, it is important to identify strokes in the early stages. 

This can be done using any ordinary fitness trackers that collect longitudinal data of heart rate and blood pressure levels in real-time which is connected to a Machine Learning model trained to identify and alert in case of a sudden extreme change in the parameters of heart rate levels.

In the proposed model, heart stroke prediction is performed on a dataset collected from my personal Mi band 4. Data from the fitness tracker is obtained in real-time by a get request from Mi Fit’s API endpoint. The continuous data is then used to feed the machine learning model which is hosted in Firebase.

The model predicts the chances a person will have stroke based on symptoms like age, gender, body mass index, work type, average heart rate, calories, steps, sleep patterns. It classifies the persons risk level by implementing various machine learning algorithms like Random Forest, Logistic Regression, K-Nearest Neighbor (KNN), Decision Tree. 

Thus, a comparative analysis is shown between the various algorithms and the most efficient one is obtained. Cardiovascular diseases are the leading cause of death globally, taking an estimated 17.9 million lives each year. With this project, We aim to save the lives of at least a percentage of those who might experience a heart stroke and alert them about the possible stroke.

## Our Solution: 

Heart stroke can have serious consequences, including heart failure, arrhythmias, and impaired cognitive function. Early detection and prevention of heart stroke is crucial in order to improve patient outcomes and quality of life. Traditional methods for identifying individuals at risk of heart stroke, such as blood tests and imaging studies, can be expensive, invasive, and often require specialized equipment and trained personnel. As a result, there is a need for more accessible and cost-effective methods
for identifying individuals at risk of heart stroke.

Fitness bands, which are wearable devices that track physical activity and other health-related metrics, have become increasingly popular in recent years. These devices generate a wealth of longitudinal data, including information about physical activity, heart rate, and sleep patterns. This data has the potential to provide valuable insights into an individual's overall health and risk of developing various diseases, including heart stroke.

In this proposed solution, we are detecting and alerting users of the risk of stroke using wearable technology, machine learning, and mobile application development.  We are utilizing MI Band 4 fitness tracker to collect longitudinal data of heart rate and blood pressure levels in real-time, which is then used to train a machine learning model to predict the chances of a person having a stroke based on symptoms such as age, gender, body mass index, work type, and continuous heart rate.

In this project, a machine learning model is deployed in an Amazon SageMaker instance to make predictions on new data in real-time. The Flutter mobile application serves as the user interface for the Heart Stroke detection system, alerting users of possible strokes based on the results of the machine learning model.

We aim to provide early detection and alerts for users who may be at risk of having a stroke. By providing timely alerts, users can seek emergency treatment quickly, which increases the chances of survival and recovery from a stroke.

The application is divided into different modules:

### 1. User Registration and Login: 
 
This module enables users to create their accounts and log in to the application securely. Users can also reset their passwords in case they forget them.

### 2 Home Screen: 

In the Home Screen module, user will be able to view their vitals. They can also edit or add new records of their vitals and can also get timely health alerts.

<p align="center">
<img src= "https://github.com/Dantusaikamal/Healthify/blob/main/assets/images/Healthify Home screen.png" width="400">
</p>

### 3. Predict Heart Stroke Risk: 

This module analyzes the input health data using the machine learning model and generates a prediction of the user's risk of having a heart stroke. The prediction is displayed on the screen along with a color-coded risk indicator.

<p align="center">
<img src= "https://github.com/Dantusaikamal/Healthify/blob/main/assets/images/Healthify Navigation screen.png" width="400">
</p>


### 4. SOS! (Emergency screen): 

Whenever the heartrate of a user is extremely high or low, they will receive a notification / pop-up screen asking if they are experiencing a stroke. If they click NO, they will be redirected to the Home screen which displays their high heart rate. But if they press YES (They are experiencing a stroke) or if they fail to press any key within 10 seconds, they will be redirected to SOS screen that will send an sms alert to user's emergenct contacts that contains user's location and a message. An alert will also be sent to nearby hospitals. 

<p align="center">
<img src= "https://github.com/Dantusaikamal/Healthify/blob/main/assets/images/Healthify SOS Screen.png" width="400">
</p>

### 5. View Previous Health Data: 

This module allows users to view their previous health data and predictions. Users can scroll through their history and compare their previous and current risk levels.

### 6. Language translation Module: 

This module enables users to use the application in their comfortable language.

### 7. Profile: 

This module allows users to customize the application's settings, such as the language, notification preferences, and user profile. Users can also log out of the application from this module.

<p align="center">
<img src= "https://github.com/Dantusaikamal/Healthify/blob/main/assets/images/Profile Screen Healthify.png" width="400">
</p>

### 8. Contact Medical Professionals: 

This module enables users to contact medical professionals in case they need urgent medical attention or have questions about their health. The application provides users with a list of nearby medical facilities and their contact information.

### 9 View Health Tips: 

This module provides users with helpful tips on how to maintain a healthy lifestyle and reduce their risk of having a heart stroke. The tips are displayed in a scrollable view and cover various topics, such as exercise, diet, and stress management.


### Technologies used:
- TensorFlow
- Flutter 
- Firebase
- Twilio
- Google Fit API
- Mi Band 4 (Hardware)









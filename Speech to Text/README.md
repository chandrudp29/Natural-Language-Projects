 # SPEECH to TEXT

## PROBLEM STAEMENT
In this project our goal is to acheive the problem of converting audio data into textual data.
DESCRIPTION OVERVIEW
Speech Recognition is an important feature in several applications used such as home automation, artificial intelligence, etc. This article aims to provide an introduction on how to make use of the SpeechRecognition library of Python. This is useful as it can be used on microcontrollers such as Raspberri Pis with the help of an external microphone.
Speech recognition technologies such as Alexa, Cortana, Google Assistant and Siri are changing the way people interact with their devices, homes, cars, and jobs. The technology allows us to talk to a computer or device that interprets what we’re saying in order to respond to our question or command.
Popular digital assistants, include:
•	Amazon’s Alexa
•	Apple’s Siri
•	Google’s Google Assistant
•	Microsoft’s Cortana

TECHNOLOGY USE
Here we will be using  Anaconda Python 3.6 and SpeechRecognition package.

## INSTALLATION
Installation of this project is pretty easy. Please do follow the following steps to create a virtual environment and then install the necessary packages in the following environment.

### In Pycharm it’s easy

1. Create a new project.
2. Navigate to the directory of the project
3. Select the option to create a new new virtual environment using conda with python3.6
4. Finally create the project using used resources.
5. After the project has been created, install the necessary packages from requirements.txt file using the command pip install -r requirements.txt



### In Conda also it’s easy

1. Create a new virtual environment using the command
    conda create -n your_env_name python=3.6
2. Navigate to the project directory.
3. Install the necessary packages from requirements.txt file using the command         
pip install -r requirements.txt

### WORKFLOW DIAGRAM

![](https://github.com/chandrudp29/Natural-Language-Projects/blob/master/Speech%20to%20Text/images/1.png)









### IMPLEMENTATION
#### 1. Project Directory

![](https://github.com/chandrudp29/Natural-Language-Projects/blob/master/Speech%20to%20Text/images/2.png)









This is the folder stucture of this project.
#### 2. requirements.txt
![](https://github.com/chandrudp29/Natural-Language-Projects/blob/master/Speech%20to%20Text/images/3.png)


This file contains the necessary package called SpeechRecognition


#### 3. speechToText.py
![](https://github.com/chandrudp29/Natural-Language-Projects/blob/master/Speech%20to%20Text/images/4.png)

This file contains the script to convert the speech to text using SpeechRecognition package.
#### 4. clientApp.py
![](https://github.com/chandrudp29/Natural-Language-Projects/blob/master/Speech%20to%20Text/images/5.png)








This this is the flask server file and entry point of your application.
TESTING IN LOCAL/API
To run this project in your local system just run the file clientApp.py and after that web server will start at http://0.0.0.0:5000/

Browse and Upload the .wav file and click on Predict button.
Finally you will get the decoded text in the Results box.

## CONCLUSION
Hence we have successfully converted audio data or speech to digital text data.
COMPARISION
Here we can improve the results by testing with other APIs which are available from diffrent third party sources or by applying deep learning approaches.


### See(k) Help - IBM Crack The Covid-19 Crisis
<img src ="media/VideoTitle.jpg"> 

### A Brief Overview
The COVID-19 Pandemic was one of the biggest global health calamities of the century. The virus rapidly spread around the world, posing enormous health, economic, environmental, social challenges to the entire human population, while also severely disrupting the global economy.  

While talking about the problems faced by the world population, we often forget to consider the ones that are the most affected by the current situation, the blind and the visually impaired. The World Health Organization estimates that there are over **2.2 Billion people with some form of visual impairment.** In most countries, blind people are not classified as ‘clinically extremely vulnerable’ and are automatically not entitled to food parcels, priority supermarket deliveries or help with basic care needs.  

•	Braille readers need to touch packets to read labels. These techniques maintain independence in normal times. Now, though, many visually impaired people are concerned by **having to touch multiple items**, moving them closer to their eyes, and spending longer in a potentially virus-laden environment. The tactile sense which plays a vital role in their livelihood is being challenged by the virus.  

•	Supermarkets usually allow a staff member to accompany a visually impaired person around the shop. Now, though, this would mean **spending more time in close contact with a potential asymptomatic carrier**.  

•	At home, people who can’t see well and live alone face challenges in reading use-by dates, checking cooking instructions on a food packet, or making sure they’re taking the right dose of medication.  

Our aim and objectives are to provide help for the visually impaired community by means of an app. We’ve created an application designed to help the blind and visually impaired identify objects they encounter in their daily lives. **Simply take a photo of anything, at any angle and you’ll hear the app identify and speak back the scene in front of you!** 

### Description
See(k) Help is an application intricately designed for the blind and the visually impaired. Be it a phone, tablet or a PC, our app utilizes the device’s camera and text-to-speech functionalities to take a picture of anything that the user points at, generate a caption of the objects in the picture and read it out loud, in the language of the user’s choice.   

Included in the solution is a **self-trained Image Captioning Model**. The dataset used to train the model is the Flickr30k Dataset. 
The model includes an **Inception-based CNN** to identify the objects in the frame and an **LSTM Neural Network** to generate the caption. We also use a language model, **GloVe Embeddings** to generate the caption with the correct Semantics. This ensures the result would be easily decipherable by the user, and not just a set of objects.   

A **web framework built with Flask** is used to link the API to the trained model which perceives the images and captions it. The result is sent to IBM’s Cloud based Text-To-Speech service which converts the generated caption to natural sounding audio, which is then played to the user. The inclusion of the IBM Language Translation service allows us to convert the generated caption which is in English to other languages, and then using the Text-To-Speech service, we can play the translated caption to the user.  

### Rationale
#### Flexibility
An easy to use app right at the tip of our fingers with a user-friendly interface especially designed for the blind along with Flask, which is a best in class framework. Since applications have become a major part of the digital landscape, our app is performance driven with the use of best technologies that provides maximum flexibility for all its users.

#### The Current Crisis
In the current times with the persistent crisis and with all the problems faced by the blind community, this app serves as a perfect companion to help them and guide them without any need of human intervention. This app also provides them with a sense of safety and security in these hard times.

#### Evolution in Technology
Machine learning along with Artificial Intelligence is redefining our future and with the evolution of current training algorithms, we can improve the prediction rate and accuracy over time and thus build upon the existing functions to provide additional features to assist the blind.

#### Inclusivity
See(k) Help is built on the principle of inclusivity. By failing to consider the needs of those different to ourselves, we will not be able to create a welcoming platform for everyone. After analysing the key issues at the intersection, we aim to promote and develop accessible technologies for all our users across platforms.  

### Architecture Diagram
![Architecture Diagram](media/Arch2.jpg)

### Screenshots
![Simple Layout For Easy Access](media/Screenshot%20(159).png) 
<p align="center">Simple Layout For Easy Access</p>  

<img src ="media/Screenshot (161).png">
<p align="center">Available Languages</p>  

### Video Demo  
[![Watch the Demo](https://img.youtube.com/vi/P_XU4UL041Y/maxresdefault.jpg)](https://www.youtube.com/watch?v=P_XU4UL041Y)     

### Steps to Run the Project:
```
Install dependencies mentioned in requirements.txt
pip install -r requirements.txt
```

1. Download both 'inception' and 'prediction.h5' from [here](https://drive.google.com/drive/folders/1xSfaPYT7tZAN9sQZovjkeVF8jvLzmOSo)   and place them in 'models' directory.
2. Open homex.html (located in the 'run' folder) in a browser.
3. Open the text files located in 'api' folder and enter the required api keys and urls for the IBM services. Note : API keys are already included but suggested to be changed by the user during the time of running the project.
4. Run test_req.py and wait for it to deploy
5. Choose language of choice and the image to be checked.
6. After clicking on 'listen' wait for 5-10 seconds for the audio to play on the webpage.

### Model
All training files has been included in the 'models_to_train' folder, with inspiration from [Harshall Lamba](https://github.com/hlamba28/Automatic-Image-Captioning/blob/master/Automatic%20Image%20Captioning.ipynb)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

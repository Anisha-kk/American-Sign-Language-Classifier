# American-Sign-Language-Classifier
## Overview
This project trains a ML model to identify alphabets of American Sign Language (ASL) from images. This ia a multi class image classification problem. The Convolutional Neural Network (CNN) model created achieved an accuracy score of ~90% in identifying the alphabets, which is fairly good.
## Problem understanding
Sign language is a visual language expressed through physical movements instead of spoken words. The language relies on visible cues from hands, eyes, facial expressions, and movements to communicate. American Sign Language (ASL) is expressed by movements of the hands and face. It is the primary language of many North Americans who are hard of hearing and is used by some hearing people as well. The image below shows the alphabets of ASL:
![american_sign_language](https://github.com/user-attachments/assets/1f1d1b9d-71fa-4dad-8252-7d4ae63db593)

The alphabets J and Z require hand movement.

Many people do not know sign language. **The ultimate aim of this project is to help such people decode the ASL sign and thereby understand what the person using ASL is communicating.**
## Data Understanding
Source: https://www.kaggle.com/datasets/datamunge/sign-language-mnist

The Sign Language MNIST is an American Sign Language letter database of hand gestures with 24 classes of letters (excluding J and Z which require motion).
Each training and test case represents a label (0-25) as a one-to-one map for each alphabetic letter A-Z (and no cases for 9=J or 25=Z because of gesture motions). The training data (27,455 cases) and test data (7172 cases) contains a header row of label, pixel1,pixel2….pixel784 which represent a single 28x28 pixel image with grayscale values between 0-255. 
## Result and Evaluation
Both Random Forest Classifier and Convolutional Neural Network (CNN) were used to train the multi class classifier. The performance of CNN is found to be much better than that of Random Forest Classifier.The CNN classifier classified the test images with an accuracy score of ~90%, which is ~10% higher than the accuracy score of Random Forest classifier.
## Future Scope
A lot of improvements can be done to this project. Some of them are as follows:<br>
1. Perform identification from videos - this will enable inclusion of letters J and Z as well. Also, it can be used to decode words instead of letters which enables proper communication <br>
2. Real time ASL recognition: Create a text to speech translator that captures the sign language video convert the letters or words to speech in real time so as to improve communication. 

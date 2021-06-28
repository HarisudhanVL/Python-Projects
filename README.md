Ticket Dispensation Using Face Detection and Classification.

Introduction:

In most parts of the world, tickets at the entry section in parks, tourist spots, theme parks, etc… are distributed manually. In this computer world, the tickets aren't to be issued manually. The ticket fare also differs with age group they belong. Generally age is categorized into three groups.

1. 0 - 3 years old (baby)
2. 3 - 13 years old (child)
3. 13 and above years old (adulescent / adult)

Objective:

So this project introduces an approach to automatically distribute tickets to customers by face detection and classification. Dispensation is done by detecting the face of the people at the ticket counter and classifying them into above mentioned categories to issue tickets. Face detection and classification methods depend on certain features within the face. The machine learning algorithms used are, a pre-trained model for face detection and MobileNetV2 for classification. The dataset has been manually collected, which has the images of people residing in different parts of Tamil Nadu, India under various age groups.

Ticket Dispensation - I: 
Here the Data is collected, augmented and preprocessed. The preprocessed data is fed into the machine learning model (MobileNetV2) and model is trained. While training the model, the weights and the parameters after updation are saved in a file name "model.h5", which can be used to predict on new data. The model is evaluated by its performance using performance metrics such as accuracy, precision, recall, f1-score and confusion matrix. And finaly the test images are given to the model for predicting the class and hence you can refer the code and the outputs in the repository folder "Ticket Dispensation - I".

Ticket Dispensation - II:
The trained and saved model is loaded. In ticket dispensation - I the test images are preprocessed and given to the model for prediction, but here the images are captured in live using webcam i.e, video capturing using webcam to capture the picture of the person who is inneed of ticket. The captured image is processed and region of interest (face) is detected using face detection caffe deep learning frame work and cropped using OpenCV. Now the detected face is given to the model for predicting class.

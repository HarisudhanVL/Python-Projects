Ticket Dispensation Using Face Detection and Classification.

Introduction:

In most parts of the world, tickets at the entry section in parks, tourist spots, theme parks, etc… are distributed manually. In this computer world, the tickets aren't to be issued manually. The ticket fare also differs with age group they belong. Generally age is categorized into three groups.

1. 0 - 3 years old (baby)
2. 3 - 13 years old (child)
3. 13 and above years old (adulescent / adult)

Objective:

So this project introduces an approach to automatically distribute tickets to customers by face detection and classification. Dispensation is done by detecting the face of the people at the ticket counter and classifying them into above mentioned categories to issue tickets. Face detection and classification methods depend on certain features within the face. The machine learning algorithms used are, a pre-trained model named Haar Cascade Classifier for face detection and MobileNetV2 for classification. The dataset has been manually collected, which has the images of people residing in different parts of Tamil Nadu, India under various age groups.

The MovileNetV2 model in Ticket Dispensation - I is saved as "model.h5" file. Which is used for prediction on new data. Each time training the model takes long time. So save the model and just load it for prediction which is faster.

Input:

Video capturing using webcam to capture the picture of the persons who is inneed of tickets. The captured image has multiple faces(group of people), so all the faces present in the captured images are detected and extracted using Haar Cascade Classifier. Then the detected faces are preprocessed.

Output:

The Preprocessed image is fed to the model to classify the detected face into above mentioned categories using the saved model "model.h5".
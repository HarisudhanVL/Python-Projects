Ticket Dispensation Using Face Detection and Classification.

Introduction:

In most parts of the world, tickets at the entry section in parks, tourist spots, theme parks, etc… are distributed manually. In this computer world, the tickets aren't to be issued manually. The ticket fare also differs with age group they belong. Generally age is categorized into three groups.

1. 0 - 3 years old (baby)
2. 3 - 13 years old (child)
3. 13 and above years old (adulescent / adult)

Objective:

So this project introduces an approach to automatically distribute tickets to customers by face detection and classification. Dispensation is done by detecting the face of the people at the ticket counter and classifying them into above mentioned categories to issue tickets. Face detection and classification methods depend on certain features within the face. The machine learning algorithms used are, a pre-trained model named Haar feature-based cascade classifier for face detection and MobileNetV2 for classification. The dataset has been manually collected, which has the images of people residing in different parts of Tamil Nadu, India under various age groups.

Input to the model:

The image of the person, face(ROI - region of interest) is alone detected and copped from the image, given to the model for prediction of class.

Output to the model:

Predicted a class for the input image from the above mentioned three categories. 



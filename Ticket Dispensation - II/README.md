Ticket Dispensation Using Face Detection and Classification.

Introduction:

In most parts of the world, tickets at the entry section in parks, tourist spots, theme parks, etc… are distributed manually. In this computer world, the tickets aren't to be issued manually. The ticket fare also differs with age group they belong. Generally age is categorized into three groups.

1. 0 - 3 years old (baby)
2. 3 - 13 years old (child)
3. 13 and above years old (adulescent / adult)

Objective:

So this project introduces an approach to automatically distribute tickets to customers by face detection and classification. Dispensation is done by detecting the face of the people at the ticket counter and classifying them into above mentioned categories to issue tickets. Face detection and classification methods depend on certain features within the face. The machine learning algorithms used are, a pre-trained model caffe deep learning framework(attached in the repository Ticket Dispensation -II) for face detection and MobileNetV2 for classification. The dataset has been manually collected, which has the images of people residing in different parts of Tamil Nadu, India under various age groups.

The MovileNetV2 model in Ticket Dispensation - I is saved as "model.h5" file. Which is used for prediction on new data. Each time training the model takes long time. So save the model and just load it for prediction which is faster.

Input:

Video capturing using webcam to capture the picture of the person who is inneed of ticket. The captured image is processed and region of interest (face) is detected using face detection caffe deep learning frame work and cropped using OpenCV.

Output:

The Preprocessed image is fed to the model to classify the captured image into above mentioned categories using the saved model "model.h5".
*******************************************************************************************************************************************************************************

Files in Ticket Dispensation direcory.
1. MobileNetV2_video_capture - Has the coding and output.

3,4. deploy.prototxt and res10_300x300_ssd_iter_140000.caffemodel are the caffe deep learning framework used for face detection from an image.

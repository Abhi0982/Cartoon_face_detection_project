Cartoon-Face-Detection-and-Recognition 

The project maintains the following directories:

preprocessing - contains the files for parsing the XML files to filter the images based on the attributes required by the sub-tasks of the project (i.e., class-wise, gender-wise, facial posture wise manners).

landmark_extractor - contains the code for managing the 15 facial landmarks extraction, arranging these to the format compatible of being merged with the Kaggle instances and training the 5 layer LeNet architecture for landmark extraction. The output csv is further used in the character and gender recognition of the cartoon faces.

datasets hosts two files:

train_own.csv is the output of running append_pixels_new.py on onlyLandmarks.csv, that contains comma separated landmark coordinates manually extracted using LandmarkManuallyGetter.jar.
face_detection contains the code for running the MTCNN, Haar and HOG based models.

face_recognition contains the code for the character recognition of the cartoons based on the Inception v3+SVM and the proposed HCNN model.

gender_recognition contains the code for the character recognition of the cartoons based on the Inception v3+SVM and the proposed HCNN model.

outputs contains the accuracy and top-5 error rate graphs for the character recognition problem, the model architectures used as well as the results of the face detection models.

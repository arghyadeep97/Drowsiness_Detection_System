# Drowsiness_Detection_System
The main goal of this project is to detect the eye of a patient and count the blinking frequency of the eye to satisfy their need if any. At the elementary process, we detect the face of the patient and predict the shape of the face using the Dlib module after having video frames using the imutils module through camera, which was assigned to monitor the patient all the time. Other than this we will need a facial key points detector that can detect eyes in real-time. For this we will use a pre-trained network in the dlib library which can detect ’68 key points’ that is presented in this paper. The required pre-trained model can be downloaded from the internet. The dlib is used because it can give predictions in real-time.
The eye aspect ratio which is calculated after eye detection, will inspect the eye's present state i.e., open or close. In case of the value of EAR is greater than the predefined threshold, then we assume patient's that winking. This process is followed by the process of counting the frequency of the eye blinking. If the count value matches with the given threshold value, we would end with a prompting message.

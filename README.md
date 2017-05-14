# FCP-Codes
This is my final course project codes. It's a project that I have done in my undergraduate Electrical Engineering degree, where I classify face expressions using machine learning.

-frames:
This notebook processes videos in a given directory. First it extract the frames of the video (29.97 frames per second) then it creates 2 folders, called FramesSemLandmark and FramesComLandmark. In the first one it saves the raw frames. In the second one it saves the frames with the 67 landmakrs (points of interest) in the face. After processing the video, it gets all the landmarks positions in the face, saving them in a csv file in the order (x1,y1,x2,y2,...) where (x1,y1) represent the landmarks coordenate in the first frame. After this step, it calculates the mean and the variance of all the landmarks, and label them from 1 to 22 according with the expressions itself, saving it in the FinalData.csv.

-Training:
This notebook processes the DinalData.csv. It creates some classifier (SVM with linear kernel) and after that it trains this classifier and test it in the test set created in the train_test_split function with 30% of the data in the test set. More classifiers will be added later.

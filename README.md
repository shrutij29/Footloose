# Footloose

**Project:** Footloose

**Summary:**
A Machine Learning project to classify dance images to a particular dance style category.

**Contributors:** Blake Bleier, Danny Nguyen, Summer McGrogan, Shruti Jain  
Each member in this group has components of EDA, Model creation, and exploration for our project in their respective branches, 
so please be sure to take a look at all the four branches in addition to our main.

**Dataset:**
https://sites.cc.gatech.edu/cpl/projects/dance/
- Original frames
- Optical flow
- Skeletal (visual & JSON)
For the purpose of our project we primarily utilized the JSON skeletal images and further experimented a bit with the 
original frames & skeletal visual data.

**Key Models:**

- **sjain/EDA/Baseline_Model.ipynb**: basic RF model that ran on data split on images, rather than videos.
- **summer/RF_Model_3.ipynb**: Part 1: basic 3-class RF model split on videos; Part 2: Latin and Ballet model split on videos 
- **summer/RF_Model_Ballet_Tap.ipynb**: ballet and tap RF using gridsearch, randomizedsearch, and boosting split on videos
- **summer/RF_Model_Swing_Latin.ipynb**: swing and latin RF model using gridsearch, randomizedsearch, and boosting split on videos
- **blake_branch/Multiple_Models.ipynb**: neural net and k-nearest neighbor models on ballet/latin/tap. Dataviz of incorrectly assigned skeletal info
- **sjain/EDA/Temporal_Model_Shruti.ipynb**: temporal data filtration, creation of new feature matrix, running this temporal data through RF models
- **blake_branch/NN_Model_on_Videos.ipynb**: temporal data filtration, creation of new feature matrix, running this temporal data through NN models
- **blake_branch/Normalized_Features.ipynb**: logic to normalize & scale features - bounding box method & hip distance method
- **danny/eda_danny**: function to compare current frame to previous frame to check and see if the person is at the same location
- **danny/EDA_img_danny**: RF model on raw images. altered and filtered images to feed into model. ran 2 test with different n_estimators with confusion matrix.
- **danny/EDA_skeletal_danny**: RF model on skeletal images. altered and filtered images to feed into model. ran 2 test with different n_estimators with confusion matrix.

**Final Presentation:**
You can navigate to our final_presentation.pdf to see our slide deck.

# InvasiveID-Model
Calssify three species of invasive plants in BC Canada using images

Link to data repostiory on google drive:
https://drive.google.com/drive/folders/1980dS2LkyXQtOTu9JKQBdEz-xdg9kQbI?usp=sharing

Includes the following files: 
* final_BC_images_raw.zip
	* Contains the images after being collected via FlickrPicCollector.ipynb and picked over manually. 
* final_BC_images-balanced.zip
	* Contains the output images after DataLoader.ipynb.
	* 400 files were manually deleted from train/class_2 and 60 from train/class_1 to balance the classes.

Notebook files: 
* FlickrPicCollector.ipynb
	* Runs 1st.
	* This is the implementation of the FlickrAPI.
 	* Searches flickr based on a dictionary named plants.

* DataLoader.ipynb
	* Runs 2nd.
	* Moves, shuffles, splits images into test and train sets.
	* Creates dataframes test and train and saves to csv.

* Keras_TFlow_Model_SageMaker.ipynb
	* Runs 3rd.
	* Includes the Keras VGG16 transfer learning model.
	* Directory structure of sourcing data is a bit different due to SageMaker.

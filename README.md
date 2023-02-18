# Canola-Disease-Detection

This is my final project for ENSE 489 Ethics of Artificial Intelligence at the U of R. It is a system that differentiates between healthy canola stems and ones infected with Sclerotinia stem rot. In the future I want to add more data, more diseases, and more usability, but we were only given 3 weeks to do this project so this was my prototype. 

The dataset is stored at https://www.kaggle.com/datasets/gregsvein55/canola-diseases and if you run the code in Google Colab, you should be able to just download the testing and training folders directly into your Google Drive and have it run no problem. Just run the .ipynb file and all other folders will be automatically created. Changes will need to be made to the filepaths if taken outside of Google Colab. 

The system works using a Convolutional Neural Network using the basic structure of Convolation -> Pooling -> Convolation -> Pooling -> Fully Connected Layer -> Output.
I did a 70/30 validation split, so 70% of the data was training and 30% was testing. The max I was able to get in all my testing was around 90% validation accuracy, which is acceptable for my prototype, althought it would need a lot more images and diversity training to ever be a fully functioning system. 

# Train it yourself
## Step 1
Download canola_disease.ipynb and then upload it to your Google Drive with Collabatory
## Step 2
Download the dataset from https://www.kaggle.com/datasets/gregsvein55/canola-diseases and upload the individual testing and training folders to your google drive.
## Step 3
Go into Collabatory and mount your Google Drive to get access to these folders. 
## Step 4
Go to the top and selct run all, for the model I have 8 epochs, if your computer is running slow it could probably still work well with a minimum of 5 epochs. My computer took around 2 minutes to run the whole thing.
## Step 5
You should see the final epoch run with 85-90% val_accuracy, and the 4 test photos should be Healthy, Healthy, Diseased, Diseased. If this doesn't happen run the model again because something went wrong. 
## Step 6
From here you can add any pictures you want to the testing files and just copy the code in the last code module and replace the name of the picture to test whatever you want. Just keep in mind that all the pictures will be shrunk to 125x125 pixels and greyscaled so for the best results use pictures that clearly show the canola stem with minimal background noise.



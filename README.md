# Canola-Disease-Detection

This is my final project for ENSE 489 Ethics of Artificial Intelligence at the U of R. It is a system that differentiates between healthy canola stems and ones infected with Sclerotinia stem rot. In the future I want to add more data, more diseases, and more usability, but we were only given 3 weeks to do this project so this was my prototype. 

The dataset is stored at https://www.kaggle.com/datasets/gregsvein55/canola-diseases and if you run the code in Google Colab, you should be able to just download the testing and training folders directly into your Google Drive and have it run no problem. Changes will need to be made to the filepaths if taken outside of Google Colab. 

The system works using a Convolutional Neural Network using the basic structure of Convolation -> Pooling -> Convolation -> Pooling -> Fully Connected Layer -> Output.
I did a 70/30 validation split, so 70% of the data was training and 30% was testing. The max I was able to get in all my testing was around 90% validation accuracy, which is acceptable for my prototype, althought it would need a lot more images and diversity training to ever be a fully functioning system. 




# oldpage

we used three different models to calculate our final predictions for our images
them being:
1. knn model for digits
2. lstm model from tesseract dataset for all alphanumeric
3. firebase ml kit (text recognition) model integrated into android studio

all these three models have been consolidated into one within android studio and using firebase ml kit features to provide the best possible output for a particular image.

our android app is built on java.

to run our application, you need to build gradle of all the files uploaded to the drive.
this should preferably be done on android studio upon integration with a separate project on our firebase console. failing to integrate the firebase client via a new project on the console will lead to errors in the code and the machine learning and text recognition aspect of the code not being able to run properly.

to run the lstm code, you need to initialize a folder for your images to be scanned.
post which you can run your code from the beginning. 
some dependencies like the tesseract files as well as opencv must be installed prior to running this code.
once the path of the images folder is mentioned in the code, the list of items in the folder is made into an array and the image to be scanned can be mentioned by mentioning the index of the element in the array.
multiple languages are supported by this model and the language to detect for can be mentioned by mentioning its 3 letter language code in the file.
other changes to the detection can be made and they are all mentioned in the ipynb file with appropriate comments to run them.

the knn file is pretty simple and some dependencies need to be installed prior to running this file of code.
matplotlib and sklearn need to be installed post which the code can be run.
sklearn dataset is pulled and the model is trained on that.
prediction of digits is done on this model with over 2000 datapoints.

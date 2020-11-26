# Chemical-Compund-Classificattion
The given dataset contains details about organic chemical compounds including their chemical features, isomeric conformation, names and the classes in which they are classified. The compounds are classified as either ‘Musk’ or ‘Non-Musk’ compounds. 

In this project we are given csv data file classificatiom.Which can be solved through several machine learing algoriths such as svm,decision tree,naive bayes,KNN,SGD etc.Here we use deep learing technique for binary classification.Here we are given classes as 0 and 1.So we use sigmoid function in final layer as there are only 2 classes.First We upload the dataset from the drive.Then we select feature and label column and remove the molucular names cause they dont give much to the molecular sturcture.We could have used Word embedding on molecular name but they have musk and non musk in them so this not proper way of classification.So after splitting the data into training and validation set into 80:20 ratio.We check for any missing data in the dataframe.Afte we do data normalization so the data is in same range of values.After we create the model using squential layer and adding dense layers.We add some dropout so there is no less chance for overfitting on data.We use rmsprop optimizer for back propagation and select binary crossentropy as a loss function.Then we select accuracy matrics.After training the data for 50 epochs and batch size of 10 we get accuracy of 97% on validation set.Then we plot the accuracy and loss for training and validation data using matplotlib library.After we get classification report such as f1 score,recall etc.Then we can download the h5 model is a pretrained model which can be used later for transfer learning or getting the output without training.

Assignment 3
Model to translate English sentences to Hinglish sentences

It is a juypter notebook you can just copy it to Google Collaboratory and execute it there or install the necessary libraries which are imported at the start of the file.

The data set is also attached.
Note - before running the code ensure that you modify the link of the CSV file according to your environment.

How I approached this problem.
1. Gathered a dataset that includes sentences and their corresponding translations in Hinglish.
2. Preprocessed the data making sure to remove any elements. Then I split it into training and validation sets.
3. The model I designed follows an encoder-decoder structure.
4. The encoder handles the sentences while the decoder generates the sentences.
5. To tokenize the input and output sentences I utilized the TextVectorization layer from TensorFlow/Keras.
6. Created tokenizers for Hinglish sentences customizing them based on the training data to establish vocabularies.
7. To train the model effectively I compiled it with an optimizer (in this case 'Adam') a loss function ('sparse_categorical_crossentropy') and evaluation metrics.
8. Using training data, for both Hinglish sentences, I proceeded to train the model for a specific number of epochs.
9. I have developed an inference model that generates translations, for English sentences. This model includes encoding and decoding components utilizing the weights obtained from the training model.
10. I have created a translation function that enables the conversion of sentences, into Hinglish using the inference model. This function predicts words sequentially taking into account generated words and initial states.

Result
The accuracy I was hoping for was not achieved, I tried different combinations of hyperparameters but due to limited resources, I was not able to train the model for more data.
If we try to train the model with more data then it may give better results.
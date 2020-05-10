# Movie-Review-Sentimental-Analysis-Using-RNN-and-LSTM

CONTRIBUTING MEMBERS - 

18BCE091 - Kaushil Mangaroliya

18BCE103 - Maharsh Shah

18BCE121 - Mitt Shah

This is a full guide and explaination of the the project named Movie Review Sentimental Analysis . 

Sentimental Analysis has always been one of the most worked upon section of Deep Learning . We has humans can understand the feelings and context behind any review someone gives us but for a machine to do the same just like human is very tough . To achieve this goal we have been using Deep Learning as our tool . 

Deep Learning with artificial neural network can act as one of the best solution when it comes to training upon descrete data or a dataset with distinct features which are unrelated to other, but when it comes to feeding a sentence or a phrase to the model doesnt make any sence and is not at all efficient. In traditional neural networks, all the inputs and outputs are independent of each other, but in cases like when it is required to predict the next word of a sentence, the previous words are required and hence there is a need to remember the previous words. 

So we need to overcome this problem as well and can be easily done by using RNN and using LSTM . Recurrent Neural Network(RNN) are a type of Neural Network where the output from previous step are fed as input to the current step. RNN came into existence and solved this issue with the help of a Hidden Layer. The main and most important feature of RNN is Hidden state, which remembers some information about a sequence. Long Short-Term Memory (LSTM) networks are a type of recurrent neural network capable of learning order dependence in sequence prediction problems. Unlike standard feedforward neural networks, LSTM has feedback connections. It can not only process single data points (such as images), but also entire sequences of data (such as speech or video) .

Neural Network Architecture Explained :-
It is a sequential model containg 1 input layer 4 hidden layer and 1 output layer .
Layer 1 - it is an embedding layer with 300 input neurons in it 
Layer 2 - it is LSTM layer implementation with 128 neurons in it and dropout of 0.5
Layer 3 - it is LSTM layer implementation with 64 neurons in it and dropout of 0.5
Layer 4 - it is simple dense layer with 100 neurons in it
Layer 5 - it includes dropout so as to make our model more efficient
Layer 6 - Output layer with 5 outputs ranging from 0 to 4 

Our output is an integer for every review, that integer defines its sentiment

0 - Negative

1 - Somewhat Negative

2 - Neutral

3 - Somewhat Positive

4 - Positive

# How to run this implementation ?

## NOTE - COMPULSARY RUN THIS IMPLEMENTATION IN GOOGLE COLAB WITH GPU SUPPORT ONLY . IF YOU TRY TO RUN THIS ON YOUR DEVICE OR WITHOUT GPU IT WILL TAKE A LOT OF TIME TO BE TRAINED. SO DONT EVEN TRY TO RUN IT ON CPU, USE GOOGLE COLAB GPU SUPPORT ONLY .

To run it with Google Colab GPU support on top left go to Edit > Notebook Settings > Hardware Accelerator > GPU


Firstly you need to download the training and testing dataset ( train.tsv and test.tsv ) from the Repository or just Download the whole repositiry , any of the moethod will work !
Datasets are very very large and will take some time to download, so be patient .

Secondly you need to have all the libraries needed to implement, list of the libraries :

1). Numpy

2). Pandas

3). NLTK ( For Natural Language and Deep Learning )

4). BeautifulSoup ( For pre-processing data )

5). Keras ( For implementing Deep Learning Architecture )

6). Sklearn ( To handle training and testing Dataset and other subordinate tasks )

7). Google ( colab ,files to upload your datasets to colab , without this you wont be able to access datasets )
 
FINALLY - Run the cells 

You will be asked to upload the datasets to the colab environment, so choose the train.tsv and test.tsv dataset files one by one from your device where you have downloaded it . For example if they are in c drive choose from C drive train.tsv file and press upload button

After uploading datasets, run all cells and you are good to leave it for training !

NOTE - IF YOU STILL FEEL THAT IT WILL TAKE MORE THAN HALF HOUR TO TRAIN THEN PLEASE REDUCE THE TRAINING DATASET TO HALF OF ITS INITIAL SIZE AND SAME FOR TESTING IF YOU WANT TO . IT WILL TAKE 90 TO 120 SECONDS FOR EVERY EPOCH TO TRAIN (total 6 epochs) SO IT WILL HARDLY TAKE MUCH OF TIME WITH GPU , BUT IF YOU STILL FEEL REDUCE DATASETS BY HALF .


BINGO ! YOU HAVE SUCCESSFULLY RUN THE IMPLEMENTATION! RUNTIME TOOK TIME BUT IF WAS WORTH EVERY EPOCH AND EVERY BATCH IF LEARNED THROUGH!











# audioset_sound_classification
Exploring sound classification using Google's Audioset dataset for Product Studio at Cornell Tech - Fall 2021. 

We downloaded data from Google's Audioset using [aoifemcdonagh's public GitHub repo](https://github.com/aoifemcdonagh/audioset-processing). 

We chose 8 classes of data from Audioset that we felt were typical of daily life in NYC: 
0 : screaming
1 : Subway, metro, underground
2 : speech
3 : Outside, rural or natural
4 : Traffic noise, roadway noise
5 : Inside, small room
6 : Outside, urban or manmade
7 : singing

We created a simple convolutional neural network (CNN) using the Python library Keras. We supplied this model with mel spectrograms. We processed our original sound data using the Python library librosa's functions to convert .WAV files into mel spectrograms. 

Our final metrics for our model's classes are as below: 
| Class | Precision | Recall | f1-score |
| ----------- | ----------- | ----------- | ----------- |
| 0 - Screaming   |  0.27    | 0.46      | 0.34       |
| 1 - Subway, metro, underground   |  0.44    | 0.70      | 0.54       |
| 2 - Speech   |  0.18    | 0.23      | 0.21       |
| 3 - Outside, rural or natural   |  0.60    | 0.10      | 0.17       |
| 4 - Traffic noise, roadway noise   |  0.44    | 0.50      | 0.47       |
| 5 - Inside, small room   |  0.28    | 0.31      | 0.29       |
| 6 - Outside, urban or manmade   |  0.24    | 0.12      | 0.16       |
| 7 - Singing   |  0.47    | 0.29      | 0.26       |

Our overall average accuracy was 0.33. 

# Intro
This dataset contains 8732 labeled sound excerpts (<=4s) of urban sounds from 10 classes: air_conditioner, car_horn, children_playing, dog_bark, drilling, enginge_idling, gun_shot, jackhammer, siren, and street_music. The classes are drawn from the urban sound taxonomy. For a detailed description of the dataset and how it was compiled please refer to our paper. All excerpts are taken from field recordings uploaded to www.freesound.org. The files are pre-sorted into ten folds (folders named fold1-fold10) to help in the reproduction of and comparison with the automatic classification results reported in the article above.

In addition to the sound excerpts, a CSV file containing metadata about each excerpt is also provided.
Dataset link - https://www.kaggle.com/chrisfilo/urbansound8k

# Methodology
1.There are 3 basic methods to extract features from audio file : a) Using the mffcs data of the audio files b) Using a spectogram image of the audio and then converting the same to data points (As is done for images). This is easily done using mel_spectogram function of Librosa c) Combining both features to build a better model. (Requires a lot of time to read and extract data).
2.I have chosen to use the second method.
3.The labels have been converted to categorical data for classification.
4.CNN has been used as the primary layer to classify data.

# Music-MNIST-Dataset

A simple audio-visual dataset consiting of sheet music images of single notes and short audio files of these notes being played on a range of pianos. Each audio file also has a noisy variation to help train more robust models. 

### Current status
+ 88 sheet music images
+ 1,948 training audio files
+ 516 testing audio files

### Dimensions
+ The sheet music images are 162x300 (heightxwidth)
+ In the Mel spectrogram representation of our audio files there are 764 frames

### Naming convention
{note name}_ {instrument}_ {augmentation (if applicable)}

### Annotation files
The dataset comes with 3 different annotation files. There is a train annotations file and test a annotations file should you want to use a separate dataloader for each set. Alternatively there is an annotations file which combines both. These annotation files also provide a template should you want to expand the dataset with new audio files to help facilitate your work. These annotation files can also be used to alter the test and train split but remember to move the audio files the correct folder depending on what set you assign them to in the annotations file.

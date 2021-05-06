# VAD_MIKO.2

dataset https://urbansounddataset.weebly.com/urbansound8k.html (this dataset include 9 differet voice and in .wav format)

If we use this approch for solving voice or not voice problem we can get a good accuracy

# EDA
- use librosa library for load ,normalise and keep only one channel i.e mono
- matplotlib to visualize the sound wave

# Feature Extraction
Here we will be using Mel-Frequency Cepstral Coefficients(MFCC) from the audio samples. The MFCC summarises the frequency distribution across the window size, so it is possible to analyse both the frequency and time characteristics of the sound. These audio representations will allow us to identify features for classification.

# Model
- Use 3 layer ANN to classify the sound , 
- Add relu activation function for 3 layers to overcome the vanishing gradient problem and Softmax function at o/p layer to classify the sound coz it is multiclass 
- Add dropout ratio to overcomethe overfitting model
- upto 100 epoches and batch size 32
- Accuract 80% 
 

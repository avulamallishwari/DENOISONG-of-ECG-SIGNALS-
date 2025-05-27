# DENOISONG-of-ECG-SIGNALS-
ECG_denoising
Python command line application used to denoise ECG data using  deep neural network.



Considered noises:
1.baseline wander
2.power line interference
3.external electromagnetic fields
4.random body movements




Deep neural networks:
Each network was trained using QT database and MIT-BIH Noise Stress Database.

FCN-DAE:
Autoencoder neural network, used to teach network how to encode and decode desired signal. FCN-DAN results are much better than aforementioned methods, nevertheless network was learning on specific dataset.
mean RMSE = 1.859
mean MAD = 0.429

DRNN:
Simple neural network consisted of LSTM layer and densely connected following layers (consisted of 64 neurons each).
mean RMSE = 3.047
mean MAD = 0.689


Results:

![image](https://github.com/user-attachments/assets/c6f476ff-71bb-4d27-8eff-1b33c2aa4793)


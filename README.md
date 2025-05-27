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
mean RMSE = 0.150
mean MAD = 0.10

DRNN:
Simple neural network consisted of LSTM layer and densely connected following layers (consisted of 64 neurons each).
mean RMSE = 0.160
mean MAD = 0.0966


Results:
![image](https://github.com/user-attachments/assets/24dc90cc-0f0f-4537-878d-c7b06eae2c18)






Databases:
1.https://physionet.org/content/nstdb/1.0.0/
2.https://physionet.org/content/qtdb/1.0.0/




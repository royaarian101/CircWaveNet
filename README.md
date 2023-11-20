# CircWaveNet
CircWaveNet: A New Convolutional Neural Network Based on Combination of Circlets and Wavelets for Macular OCT Classification 

For the first time, we explore the impact of different X-lets on classifying OCT B-scans, featuring one normal class and two abnormal classes (AMD and DME). Different transforms of each B-scan have been fed to the designed 2D-Convolutional-Neural-Network (2D-CNN) to extract the best-suited features. Subsequently, MSVM and MLP classifiers were employed, revealing superior performance of 2D-DWT for normal cases and circlet transform for DME cases. Therefore, we combine these two X-lets and propose a new transform named CircWave which uses all sub-bands of both transformations in the form of a multi-channel-matrix, with the aim to increase the classification accuracy of normal and abnormal cases, simultaneously and improve the results.
In this research, MATLAB R2020a software was utilized for executing the pre-processing algorithm and obtaining contourlet, circlet, and ellipselet representations. Simultaneously, the Python 3.7 software environment with Keras and Tensorflow platform backend was employed to extract 2D-DWT, DTCW, and shearlet coefficients, as well as to implement classification models. Therefore we provide two folders for each software. 
If you utilize any portion or the entirety of this code, kindly cite the paper titled "CircWaveNet: A Novel Convolutional Neural Network Based on the Fusion of Circlets and Wavelets for Macular OCT Classification."


Initially, download all the .rar files and store them collectively in a folder named "codes". Subsequently, follow the steps below to implement the proposed "CircWaveNet".
1.	First download the data via https://misp.mui.ac.ir/en/dataset-oct-classification-50-normal-48-amd-50-dme-0 and extract the zip file and store it in DATA folder. 
2.	Navigate to the preprocessing folder within the MATLAB folder, and execute the preprocessing.m file to perform the preprocessing as outlined in the manuscript. 
3.	From the Python folder, run the data_sorting.py file in order to sort all B-scans in a dictionary.
4.	Utilize the preparing_data_for_matlab.py script located in the Python folder to prepare the data for circlet transformation.
5.	In the MATLAB folder open the Circlet_transform folder and run the main.m file.
6.	Run the CircWave.py file located in Python folder to decompose each B-scan into 19 sub-bands using the proposed CircWave transform.
7.	Ultimately, the execution of the classification based on the proposed method can be initiated by running the CircWaveNet.py file located in the Python folder.


For additional information, please reach out to us at: royaarian101@gmail.com.  

CircWaveNet: A New Convolutional Neural Network Based on Combination of Circlets and Wavelets for Macular OCT Classification
For the first time, we explore the impact of different X-lets on classifying OCT B-scans, featuring a normal class, a DME class and another abnormal classes (i.e. AMD). Different transforms of each B-scan have been fed to the designed 2D-Convolutional-Neural-Network (2D-CNN) to extract the best-suited features. Subsequently, MSVM and MLP classifiers were employed, revealing superior performance of 2D-DWT for normal cases and circlet transform for DME cases. Therefore, we combine these two X-lets and propose a new transform named CircWave which uses all sub-bands of both transformations in the form of a multi-channel-matrix, with the aim to increase the classification accuracy of normal and abnormal cases, simultaneously and improve the results. In this research, MATLAB R2020a software was utilized for executing the pre-processing algorithm and obtaining contourlet, circlet, and ellipselet representations. Simultaneously, the Python 3.7 software environment with Keras and Tensorflow platform backend was employed to extract 2D-DWT, DTCW, and shearlet coefficients, as well as to implement classification models. Therefore we provide two folders for each software. If you utilize any portion or the entirety of this code, kindly cite the paper titled "CircWaveNet: A Novel Convolutional Neural Network Based on the Fusion of Circlets and Wavelets for Macular OCT Classification."


Follow the steps below to implement the proposed "CircWaveNet".
1.	Store your data including three classes in three folders in the DATA folder.
2.	Do the preprocessing steps mentioned in the article “A new convolutional neural network based on combination of circlets and wavelets for macular OCT classification”. If you want to use the alignment algorithm you can find the code in the reference article “Kafieh R, Rabbani H, Abramoff MD, Sonka M. Curvature Correction of Retinal OCTs Using Graph-Based Geometry Detection. Phys Med Biol. 2013 May 7;58(9):2925–38.”
3.	From the Python folder, run the data_sorting.py file in order to sort all B-scans in a dictionary.
4.	Utilize the preparing_data_for_matlab.py script located in the Python folder to prepare the data for circlet transformation.
5.	In the MATLAB folder open the Circlet_transform folder and run the main.m file.
6.	Run the CircWave.py file located in Python folder to decompose each B-scan into 19 sub-bands using the proposed CircWave transform.
7.	Ultimately, the execution of the classification based on the proposed method can be initiated by running the CircWaveNet.py file located in the Python folder.

For additional information, please reach out to us at: royaarian101@gmail.com.

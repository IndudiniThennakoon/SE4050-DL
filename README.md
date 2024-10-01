
# 🏷️ NOTE:
- The modified answer notebooks (`lab_7_AE_FFNN.ipynb`, `lab_7_AE_Vanilla_CNN.ipynb` and, `lab_7_AE_CNN_Image_Denoising.ipynb`) are available in the repository.
- The answer sheet, including screenshots form Task 2 is in the `IT21170966_labsheet7_Answer.docx` word document.
  
# Deep Learning – Lab 7 - Autoencoders

## 🚀 Tasks 

1. Upload the Autoencoder (AE) jupyter notebook file (i.e., lab_7_AE_FFNN.ipynb) to google colab root directory.
     - In this code, an image reconstruction is done using dense layers-based AE.
     - Fashion MNIST dataset is used for this task (also for the subsequent tasks as well).
     - Run the above code and understand it.
     - Train the model with 30 epochs.
     - Write the code implementation to calculate the loss (Mean Squared Error) for the test dataset.
     - Write the code implementation to plot the train and validation loss against number of epochs.
     </br>

2. When above AE is used without activation functions, it is called a linear AE. Explain the relationship between linear AE and principal component analysis (PCA). Write the answer in a word file. </br>

3. Upload the Vanilla CNN AE jupyter notebook file (i.e., lab_7_AE_Vanilla_CNN.ipynb) to google colab root directory.
     - In this code, instead of dense layers, 2D CNN layers are used.
     - Task in the same as before with the same Fashion MNIST dataset.
     - Run the above code and understand it.
     - Train the model with 30 epochs.
     - Write the code implementation to calculate the loss (Mean Squared Error) for the test dataset.
     - Write the code implementation to plot the train and validation loss against number of epochs.
    </br>
4.	Observe the model performance improvements between the above two models and give reasons for the observed improvements.  </br>
5.	Upload the Image De-noising AE jupyter notebook file (i.e., lab_7_AE_CNN_Image_Denoising.ipynb) to google colab root directory.  </br>
     - In this code, noise is first added to the images before the reconstruction.
     - This is a method to overcome the overfitting that happens in AEs.
     - Run the above code and understand it.
     - Train the model with 30 epochs.
     - Write the code implementation to calculate the loss (Mean Squared Error) for the test dataset.
     - Write the code implementation to plot the train and validation loss against number of epochs.
     - Experiment with “noise_factor” value and use the best value you find in the final implementation. (Pay attention to how this value affect the images by observing the noise added images in the code.)
        </br>
6.	Observe the model performance improvements between the Image De-noising AE and the Vanilla CNN AE.
     - Explain the reasons for the observed improvements.
        </br>
7.	Explain the differences between AE and Variational AE (VAE).




___________     
<sub><sup>📌 *documented by @IndudiniThennakoon 2024* </sup></sub>

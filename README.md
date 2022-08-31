# DDL-Calibration-HestonModel

I applied the Differential Deep Learning (DDL) technique to price vanilla European options (i.e. the calibration instruments) when the underlying asset follows a Heston model and then calibrated the model using the trained network. This repository contains the code I have implemented to this end. You will find:
* 3 Jupyter notebooks intended to be opened in a Google Colab environment:

    1. ”DataGeneration.ipynb” file contains the implementation of the Heston pricer, the different differentials of the normalised forward put price w.r.t inputs as well as the generator used to build the datasets utilised to train, validate, and test the neural networks.
    2.  ”DifferentialNeuralNetworks.ipynb” file presents how to apply the DDL technique to price European put options when the underlying asset follows a Heston model. I also introduced different regularisation techniques and applied them notably in the case of the DDL. I compared their performance in reducing overfitting and improving the generalisation error. The DDL performance is also compared to the classical Deep Learning (DL) (without differentiation) one in the case of Feed-Forward Neural Networks. I showed that the DDL outperforms the DL.
    3.  ”Calibration.ipynb” presents how DDL is used to dramatically reduce Heston calibration’s computation time and compares traditional calibration to Differential Neural Network (DNN) based calibration.
    
* The files to be imported into the Google Colab environment.
* The files containing the different results.

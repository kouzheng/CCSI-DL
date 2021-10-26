# CCSI-DL
The model combines a bidirectional GRU with a one-dimensional convolution and uses the genome sequence of coronaviruses as direct input to predict the pandemic risk of human infection.

Guideline
1. The code is design based on Python 3.7.4 , tensorflow 2.1.0 and Keras 2.3.1.
2. seq_preprocess.py: preprocess the gene sequences of coronavirus.The input file is the full sequences of coronavirus genome as fasta format and should be put into the "fasta" folder.
3. predict_CCSI-DL.py: the main file to predict the cross-species transmission risk.The first parameter is the name of query file, the second parameter is the prediction confidence.
4. predicting_results.csv shows the result for the prediction of cross-species transmission. The predicted label for 'H' means the phenotype of cross-species transmission while label for 'N' means not.
5. The models mentioned in our paper are saved as HDF5 files in "model" folder.

Reference
Kou, Z., Huang, YF., Shen, A. et al. Prediction of pandemic risk for animal-origin coronavirus using a deep learning method. Infect Dis Poverty 10, 128 (2021).
https://doi.org/10.1186/s40249-021-00912-6
https://idpjournal.biomedcentral.com/articles/10.1186/s40249-021-00912-6

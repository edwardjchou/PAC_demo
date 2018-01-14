README

Code Descriptions:
PAC_sample.ipynb - Generates pac_guide.csv and the numpy files in pac_arrays.  Also holds some code for playing around to be ignored.
PAC_CNN_camera_and_sanitation_classification.ipynb - Trains a transfer learning model on all the data for sanitation labels, creates pca_camera_and_sanitation_classification.hdf5
PAC_CNN_camera_classification.ipynb - Trains a classifier on all data to classify camera source, creates pca_camera_classification.hdf5
PAC_CNN_sanitation_classification.ipynb - Trains a classifier for each camera to classify sanitation label, creates pca_camera_XX.hdf5
ImageAugmentation-master/img_transform_NB.ipynb - Generates the transformations of the images to augment dataset, also creates pac_transform_guide.csv and numpy arrays in pac_augment_arrays
PAC_Augmented_CNN.ipynb - Trains a classifier for each camera to classify sanitation label on augmented data, creates pca_augment_camera_XX.hdf5
PAC_CNN_Features.ipynb - Generates the data in pac_cnn_features by running images through VGG16 network
PAC_HOG.ipynb -  Generates the data in pac_hog_features, transforms images to HOGs, compresses into PCA
PAC_SVM_CNN.ipynb - Runs SVM on the CNN features, reports classification metrics
PAC_SVM_HOG.ipynb - Runs SVM on the HOG features, reports classification metrics
PAC_CNN_Metrics.ipynb - Reports classification metrics on weighted transfer learning model
PAC_CNN_Augmented_Metrics.ipynb - Reports classification metrics on augmented transfer learning model

PAC_runscript.ipynb - Testing script, use to run code on sample files 0.png and 20160930_084735_699.npz

CSV Guides Descriptions:
pac_guide.csv - Links indices to numpy file directories, also holds label information
pac_transform_guide.csv - Links indices to image file directories, also holds label information

Data Descriptions:
pac_arrays - Records indices of subsampling of pac_guide.csv
pac_augment_arrays - Records indices of subsampling of pac_transform_guide.csv
pac_cnn_features - Holds PCA compressed CNN features 
pac_hog_features - Holds PCA compressed HOG features
pac_models - Holds all the different models (move individual models to parent directory to run with code)

0.png - Sample augment image file, is camera_02 label 1
20160930_084735_699.npz - Sample numpy file, is camera_02 label 1

pac-research-sample.pdf - 2 page writeup
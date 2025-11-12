1) The folder LungAbnormalityDeterctorDataset(Plain), is the original dataset with un-augmented and un-processed images.



2) The folder LungAbnormalityDeterctorDataset(PreprocessedAugmented) contains the augmented and preprocessed images.



3) new-yolo-tbx11k is an extended version of tbx-11k-simplified. For every image in the latter dataset, this one contains:: The original image copy, Brightness & Contrast variation, Zoomed in and Gaussian Noise added copy, copy with applied CLAHE. This is in the yolo format to enable the training of the Yolo v8 model. It's been done using the script YoloDatasetGenerator.ipynb.



4) PakistanDataset(Plain) contains 2494 images of TB lungs and 514 images. These are unprocessed images and have been used for testing various models.



5) PlottedImages contains the images from new-yolo-tbx11k with their bounding boxes plotted using a 2 pixel wide, red line.


6) TB_ChestRadiography_Database contains the dataset used for training initial models. It contains images of the following category:: Normal, Tuberculosis, Viral Pneumonia and Bacterial Pneumonia.


7) tbx11k-simplified contains the raw dataset from Kaggle, that contains:: TB images, Sick but not TB images and Healthy lung images.


8) yolo-tbx11k-simplified contains the version of tbx11k-simplified that has been processed to be brought into the yolo format to enable the training of the Yolo v8 model. It's been done using the script YoloDatasetGenerator.ipynb.



9) DataPreprocessing&Augmentation contains the python 3.12.1 code that has been used to preprocess and augment the datasets for training. 


10) YoloDatasetGenerator.ipynb contains the script(python 3.12.1) that has been used to convert datasets into yolo architecture compatible formats(image folder with train and val sets, labels folder with train and val text files and a .yaml file containg all the paths).
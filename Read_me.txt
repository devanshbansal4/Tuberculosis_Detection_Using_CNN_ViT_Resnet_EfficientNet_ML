The .pt/ .keras/ .h5 files mentioned below have been removed, since many were too big for git. 
This repo contains multiple Models trained for detecting TB in Chest X-ray PA/AP view images.

1) The folder Model2 contains all contents of the EfficientNetB3 model(384 layers).
	-lungabnormalitydetectortwo.ipynb contains the code that trained the model.
	-LungAbnormalityDetectorTwoModel.h5 contains the reusable model.
	-PerformanceLungAbnormalityDetectorTwo.ipynb contains the model performance and the code that allows for the model to be used anytime.


2) The folder Model3 contains all contents of the Resnet50 model(177 layers).	
	-lungabnormalitydetectorthree.ipynb contains the code that trained the model.
	-LungAbnormalityDetectorThree_ModelResnet.h5 contains the reusable model.
	-LungAbnormalityDetectorThree_ModelResnet.tflite contains the reusable model for edge devices.
	-PerformanceLungAbnormalityDetectorThree.ipynb contains the model performance and the code that allows for the model to be used anytime.



4) The folder Model4 contains all contents of the Xception.	
	-lungabnormalitydetectorfour-xception.ipynb contains the code that trained the model.
	-LungAbnormalityDetectorFourModel_Xception.h5 contains the reusable model.
	-LungAbnormalityDetectorFourModel_Xception.tflite contains the reusable model for edge devices.
	-PerformanceLungAbnormalityDetectorFour.ipynb contains the code that allows for the model to be used anytime.



5) The folder Model5_ViT contains all contents of the pyTorch Model ViT.	
	-Model_5_ViT_Training.ipynb contains the code that trained the model.
	-best_model (1).keras contains the Keras model taht is called upon to segment lungs in the X-Ray image.
	-vit_model.pth contains the reusable predictive model for edge devices.
	-UseModel.ipynb contains the code that allows for the model to be used anytime. It first calls the best_model (1).keras to segment lungs in the image, and then calls vit_model.pth to make predictions on the segment lung images.


6) The folder Model6_CNN contains all contents of the custom 3 layered CNN model.	
	-model-6-cnn.ipynb contains the code that trained the model.
	-model_tb.h5 contains the reusable model.
	-results.csv contains the bounding box coordinates predicted.
	-UseModel6.ipynb contains the model performance and the code that allows for the model to be used anytime.



7) The folder Model7_resnet50 contains all contents of the Resnet50 model that predicts bounding box, this is an extension and an improved version of Mdel6_CNN.	
	-model-7-resnet50-training.ipynb contains the code that trained the model.
	-model-7-Resnet50.h5 contains the reusable model.
	-UseModel7.ipynb contains the code that allows for the model to be used anytime.


8) The folder Model8_Yolo8-tbx11k-simplified contains all contents of the yolov8s model trained on the dataset yolo-tbx11k-simplified.	
	-model8-yolov8.ipynb contains the code that trained the model.
	-best_tb_model.pt contains the reusable model.
	-model-performance.ipynb contains the test performance of the model
	-Use_Yolo_Model8.ipynb contains the code that allows for the model to be used anytime.


9) The folder Model9_Yolov8-new-tbx11k contains all contents of the model trained on the dataset new-yolo-tbx11k.	
	-model9-yolov8-new.ipynb contains the code that trained the model.
	-best_tb_model.pt contains the reusable model.
	-model-performance.ipynb contains the model performance on the test set.
	-UseModelUsingPath.ipynb contains the code that allows for the model to be used anytime.


8) The folder Model10_Yolov8m-tbx11k-simplified contains all contents of the model trained on the dataset yolo-tbx11k-simplified. This is an advanced and a bigger architecture of the yolov8 model, that is the "m" version.	
	-model10-yolov8m.ipynb contains the code that trained the model.
	-best.pt contains the reusable model.
	-mode-performance.ipynb contains the model performance on the test set.
	-UseModel.ipynb contains the code that allows for the model to be used anytime.









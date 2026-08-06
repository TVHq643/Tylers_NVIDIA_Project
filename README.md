## Bone Fracture Detector

Uses a detectnet neural network to identify if a x-ray contains a fracture. Made to be eventually used to identify fractures in ERs faster and more efficiently, allowing doctors to spend more time treating the patient directly. 

## The Algorithm

The detectnet neural network is trained on x ray images from a kaggle dataset (https://www.kaggle.com/datasets/osamajalilhassan/bone-fracture-dataset) and is programmed to identify bone fractures in those images. When it is trained, it learns patterns in what images are fractured and which are not, letting it identify fractures in a patient x ray.


## Running this project

- Go to GitHub and download the model

- Set variables (NET=model/checkmodel2phase)(DATA=data/dataset) 

- Go into the Test folder and select an image

- Run the command to process the image (imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$DATASET/labels.txt $DATASET/test/<fractured/not_fractured>/<IMAGE_FILE_NAME> <RESULT_NAME>.jpg)

[View a video explanation here](video link)

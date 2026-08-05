Bone Fracture Detector

Uses a detectnet nurial network to identefy if a x-ray contains a fracture. Ment to be eventuly used to identefy fractures in ERs faster and more efficiantly, allowing doctors to spend more time treating the patient directly. 

![add image descrition here](direct image link here)

## The Algorithm

The nurial network is trained on x ray images and is programmed to decect bone fractures in those images. When it is trained, it learns patterns in what images are fractured and which are not, letting it identify fractures in a patint x ray.


##Running this project

- Go to GitHub and download the model

-set variables (NET=model/check2phase)(DATA=data/dataset) 

- Go into the Test folder and select an image

- Run the command to process the image (imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$DATASET/labels.txt $DATASET/test/<fractured/not_fractured>/<IMAGE_FILE_NAME> <RESULT_NAME>.jpg)

[View a video explanation here](video link)
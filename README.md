# Enhanced Object Detection in Low-Visibility Haze Conditions with YOLOv9s

This repository contains the code and instructions to validate the GEW-Yolov9 model on the COCO validation dataset. Follow the steps below to set up the environment, prepare the data, and perform validation.

First, ensure that you have Python installed on your system. Then, install the necessary dependencies by running the following command: 

```bash
pip install -r requirements.txt
```

This will install all the required libraries to run the model and perform validation.

To validate the model, you need to download the COCO validation dataset. Place the dataset in the appropriate directory, or update the data path in the configuration file if necessary.

Once the environment is set up and the data is ready, you can run the validation process using the following command:

```bash
cd GEW-Yolov9
python val.py --data data/coco.yaml --img 640 --batch 32 --conf 0.001 --iou 0.7 --device 0 --weights './model.pt' --save-json --name yolov9
```

After running the command, the validation results will be generated and saved in the specified format.

Make sure to adjust any paths or configurations according to your environment and requirements. For more details on using the Yolov9 framework, refer to the official documentation.

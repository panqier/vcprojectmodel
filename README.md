- first step is unzip the images.zip using command:
  
  unzip vcmodel/dataset/images.zip

- move images folder under dataset -> dataset/images

- unzip dataset-resized.zip under trashnet/data

- download yolo model using command:
  
  python -m venv venv

  source venv/bin/activate

  pip install ultralytics opencv-python matplotlib

- run the yolo model:
  (epochs is how many turns, and imgsz is input size, both can be modified)
  
  yolo detect train data=dataset/dataset.yaml model=yolov8n.pt epochs=30 imgsz=640

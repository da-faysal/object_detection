This project is about object detection (Koala) using pretrained yolov5 model. Validation and training metrics are found inside yolov5/runs/val/exp and yolov5/runs/train/exp respectively. The following commands need to be executed to run train and val script:

(to train) python train.py --img 640 --batch 16 --epochs 20 --data custom_data.yaml --weights yolov5s.pt --cache

(to validate using the best model in training) python val.py --img-size 640 --batch-size 16 --conf-thres 0.001 --iou-thres 0.6 --data custom_data.yaml --weights runs/train/exp/weights/best.pt

While running the 2 commands above, make sure you are inside yolov5 directory.
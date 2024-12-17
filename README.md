# YOLOv7
Group member: Yihao Liao & Adekunle Timothy ADEWOYE

The AIA project: 1.Modification of YOLOv7 

## Jobs we have done
1. Understanding of YOLOv7
2. Change the upsample model to dynamic sample model
3. Change the coco dataset to VisDrone dataset
4. Finish the training part for the modified YOLOv7 model

## Jobs we still need to do
1. Compare the YOLOv7 and the modified YOLOv7
2. Finish the testing part and visulize the results
3. Complete the presentation slides


## How to train the modified model
By training the modified model, we use the YOLOv7-tiny model and make a change in it. And we also change the dataset to VisDrone dataset, which is smaller, containing less classes, but faster for training.
```
python train.py --workers 8 --device 0 --batch-size 32 --data data/visdrone_new.yaml --img 640 640 --cfg cfg/training/yolov7-tiny.yaml  --name yolov7-tiny --hyp data/hyp.scratch.p5.yaml
```


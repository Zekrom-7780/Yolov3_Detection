# YOLOv3_Detection
 
This is the Yolov3 Detection fot static images as well as videos.


## Requirements
- OpenCV 4.4
- Python 3.6    
- Tensorflow-gpu 2.12.0 
- Keras 2.1.3

## Quick start

So to run this code, you need to:

- Download official [yolov3.weights](https://pjreddie.com/media/files/yolov3.weights) and put it on top floder of project.

- Run the follow command to convert darknet weight file to keras h5 file. This `yad2k.py` was modified from [allanzelener/YAD2K](https://github.com/allanzelener/YAD2K).
```
python yad2k.py cfg\yolo.cfg yolov3.weights data\yolo.h5
```

- run follow command to show the demo. The result can be found in `images\res\` floder.
```
python demo.py
```

## Demo result

<img width="400" height="350" src="/images/res/dog.jpg"/><img width="400" height="350" src="/images/res/person.jpg"/>

## Implementation in Rust

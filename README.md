# robot-face-detect


![Ton](images/ton.jpg)

```
# tree
.
├── README.md
├── age_detector
│   ├── age_deploy.prototxt
│   └── age_net.caffemodel
├── detect_age.py
├── detect_age_video.py
├── face_detector
│   ├── deploy.prototxt
│   └── res10_300x300_ssd_iter_140000.caffemodel
├── images
│   └── ton.jpg
├── object_tracker.py
└── pyimagesearch
    └── centroidtracker.py
```

```
# Age detection from images
python3 detect_age.py --image images/ton.jpg --face face_detector --age age_detector

# Real-time age detection with OpenCV
python3 detect_age_video.py --face face_detector --age age_detector

# Real-time object tracking with OpenCV
python3 object_tracker.py --prototxt face_detector/deploy.prototxt --model face_detector/res10_300x300_ssd_iter_140000.caffemodel

```
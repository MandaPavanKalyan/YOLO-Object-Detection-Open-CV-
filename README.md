# Object Detection using YOLO

## Features
- **Object Detection**: Detects objects in real-time using YOLO (You Only Look Once).
- **Text-to-Speech**: Speak out the detected object names using `pyttsx3`.
- **Multiple Object Detection**: Detects multiple objects and displays the count.

---

## Installation

Ensure you have Python installed (>=3.6). Install the required dependencies:

```sh
pip install pyttsx3 pywin32 opencv-python opencv-contrib-python imutils numpy
```

For text-to-speech on Windows, you may also need:

```sh
pip install pywin32
```

## Usage

1. **Download YOLO Weights**: Download the YOLO weights file from [here](https://pjreddie.com/media/files/yolov3.weights).
2. **Prepare COCO Names**: Create a `coco.names` file with the COCO dataset class names.
3. **Run Object Detection**: Use the provided Python script to run object detection on a video stream or images. The script will:
    - Load YOLO model and COCO names.
    - Capture video from the webcam.
    - Perform object detection.
    - Display the detected objects and their count.
    - Optionally, use text-to-speech to announce detected objects.

### Example Output

Upon running the script, you should see the video stream with detected objects outlined by bounding boxes and labels. The console will display the detected objects and their count.

```plaintext
Wait for calibrations...
Start speaking...
Recorded successfully
Recognized Speech: "hello"
Translating...
Type the translation language code: fr
Translation: "bonjour"
```

```plaintext
Enter the sentence: "How are you?"
Detected Language: en
Type the translation language code: es
Translation: "¿Cómo estás?"
Detected Translated Language: es
```

### COCO Names

```plaintext
person
bicycle
car
motorbike
aeroplane
bus
train
truck
boat
traffic light
fire hydrant
stop sign
parking meter
bench
bird
cat
dog
horse
sheep
cow
elephant
bear
zebra
giraffe
backpack
umbrella
handbag
tie
suitcase
frisbee
skis
snowboard
sports ball
kite
baseball bat
baseball glove
skateboard
surfboard
tennis racket
bottle
wine glass
cup
fork
knife
spoon
bowl
banana
apple
sandwich
orange
broccoli
carrot
hot dog
pizza
donut
cake
chair
sofa
pottedplant
bed
diningtable
toilet
tvmonitor
laptop
mouse
remote
keyboard
cell phone
microwave
oven
toaster
sink
refrigerator
book
clock
vase
scissors
teddy bear
hair drier
toothbrush
```

## Future Enhancements

- Improve object detection accuracy.
- Add support for offline object detection.
- Implement voice selection and accents in text-to-speech.
- Integrate machine learning for smarter object detection and recognition.

## Author

Developed by Pavan Kalyan Manda

Website Developer | IoT & Embedded Systems Enthusiast | AI/ML Developer

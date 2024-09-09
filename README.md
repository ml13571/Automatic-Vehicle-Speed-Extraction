[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LsMQRXMKSvoYOkSkia0CwEa5j7TdQWPw?usp=sharing)

# Speed Estimation from Video using YOLOv9 and DeepSORT

This project estimates the speed of objects in a video using YOLOv9 for object detection and DeepSORT for tracking. The estimated speeds are overlaid on the video along with bounding boxes around the detected objects.

## Installation

1. Create new environment:
  - Using Conda
  ```
  conda env create -f conda.yml
  conda activate speed_py311
  ```

2. Install YOLOv9 dependency:
  ```
   pip install -r yolov9/requirements.txt
  ```
3. Download model weights:
  ```
   mkdir weights
   wget -P weights https://github.com/WongKinYiu/yolov9/releases/download/v0.1/yolov9-e.pt
  ```
4. Download input video:
  ```
   mkdir content
   wget -P content https://github.com/AarohiSingla/Speed-detection-of-vehicles/raw/main/highway.mp4
   wget -P content https://github.com/AarohiSingla/Speed-detection-of-vehicles/raw/main/highway_mini.mp4
  ```  
5. Run:
  ```
   python3 object_tracking.py
  ```  

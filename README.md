
# yolov5_opencv_cpp_python
Object Detection using YOLOv5 and OpenCV DNN (C++ and Python)
[Original Source](https://learnopencv.com/object-detection-using-yolov5-and-opencv-dnn-in-c-and-python/)


```bash
git clone --recursive git://github.com/majnas/yolov5_opencv_cpp_python.git
cd yolov5

# Install dependencies.
pip install -r requirements.txt
pip install onnx

# Download .pt model.
cd models
wget https://github.com/ultralytics/YOLOv5/releases/download/v6.1/YOLOv5s.pt

# Export to ONNX
python export.py --weights models/YOLOv5s.pt --include onnx
```


# To use python
```python
    cd py
    python main.py
```


# To compile cpp version
```python
    cd cpp
    mkdir build
    cd build
    cmake ..
    make     
```

# To run cpp version
```python    
    cd cpp/build
    ./app
```

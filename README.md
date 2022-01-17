# fire-smoke-detection
YOLO V5 Fire - Smoke

# pip install -r requirements.txt

# Base ----------------------------------------
matplotlib>=3.2.2
numpy>=1.18.5
opencv-python>=4.1.2
Pillow>=7.1.2
PyYAML>=5.3.1
requests>=2.23.0
scipy>=1.4.1
torch>=1.7.0
torchvision>=0.8.1
tqdm>=4.41.0

# Logging -------------------------------------
tensorboard>=2.4.1
# wandb

# Plotting ------------------------------------
pandas>=1.1.4
seaborn>=0.11.0

# Export --------------------------------------
# coremltools>=4.1  # CoreML export
# onnx>=1.9.0  # ONNX export
# onnx-simplifier>=0.3.6  # ONNX simplifier
# scikit-learn==0.19.2  # CoreML quantization
# tensorflow>=2.4.1  # TFLite export
# tensorflowjs>=3.9.0  # TF.js export


!python detect.py --weights last.pt --img 640 --conf 0.25 --source data/images

!python detect.py --weights last.pt --img 640 --conf 0.25 --source 0           = real time work
!python detect.py --weights last.pt --img 640 --conf 0.25 --source example.mp4 = just videos (mp4,webm...)
!python detect.py --weights last.pt --img 640 --conf 0.25 --source example.jpg = just image (jpg,png...)
python detect.py --weights last.pt --img 640 --conf 0.25 --source fotos/1.jpg 
or -----------------
python detect.py --weights last.pt --img 640 --conf 0.25 --source 0  
more fast python detect.py --weights last.pt --img 350 --conf 0.25 --source 0  #250, 300 ....
if you want , you can use -- conf 0.50 (the best detect)

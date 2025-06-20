# YOLOv5 v3 – Custom Object Detection

This repository showcases object detection using **YOLOv5**, trained on a custom dataset (v3 version). The model was developed and trained on **Kaggle**, achieving improved accuracy over previous versions.

---

## 🔍 Project Overview

- **Model**: YOLOv5 (Ultralytics)
- **Version**: v3
- **Dataset**: Custom dataset (e.g., animals, vehicles, etc.)
- **Training Platform**: Kaggle Notebooks
- **Framework**: PyTorch

---

## 🧠 Features

- Custom dataset object detection using YOLOv5
- Supports image and video inference
- Model trained on GPU (Kaggle runtime)
- Outputs include predictions, metrics, and best model

---

## 🗂️ Folder Structure

YoloV5/
├── runs/
│ └── train/
│ └── exp3/ ← Output from v3 training
├── data/ ← YAML and dataset structure
├── weights/ ← Trained model (best.pt)
├── detect.py ← Inference script
├── train.py ← Training script
├── README.md ← This file


---

## 🚀 How to Use

1. **Clone the repository**:

```bash
git clone https://github.com/pranavmukundanA/Yolov5-v3.git
cd Yolov5-v3

2.Install YOLOv5 dependencies:
pip install -r requirements.txt

3.Train the model:
python train.py --img 640 --batch 16 --epochs 50 --data data.yaml --weights yolov5s.pt

4.Run inference:
python detect.py --weights weights/best.pt --img 640 --conf 0.25 --source your_image_or_vide


5.Results:
| Metric        | Value  |
| ------------- | -----  |
| Precision     | 61.38% |
| Recall        | 94.88% |
| mAP@0.5       | 64.02% |
| mAP@0.5:0.95  | 55.70% |

6.Tech Stack
Python
PyTorch
YOLOv5 (Ultralytics)
Kaggle
Git & GitHub


---

Let me know if you want:
- This pushed automatically
- Help generating a `.gitignore`
- Instructions for uploading `best.pt` as a release

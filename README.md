# TIAND-Vision  
### Benchmarking Camera-Based Object Detection Models on Unstructured Indian Roads

TIAND-Vision is a large-scale real-world camera dataset created for evaluating object detection systems in the highly diverse, dense, and unstructured traffic environments of India.  
The dataset is designed to push perception systems beyond structured-road assumptions toward real deployment readiness.

---


<p align="center">
  <img src="[assets/tiand_vehicle.jpg](https://github.com/kumpati-aravind77/TIAND-Vision-/blob/main/assets/tiand_vehicle.png)" width="800">
</p>


## 🚗 Highlights

- 7100+ km of driving  
- 30+ cities across India  
- 154 hours of recordings  
- ~300K captured images  
- ~100K manually annotated frames  
- 29% night-time data  
- Fog, rain, haze conditions  
- Dense traffic & long-tail objects  
- YOLO compatible annotations  
- 26 traffic & safety-critical classes

---

## 🌍 Driving Conditions Covered

- Urban city traffic  
- Rural environments  
- Highways  
- Ghat / mountain roads  
- Tunnels  
- Marketplace & pedestrian-heavy areas  
- Day & night  
- Adverse weather

---

## 🧠 Categories (26)
person
bicycle
car
motorcycle
route board
bus
commercial vehicle
truck
traffic sign
traffic light
autorickshaw
ambulance
construction vehicle
animal
unmarked speed bump
marked speed bump
pothole
police vehicle
tractor
pushcart
temporary traffic barrier
rumblestrips
traffic cone
zebra crossing
van
rickshaw



The dataset follows a natural long-tail distribution, making rare-class detection a primary challenge.

---

## 📊 Dataset Scale

| Metric | Value |
|-------|------|
| Raw Frames | ~300,000 |
| Annotated Frames | ~100,000 |
| Annotation | 2D Bounding Boxes |
| Format | YOLO |
| Resolution | 1280 × 720 |

---

## 🗂 Directory Layout

```
TIAND-Vision/
├── images/
│   ├── train/
│   ├── val/
│   └── test/
├── labels/
│   ├── train/
│   ├── val/
│   └── test/
└── data.yaml
```


---

## 🧾 Annotation Format

Each image has a `.txt` file:

All values are normalized.

---

## 🧪 Baseline Benchmark Results

| Model | mAP@0.5 | mAP@0.5:0.95 | Precision | Recall |
|------|--------|-------------|----------|--------|
| YOLOv5 | 0.895 | 0.651 | 0.854 | 0.858 |
| YOLOv8 | 0.902 | 0.673 | 0.856 | 0.866 |
| YOLOv9 | 0.896 | 0.659 | 0.838 | 0.871 |
| **YOLOv11** | **0.907** | **0.679** | 0.854 | **0.873** |
| Faster R-CNN | 0.465 | 0.289 | 0.465 | 0.383 |
| RT-DETR | 0.895 | 0.646 | 0.645 | 0.766 |

YOLOv11 currently provides the strongest balance of localization accuracy and recall in dense Indian traffic scenes.



# VisionGuard — Object Detection & Safety Classification

A lightweight image‑moderation + object‑detection system powered by the web and deployed to HuggingFace.

**Repository:** https://github.com/Harshitsoni294/VisionGuard-Object_Detection_NSFW_System  
**Live Demo:** https://huggingface.co/spaces/Harshitsoni294/Object-detection-and-safety-classification  

This project offers two primary capabilities:

- **NSFW / SFW image classification**  
- **Object detection with bounding boxes**  

---

## 🚀 Live Demo  
Visit the live interactive demo:  
https://huggingface.co/spaces/Harshitsoni294/Object-detection-and-safety-classification

---

## 🧠 Project Overview  
Modern applications involving user‑generated content require both content moderation and object recognition. VisionGuard provides:

- **Fast inference**
- **Lightweight deployment**
- **Simple web interface**
- **Clean API outputs**

### Workflow  
1. Upload image  
2. NSFW classifier processes input  
3. Object detector extracts objects + bounding boxes  
4. Combined result returned  

---

## 🏗️ Features  
### ✔ NSFW Detection  
- Safe / Not Safe classification  
- Confidence score  

### ✔ Object Detection  
- Multi‑object detection  
- Bounding boxes + labels  
 

### ✔ HuggingFace Deployment  
- Drag‑and‑drop image upload  
- Real‑time inference  

---

## 📂 Installation  
```bash
git clone https://github.com/Harshitsoni294/VisionGuard-Object_Detection_NSFW_System.git
cd VisionGuard-Object_Detection_NSFW_System
pip install -r requirements.txt
```

---

## 💻 Usage  
```python
from model import classify_nsfw, detect_objects
from PIL import Image

img = Image.open("example.jpg")

nsfw_result = classify_nsfw(img)
objects = detect_objects(img)

print(nsfw_result)
print(objects)
```

---

## 📜 Output Formats  
### NSFW
```json
{
  "status": "safe",
  "confidence": 0.92
}
```

### Detection
```json
[
  {
    "label": "dog",
    "bbox": [102, 55, 340, 290]
  }
]
```

---

## 🖼️ Screenshots  
Place your screenshots here:

```
<img width="1919" height="858" alt="image" src="https://github.com/user-attachments/assets/32d112f3-79a0-4df2-b4b2-ab93a5be711b" />
<img width="747" height="547" alt="image" src="https://github.com/user-attachments/assets/6404e66b-5e40-47c6-84ea-4cf5e807415b" />
<img width="746" height="392" alt="image" src="https://github.com/user-attachments/assets/e2df3121-a44a-46da-b281-ece5ec9c76ea" />

```

---

## 🌍 Deployment  
Use HuggingFace Spaces → Gradio → upload repository → done!

---

## 📜 License  
MIT License — free to use and modify.

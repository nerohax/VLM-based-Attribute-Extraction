# 🧠 Human-Face Attribute Extraction Pipeline

This project implements a complete pipeline that detects humans and faces in images, crops individual faces with contextual information, and extracts key facial attributes using a Vision-Language Model (VLM) via the OpenRouter API.

---

## 🔍 Use Case

Useful for applications like:

- Facial analysis
- Skincare recommendation engines
- Age/gender estimation tools
- VLM-based interpretation pipelines

---

## 📸 Pipeline Overview

1. **Human Detection**  
   Detects all humans in an image using pre-trained object detection models like YOLOv8 or GroundingDINO.

2. **Face Detection**  
   For each detected human, a face detector (e.g., Mediapipe, MTCNN) is used to locate individual faces.

3. **Face Cropping**  
   Detected faces are cropped from the original image with context to maintain a natural aspect ratio and include surrounding skin regions.

4. **Attribute Extraction using VLM**  
   The cropped face is sent to a Vision-Language Model via the OpenRouter API, and it returns structured facial attributes.

---
## VLM Sample Output
{
  
  "gender": "Male",
  "age_estimate": "25-30",
  "skin_conditions": ["acne", "redness", "baggy eyes"]
  
}
---
## Install Requirements.txt
     pip install -r requirements.txt
---


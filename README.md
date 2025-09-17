# 🌾 Crop Disease Classification with MobileNetV3-Large

This repository contains a fine-tuned **MobileNetV3-Large** model for crop disease classification across **17 classes** of corn, cotton, rice, and wheat.  
The model is trained on a **balanced dataset** of 418 images per class and achieves high accuracy on both validation and test sets.  

---

## 📊 Dataset
- **Classes (17 total):**
  - Corn: Common Rust, Gray Leaf Spot, Healthy, Northern Leaf Blight
  - Cotton: Bacterial Blight, Curl Virus, Fusarium Wilt, Healthy
  - Rice: Bacterial Leaf Blight, Brown Spot, Healthy, Leaf Blast, Leaf Scald, Sheath Blight
  - Wheat: Brown Rust, Healthy, Yellow Rust

- **Split (per class, 418 images):**
  - Train: 292  
  - Validation: 62  
  - Test: 64  

- **Total images:** 7,106  

---

## 🧠 Model Details
- **Base Model:** MobileNetV3-Large (pretrained on ImageNet)
- **Fine-tuning:** Last classification layer modified for 17 output classes
- **Optimizer:** AdamW
- **Loss Function:** CrossEntropyLoss
- **Training Strategy:** Balanced dataset with stratified split

---

## ✅ Performance
| Dataset      | Accuracy | Loss   |
|--------------|----------|--------|
| Validation   | **96.02%** | 0.4758 |
| Test         | **95.86%** | 0.4682 |

---

# 🛡️ RUDRA - REAL TIME UNMASKING OF DEEPFAKE DETECTION ALGORITHM

**RUDRA** is a hybrid deepfake detection architecture leveraging both ResNeXt and LSTM models. It is designed for high-accuracy deepfake video classification using a custom dataset aggregated from popular sources like **FaceForensics++**, **DFDC**, and **Celeb-DF**.

---

## 📦 Dataset Summary

We created a custom dataset of **6000 videos** from three well-known sources:

| Dataset           | No. of Videos |
|------------------|---------------|
| FaceForensics++  | 2000          |
| DFDC             | 3000          |
| Celeb-DF         | 1000          |
| **Total**        | **6000**      |

All videos were processed into face frames and stored as `Video + Target` pairs to be loaded by our custom data pipeline.

---

## 🧠 Model Architecture

![Architecture](architecture.png)

### Components:
- **ResNeXt:** for spatial feature extraction
- **LSTM:** for temporal sequence learning
- **Cloud-enabled training & inference**

🔴 **Training Flow** | 🟢 **Prediction Flow**

---

## 📊 Selected Results

| Model Name                         | Dataset         | Sequence Length | Accuracy (%)  |
|-----------------------------------|------------------|------------------|---------------|
| model_97_acc_80_frames_FF_data    | FaceForensics++  | 80               | **97.73%**    |
| model_97_acc_100_frames_FF_data   | FaceForensics++  | 100              | **97.76%**    |
| model_91_acc_60_frames_final_data | Our Dataset      | 60               | **91.59%**    |
| model_93_acc_100_frames_final_data| Our Dataset      | 100              | **92.10%**    |

These models demonstrate excellent accuracy, particularly for longer frame sequences.

---

## 🧩 Technologies Used

- Python, OpenCV, PyTorch
- ResNeXt + LSTM
- Custom dataset loader and video frame extraction
- Preprocessing pipeline for face-centric training

---

## 🔗 Dataset Access

[📁 Google Drive Link](https://drive.google.com/drive/folders/1WoCykd-dNAXJkB_YW-Unee4bhFQpDz3S?usp=drive_link)

---

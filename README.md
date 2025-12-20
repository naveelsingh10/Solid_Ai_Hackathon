# Solid AI Hackathon - Fastener Detection System

[![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
[![Model](https://img.shields.io/badge/Model-YOLO11m-green)](https://github.com/ultralytics/ultralytics)
[![Hugging Face](https://img.shields.io/badge/Hugging%20Face-Model%20Weights-yellow)](https://huggingface.co/naveelsingh10/final_solidworks-yolo)

> **Fast & accurate fastener detector using YOLO11m for Solid AI Hackathon IITM. Classifies bolts, nuts, washers & locating pins.**

## 📌 Project Overview
This repository contains the solution for the **Solid AI Hackathon** at IIT Madras. The system uses a custom-trained **YOLO11m (Medium)** model to detect, classify, and count industrial fasteners in high-resolution images.

The pipeline is optimized for high-volume inference, featuring a local caching mechanism that accelerates processing speed by **10x** on Google Colab T4 GPUs.

## 🛠️ Tech Stack
* **Framework:** [Ultralytics YOLO11](https://github.com/ultralytics/ultralytics)
* **Model Architecture:** YOLO11m
* **Language:** Python 3.10+
* **Key Libraries:** `ultralytics`, `pandas`, `huggingface_hub`

## 🎯 Classes Detected
The model is trained to identify and count the following components:
1.  **Bolt**
2.  **Nut**
3.  **Washer**
4.  **Locating Pin**

## 🚀 Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/naveelsingh10/Solid_Ai_Hackathon.git](https://github.com/naveelsingh10/Solid_Ai_Hackathon.git)
    cd Solid_Ai_Hackathon
    ```

2.  **Install dependencies:**
    ```bash
    pip install ultralytics pandas huggingface_hub
    ```

## 💻 Usage

The inference script automatically downloads the trained model weights from Hugging Face and generates the `submission.csv` file.

### Running the Inference Script
1.  Open the `submission.py` (or your main script file).
2.  Update the `drive_test_dir` variable to point to your image dataset path.
3.  Run the script:

```python
python submission.py

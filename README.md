# Solid AI Hackathon - Fastener Detection System

[![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
[![Model](https://img.shields.io/badge/Model-YOLO11m-green)](https://github.com/ultralytics/ultralytics)
[![Hugging Face](https://img.shields.io/badge/Hugging%20Face-Model%20Weights-yellow)](https://huggingface.co/naveelsingh10/final_solidworks-yolo)

> **Fast & accurate fastener detector using YOLO11m for Solid AI Hackathon IITM. Classifies bolts, nuts, washers & locating pins.**

##  Project Overview
This repository contains the solution for the **Solid AI Hackathon** at IIT Madras. The system uses a custom-trained **YOLO11m (Medium)** model to detect, classify, and count industrial fasteners in high-resolution images.

The pipeline is optimized for high-volume inference, featuring a local caching mechanism that accelerates processing speed by **10x** on Google Colab T4 GPUs.

##  Tech Stack
* **Framework:** [Ultralytics YOLO11](https://github.com/ultralytics/ultralytics)
* **Model Architecture:** YOLO11m
* **Language:** Python 3.10+
* **Key Libraries:** `ultralytics`, `pandas`, `huggingface_hub`

##  Classes Detected
The model is trained to identify and count the following components:
1.  **Bolt**
2.  **Nut**
3.  **Washer**
4.  **Locating Pin**

##  Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/naveelsingh10/Solid_Ai_Hackathon.git](https://github.com/naveelsingh10/Solid_Ai_Hackathon.git)
    cd Solid_Ai_Hackathon
    ```

2.  **Install dependencies:**
    ```bash
    pip install ultralytics pandas huggingface_hub
    ```

##  Usage

The inference script automatically downloads the trained model weights from Hugging Face and generates the `submission.csv` file.

### Running the Inference Script

1. **Open in Google Colab:**
   Download the `Solid_Ai_Hackathon.ipynb` notebook and upload it to Google Colab, or use the link below to open it directly:
   https://colab.research.google.com/drive/1Nc4WY35AxWso28AF86md57MYCgoZn9cp?usp=sharing

2. **Select GPU Runtime:**
   In the Colab menu, go to **Runtime > Change runtime type** and select **T4 GPU** to ensure faster processing.

3. **Configure and Run:**
   Locate the `test_dir` variable in the notebook cells. Update this path to point to your specific image dataset location. Once updated, run all cells to generate the results.

##  Project Presentation

You can view the detailed project presentation, including our approach and architecture, on Canva:

[**View Project Presentation**](https://www.canva.com/design/DAG7-32oerk/6wAM1wupJThA0EhKTQPJoA/edit?utm_content=DAG7-32oerk&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

## Certificate  

Uploaded in Main dir

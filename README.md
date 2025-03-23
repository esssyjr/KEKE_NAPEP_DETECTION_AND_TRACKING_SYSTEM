# KEKE_NAPEP_DETECTION_AND_TRACKING_SYSTEM  

![Image](https://github.com/user-attachments/assets/15dd6579-e843-4f8f-b1ed-3f4909abce0b)

## Overview  

This project focuses on detecting and tracking **KEKE_NAPEP** (tricycles), a primary mode of public transportation in Nigeria. Built using **YOLOv8**, the system enables real-time identification, tracking, and analysis of Keke Napep in video streams. By integrating **object detection, tracking, and counting features**, this project serves as a foundation for various applications, including **traffic management, fleet monitoring, and urban mobility analysis**.  

## Features  
- **Real-time detection** of Keke Napep using a **custom-trained YOLOv8 model**  
- **Tracking** Keke Napep across multiple video frames using the **Supervision library from Roboflow**  
- **Polygon zone feature** for counting Keke Napep entering predefined areas  
- **Scalability** for large-scale deployments in traffic monitoring and urban planning  

---

# Dataset

The dataset consists of **84 annotated images**, sourced from **various locations in Kano State, Nigeria**, capturing diverse environmental conditions. Both images and labels are provided in **YOLO format**, making it directly compatible with **Ultralytics YOLOv8** and other object detection models.  

## Annotation Details
- **Annotation Tool:** CVAT.ai  
- **Labeling:** Each image is manually labeled to ensure accurate detection.

## Dataset Link
The dataset is publicly available on **Kaggle**:  
📂 **[Keke Napep (Tricycle) Dataset](https://www.kaggle.com/datasets/ismailismailtijjani/keke-napep-tricycle-dataset)**  

## Future Improvements for dataset
Future improvements include expanding the dataset to cover:  
- **More geographical locations** across Nigeria, including **urban, rural, and suburban areas**.  
- **Various weather conditions**, such as **day, night, and different lighting scenarios**.  
- **Different KEKE NAPEP varieties**, including **various colors, designs, and modifications**.  




---

## Model Training  

The **YOLOv8n** model (lightweight version of YOLOv8) was chosen for its balance between **efficiency and accuracy**, making it suitable for deployment on devices with limited computational power.  

- **Training Duration:** 100 epochs  
- **Performance:** The model demonstrated **high accuracy** in detecting KEKE_NAPEP under different conditions  

---

## Tracking Implementation  

Building on the **Keke Napep Detection Model**, a tracking system was developed to monitor movement over time. The system:  

1. **Captures video streams**  
2. **Detects Keke Napep in each frame** using the trained model  
3. **Tracks movement across frames** using **Supervision (Roboflow)**  
4. **Counts** Keke Napep within predefined **polygon zones**  

### **Polygon Zone Counting**  
A **polygon zone feature** was integrated, allowing the system to:  
- Detect when Keke Napep enter specific zones  
- Count the number of Keke Napep inside the zone in **real-time**  
- Analyze **traffic density** and congestion in predefined areas  

#### **Tracking Demo**  
Watch the tracking test video here:  
📹 [KEKE_NAPEP_VIDEO_TRACKING_DEMO_1](https://youtu.be/sZ4QVAU8XIg?si=ywSxweO6F7owK_5B)  
📹 [KEKE_NAPEP_VIDEO_TRACKING_DEMO_2](https://youtu.be/UOqrPQgLDT8?si=5i_yNVAhxckf7DjR)  

---

## Future Improvements  

### **1. Speed Estimation**  
- Estimate **KEKE_NAPEP speeds** by analyzing their movement across multiple frames  
- Use **frame rate and distance traveled** for precise calculations  

### **2. Improved Object Tracking**  
- Enhance tracking using **Kalman filters** or deep-learning-based trackers  
- Reduce ID switching for long-duration tracking  

### **3. Real-World Applications**  
- **Government & Transport Authorities:** Traffic monitoring and regulatory enforcement  
- **Fleet Operators:** Real-time monitoring and optimization  
- **Urban Planning:** Data-driven decision-making for mobility solutions  
- **Autonomous Vehicles:** Possible integration into self-driving navigation systems  

---


## Installation & Usage

### Step 1: Clone the Repository
```sh
git clone https://github.com/esssyjr/KEKE_NAPEP_DETECTION_AND_TRACKING_SYSTEM.git
cd naira-classification
```

## Step 2: Install Dependencies

Ensure you have **Python 3.8+** installed, then run:


```sh
pip install -r requirements.
```

## Step 3: Download the Dataset
Download the dataset from **[Keke Napep (Tricycle) Dataset](https://www.kaggle.com/datasets/ismailismailtijjani/keke-napep-tricycle-dataset)**   and extract it into the project directory.

## Step 4: Run the Application
Start the **Gradio** interface:

``` sh
python app.py
```
The application will launch a web interface where you can **upload and detect KEKE_NAPEP**.

## Step 5: Test with the Dataset
To test the model:

1. **Open the Gradio UI.**  
2. **Upload an image** of a KEKE_NAPEP.  
3. Click **"Submit"** to see the classification result.  

## Collaboration  

As an AI & Computer Vision developer, I recognize the importance of **collaboration** in scaling projects.  
I welcome partnerships with:  
- **Developers & Data Scientists** for improving detection & tracking models  
- **Software Engineers** for integrating models into real-world applications  
- **Domain Experts** in transportation, urban mobility, and security  
- **Organizations** interested in deploying AI-powered transportation analytics  

🚀 If you’re interested in collaborating, feel free to reach out!  

---

## Citation  

The dataset used in this project was provided by **EJAZTECH.AI**, a company dedicated to **gathering local datasets for AI applications**.  

📧 **Contact:** [ejaztech.ai@gmail.com](mailto:ejaztech.ai@gmail.com)  

We acknowledge **EJAZTECH.AI** for their invaluable contributions in providing localized data that played a crucial role in training and validating the **KEKE_NAPEP DETECTION AND TRACKING SYSTEM**.  

---

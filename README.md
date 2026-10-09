# Crop Disease Detection

AI-powered crop disease detection using smartphone images with offline on-device inference and agricultural advisory.

## 📌 Project Overview

This project aims to develop a mobile-based AI system that can help farmers identify crop diseases or pests using a **smartphone camera**.

The farmer will capture a photo of a crop leaf using their existing smartphone. An AI model running on the device will analyze the image and provide a predicted result such as:

- Healthy
- Disease detected
- Possible pest/disease
- Confidence score

The system is designed with **offline usage** in mind, so basic disease detection should work without requiring a continuous internet connection.

An agricultural advisory module will later provide useful information related to the detected disease, such as symptoms, prevention methods, and general management guidance.

---

## 🎯 Project Goals

- Detect crop diseases from smartphone images.
- Use an AI model that can run on a mobile device.
- Support offline disease detection.
- Provide simple and understandable results to farmers.
- Provide offline agricultural advisory information.
- Keep the system lightweight and practical for real-world use.
- Explore deployment on edge/SoC hardware as part of the final prototype.

---

## 🌱 Initial Crop

The initial prototype will focus on:

**Tomato**

Initial disease/health classes:

1. Healthy
2. Early Blight
3. Late Blight
4. Leaf Mold
5. Septoria Leaf Spot

The crop and classes may be expanded or modified as the project develops.

---

## 🏗️ Planned System Architecture

```text
Farmer
   │
   ▼
Smartphone App
   │
   ▼
Smartphone Camera
   │
   ▼
Image Preprocessing
   │
   ▼
On-Device AI Model
   │
   ▼
Disease / Healthy Prediction
   │
   ▼
Offline Advisory Database
   │
   ▼
Result + Agricultural Guidance
```

Internet connectivity may be used later for model/advisory updates, but basic diagnosis is intended to work offline.

---

## 📁 Project Structure

```text
crop-disease-detection/
│
├── ai_model/          # AI model development and training
├── dataset/           # Dataset information and dataset-related files
├── mobile_app/        # Mobile application
├── advisory/          # Agricultural advisory information
├── backend/           # Backend services if required
├── docs/              # Project documentation
├── tests/             # Testing files
│
├── .gitignore         # Files/folders that Git should not track
├── README.md          # Project documentation
└── requirements.txt   # Python dependencies
```

This structure will be updated as the project develops.

---

## 🛠️ Current Development Status

### Phase 1 — Initial Setup

- [x] GitHub repository created
- [x] Repository cloned locally
- [x] Initial project folders created
- [x] Python installed
- [x] Python virtual environment created
- [x] Initial Python packages installed
- [x] `requirements.txt` created

### Phase 2 — Dataset

- [ ] Select suitable dataset
- [ ] Define final disease classes
- [ ] Organize dataset
- [ ] Split dataset into training, validation and testing sets
- [ ] Inspect and clean images
- [ ] Prepare real-world smartphone test images

### Phase 3 — AI Model

- [ ] Select AI framework
- [ ] Select lightweight model architecture
- [ ] Prepare training pipeline
- [ ] Train initial model
- [ ] Evaluate model
- [ ] Generate confusion matrix and performance metrics
- [ ] Improve model accuracy and robustness

### Phase 4 — Mobile Deployment

- [ ] Select mobile development approach
- [ ] Convert/export trained model
- [ ] Integrate model into mobile application
- [ ] Implement smartphone camera input
- [ ] Implement on-device inference
- [ ] Test offline operation

### Phase 5 — Agricultural Advisory

- [ ] Create advisory database
- [ ] Connect disease predictions with advisory information
- [ ] Add prevention and management guidance
- [ ] Implement offline advisory access

### Phase 6 — Testing & Optimization

- [ ] Test with different lighting conditions
- [ ] Test with real smartphone images
- [ ] Test different crop backgrounds
- [ ] Measure inference speed
- [ ] Reduce model size if necessary
- [ ] Improve usability

### Phase 7 — Final Prototype & Edge Deployment

- [ ] Prepare final prototype
- [ ] Document system architecture
- [ ] Explore SoC/edge deployment
- [ ] Optimize model for target hardware
- [ ] Perform final testing
- [ ] Prepare project demonstration

---

## 🐍 Python Environment

The project uses a Python virtual environment to keep project dependencies isolated.

Create the environment:

```bash
python -m venv .venv
```

Activate it on Windows Command Prompt:

```cmd
.venv\Scripts\activate
```

Install the project dependencies:

```bash
pip install -r requirements.txt
```

---

## 📦 Current Python Dependencies

The initial development environment uses Python packages for:

- Numerical computing
- Dataset handling
- Image processing
- Data visualization
- Machine learning evaluation
- Interactive experimentation

The complete dependency list is maintained in:

```text
requirements.txt
```

---

## 🤖 AI Approach

The initial AI approach will be **image classification**.

The model will receive an image of a tomato leaf and predict one of the defined classes.

Example:

```text
Input:
Tomato leaf image

        ↓

AI Model

        ↓

Prediction:
Early Blight

Confidence:
92%
```

After the initial classification system is working, the project may be expanded to more advanced detection or segmentation if required.

---

## 📊 Model Evaluation

The model will not be evaluated using accuracy alone.

The following metrics may be considered:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix
- Inference time
- Model size

Real-world smartphone images will also be used to evaluate how well the model performs outside the training dataset.

---

## 📱 Offline-First Design

A major goal of this project is to allow basic disease detection without continuous internet access.

The intended flow is:

```text
Camera
   ↓
Local Image Processing
   ↓
Local AI Model
   ↓
Prediction
   ↓
Local Advisory Database
   ↓
Result
```

Internet connectivity may be used for future updates, synchronization, or downloading improved models, but it should not be required for the core diagnosis workflow.

---

## ⚠️ Important Note

AI predictions are intended to provide preliminary guidance and should not automatically be treated as a definitive agricultural diagnosis.

Advisory information will be developed carefully and, where applicable, should be verified with reliable agricultural sources or qualified agricultural professionals.

---

## 📚 Documentation

Project documentation will be added progressively as development continues.

Planned documentation includes:

- Dataset documentation
- Model architecture
- Training process
- Evaluation results
- Mobile application architecture
- Offline system design
- Advisory system
- Deployment process
- Edge/SoC deployment
- Testing results

---

## 🚀 Development Approach

This project will be developed incrementally.

The current priority is:

```text
Project Setup
     ↓
Dataset
     ↓
AI Model
     ↓
Model Evaluation
     ↓
Mobile Deployment
     ↓
Offline Advisory
     ↓
Testing
     ↓
Final Prototype
     ↓
Edge/SoC Deployment
```

Each phase will be completed and tested before moving to the next major phase.

---

## 📌 Current Next Step

**Next:** Dataset preparation and selection.

The next phase will focus on obtaining a suitable tomato leaf disease dataset, understanding its classes, organizing the images, and preparing the data for AI model training.

---

## 📄 Project Status

**Status:** Early Development / Initial Setup

This README will be continuously updated as new components are completed.

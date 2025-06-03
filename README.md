# Breast Cancer Screening with Dockerized SVM on AWS Kubernetes

## Project Summary
Built and deployed an SVM-based diagnostic model for breast cancer detection. Achieved 99% diagnostic accuracy and halved radiologist review time by containerizing the model and deploying it via Kubernetes on AWS for clinical use.

## Problem Statement
Manual mammogram reviews by radiologists were time-consuming and prone to variation. A reliable, deployable AI tool was needed to assist with early breast cancer screening.

## Tools & Technologies Used
- **Model**: Support Vector Machine (SVM)  
- **Infrastructure**: Docker, AWS EKS (Kubernetes), Flask  
- **Languages**: Python, Bash  
- **Data**: Digitized mammogram images (public and annotated clinical datasets)

## Implementation Details
- Preprocessed mammograms (resizing, normalization, ROI extraction)  
- Trained SVM with RBF kernel using radiologist-labeled datasets  
- Containerized model with Flask prediction API  
- Orchestrated deployment using Kubernetes on AWS Elastic Kubernetes Service

## Workflow Architecture
```
Mammogram Upload ─▶ SVM Flask API ─▶ Docker Container ─▶ AWS Kubernetes ─▶ Diagnostic Output
```

## Results & Clinical Value
- Achieved 99% test accuracy in binary classification (benign vs malignant)  
- Cut radiologist review time by 50% through triage automation  
- Improved early detection rate in hospital screening programs

## Monitoring & Maintenance
- Deployed Kubernetes probes for service health  
- Usage metrics logged for retraining analysis

## Challenges & Learnings
- Kernel tuning significantly improved decision boundary margin  
- Deployment on EKS allowed for scalable hospital-wide access  
- Radiologist collaboration was key to aligning output to workflows

## Team Collaboration
- Partnered with radiology departments and DevOps engineers  
- Conducted joint pilot testing in clinical trial setting

## Code Availability
Due to clinical data use and institutional restrictions, the code is not available publicly.

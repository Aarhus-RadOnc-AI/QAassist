# QAassist
QAassist: Quality Assurance Assistant for Deep Learning-based GTV Segmentation in Head and Neck 

## Project Description
### Objective
- **QAassist** aims to improve the quality and reliability of deep learning models used in the segmentation of primary gross tumor volume (GTV-T) and involved nodal metastases (GTV-N) for head-and-neck cancer (HNC) patients.

### Challenges Addressed
- Deep learning models, while efficient, are prone to occasional errors and uncertainties, limiting their clinical application.
- The need for a robust mechanism to assess and assure the quality of these models in a clinical setting.

### Core Functionality

#### 1. Advanced Uncertainty Assessment
- Enables users to input probability maps or uncertainty estimations alongside predicted segmentations (masks) and images (e.g., CT, PET, T1w, T2w).
- Incorporates uncertainty estimation methods to provide confidence levels for model predictions, enhancing reliability.

#### 2. Segmentation Accuracy Prediction
- In the absence of uncertainty estimation, QAassist uses provided segmentations and imaging data (which can be singular, like only CT) to predict segmentation accuracy.
- Employs metrics such as DICE, HD95, MSD, or Surface-Dice for accuracy assessment.

#### 3. Quality Assurance
- The primary goal is to predict the segmentation accuracy for quality assurance purposes.
- Facilitates the evaluation of the deep learning model's performance in real-world clinical applications.

#### 4. Flexibility in Data Requirements
- Accommodates incomplete data sets, not requiring all four imaging modalities for functionality.

# GestureMatrix

This project recognizes American Sign Language (ASL) alphabets (A–Z) using deep learning with **EfficientNetB0**, and deploys a **real-time detection app** using **Streamlit + OpenCV** with speech output.

##  eatures
- Train ASL alphabet recognition model with EfficientNetB0 (`model_train.py`)
- Real-time hand gesture recognition (`asl.py`)
- Text-to-Speech support
- Saved trained models (`.keras`)
- Class label mappings (`class_labels.json`)

## Project Structure
```
.
├── asl.py                     # Streamlit real-time detection app
├── model_train.py             # Model training script
├── sign_language_model_fixed.keras
├── best_model.keras
├── class_labels.json
├── training_history.png
├── requirements.txt
└── README.md
```

## Installation
```bash
git clone https://github.com/samarthuttampalle/asl-sign-language.git
cd asl-sign-language
pip install -r requirements.txt
```

## Usage
### Train Model
```bash
python model_train.py
```

### Run Real-time Detection
```bash
streamlit run asl.py
```

## Results
- Accuracy and loss curves saved in `training_history.png`
- Real-time predictions with confidence scores

---
Built with TensorFlow, Streamlit, and OpenCV

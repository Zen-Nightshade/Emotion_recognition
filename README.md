# Emotion Recognition from Voice (RAVDESS Dataset)

This project implements a deep learning-based emotion recognition system using audio data from the [RAVDESS dataset](https://zenodo.org/record/1188976). The primary focus is on leveraging audio features, such as spectrograms and MFCCs, for classifying emotions conveyed in speech.

## Project Highlights

- **Audio-based Emotion Recognition:**  
  Built a pipeline to process raw audio into spectrogram and MFCC representations, enabling effective training of convolutional neural networks (CNNs) for emotion classification.
- **Model Improvements:**  
  - Incorporated Batch Normalization layers for improved training stability and convergence.
  - Integrated ResNet blocks and fine-tuned a pretrained ResNet-18 model to enhance accuracy.
  - Explored and applied various audio data augmentation techniques to improve model generalization.
- **Performance:**  
  Achieved $~70%$ accuracy in the initial CNN-based emotion recognition model on the RAVDESS dataset, later improved to 80% through model improvements.

> **Note:**  
> Some experiments were conducted using recurrent neural networks (RNNs) on transcript data, but this approach was limited by the RAVDESS dataset's low diversity in text samples. The main results and improvements presented here are focused on audio-based emotion recognition.

## Notebooks

- The initial prototype is in `audio_processing.ipynb`.
- Ongoing and main development takes place in `emotion-recognition-system.ipynb`, which includes ResNet blocks, fine-tuning of ResNet-18, and additional improvements.

## Tools & Libraries

- **Programming Language:** Python
- **Deep Learning:** PyTorch, torchvision
- **Audio Processing:** Librosa
- **Image Processing:** PIL
- **Visualization:** Matplotlib
- **Machine Learning Utilities:** scikit-learn
- **(Optional) Speech-to-Text:** Whisper

## Usage

Clone the repository and run the provided Jupyter notebooks. Make sure to install the required libraries. The workflow covers preprocessing of the RAVDESS dataset, audio feature extraction, model training, and results analysis.

---

Feel free to explore the notebooks for detailed implementation and experimentation logs.

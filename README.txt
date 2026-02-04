README - BirdDiff: Bird Call Generation via Enhanced Diffusion Learning

1. Citation
If you use this code, please cite:

    Tianyu Song, Ton Viet Ta,
    Towards High-Fidelity and Controllable Bioacoustics Generation via Enhanced 
    Diffusion Learning.

2. Files
    df_birds.csv                       # Dataset metadata with labels
    model.ipynb                        # Main training notebook
    model_update.ipynb                 # Updated model version
    evaluate_test.ipynb                # Evaluation script
    evaluate_test_update.ipynb         # Updated evaluation
    traditional_augmentation.ipynb     # Comparison

3. Requirements
    Python 3.11+
    PyTorch 2.6.0+
    CUDA 12.5+ (GPU required)

Install dependencies:

    pip install torch torchvision torchaudio numpy scipy librosa

4. Usage
(1) Ensure df_birds.csv is in the same directory as the notebooks

(2) Run training:
    
    jupyter notebook model.ipynb

(3) Run evaluation:
    
    jupyter notebook evaluate_test.ipynb

(4) Compare with traditional augmentation:
    
    jupyter notebook traditional_augmentation.ipynb

5. Dataset
The dataset contains bird call recordings from 12 species:
- Audio format: 22.05 kHz, 2 seconds, single-channel WAV
- Metadata in df_birds.csv includes file paths, labels, and text descriptions

6. Model Overview
Two-stage framework:
(1) Multi-scale Adaptive Enhancement (MABE): Preprocessing
(2) Diffusion Generator: Conditioned on MFCC + category labels + text

See notebooks for implementation details.

7. Contact
For questions or collaboration inquiries, please contact us using the email addresses provided in the published paper.


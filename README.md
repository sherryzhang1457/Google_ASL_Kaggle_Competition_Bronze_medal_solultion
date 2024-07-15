# Google - ASL Fingerspelling Recognition

Competiton website: https://www.kaggle.com/competitions/asl-fingerspelling

The feature extraction was adapted to handle mediapipe landmarks by 1D-CNN. Data augmentations are also performed to regularize the model. 
The encoder has 6 layers (deeper model shows a better result) and a simple decoder with CTC. Training takes are done on TPU which speed up around 3 times.
Inference is done by GPU for submission with TensorFlow-lite 16-bit floating point (FP16).

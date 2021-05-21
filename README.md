# Tacotron2_GST_SparsePitchMatrix
This is our work on learning speaking style in speech synthesis but only using the pitch frequency sub-band as a speaker reference. We trained a modified version of the NVIDIA's Tacotron2 model but including Global Style Tokens (GST). In this work, instead of using the whole log-mel spectrogram representation to train the bank of embeddings, we extracted only the pitch sub-band of all samples and represented them as a binary matrix which we named Pitch Binary Matrix (PBM).  

## Training
Executing MAIN.py training is executed. You just have to change the paths to yours.

## Inference
Executing INFERENCE_SYNTHESIS.py you will generate samples you define inside the script. Remember to also change paths where to save your WAV clips.
Note that WaveGlow model is included, which is cloned from the NVIDIA repository (https://github.com/NVIDIA/waveglow).

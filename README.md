# Clone-Your-Voice

Zero-shot voice cloning notebook powered by [VoxCPM2](https://huggingface.co/openbmb/VoxCPM2), pre-configured for Kaggle with GPU acceleration.

## Overview

Use a short, clean recording of your voice to synthesize any target text into speech using OpenBMB's VoxCPM2 model.

## Quickstart

1. **Open on Kaggle**:
   - Upload `Clone_Your_Voice_VoxCPM2_Kaggle.ipynb` to Kaggle.
   - Set accelerator to **GPU** (T4 / P100).
   - Ensure **Internet** is enabled under Settings (for initial model download).

2. **Add Reference Audio**:
   - Upload a clean, dry recording of your voice (WAV, MP3, etc.) via **Add Input**.
   - Set `REFERENCE_AUDIO` to your audio file path.

3. **Synthesize**:
   - Edit the `TEXT` variable with the script you want to speak.
   - Run the notebook cells sequentially.
   - Download the generated WAV from `/kaggle/working/voice_clones/`.

## Requirements

- Python 3.10+
- `voxcpm`
- `soundfile`
- `huggingface_hub`

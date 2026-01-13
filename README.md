# DemoFace

The collection of Jupyter notebooks and utilities for preparing image data and experimenting with
vision+language models (inference and fine-tuning).

## Quick start
1. Clone the repo:
   ```
   git clone https://github.com/Sufianlab/Demoface.git
   ```
2. Create & activate a virtual environment:
   ```
   python -m venv .venv
   source .venv/bin/activate   # macOS / Linux
   .\.venv\Scripts\activate    # Windows
   ```
3. Install basic dependencies:
   ```
   pip install jupyterlab torch torchvision transformers datasets pillow numpy opencv-python requests
   ```
4. Open notebooks:
   ```
   jupyter lab
   ```

## Requirements
- Python 3.8+
- jupyter / jupyterlab
- torch, torchvision
- transformers, datasets
- pillow, numpy, opencv-python, requests
- Optional (for 8-bit / LoRA training): bitsandbytes, peft, accelerate

## Notebooks (short)
- BLIP_2_inference.ipynb — BLIP-2 style inference examples
- BLIP_2_fine_tuneing.ipynb — fine-tuning with notes on LoRA / 8-bit workflows
- Paligemma_inference.ipynb — PaliGemma-style inference examples
- Paligemma_fine_tuneing.ipynb — fine-tuning pipeline for PaliGemma
- raw_image_downloader.ipynb — download raw demographic images with api
- face_preprocessing_through_cv2.ipynb — preprocessing with OpenCV / PIL

## Dataset format
JSON entry format:
```
{
  "id": "123",
  "image": "path/to/image.png",   // or image bytes
  "Question": "Prompt text",
  "Answer": "Expected answer"
}
```

Ensure image paths are valid and update notebook variables that point to the dataset and image directories.

## Dataset Access Form

You need to submit the Google Form below to get access to the dataset:

👉 **[Dataset Access Google Form](https://forms.gle/BH359sRNFHZX6Szx5)**

## Disclaimer
The rest of the code and files are under construction and will be updated shortly.

## Maintainer & Contact
Maintainer: Sufianlab

GitHub: https://github.com/Sufianlab


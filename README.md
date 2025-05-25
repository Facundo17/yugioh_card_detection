# yugioh_card_detection
This project consists of detecting the types of cards from the Yu-Gi-Oh Card Game.

# The number of types of cards to detect will be only 3:
- Monster
- Spell
- Trap

# Dataset
- 101 images.
- 101 label files.
- labels made on labelImg

# Training
- YoloV11 with google colab.
- 91 training images.
- 10 validation images.
- 60 epochs.
- Time: 0.043 hours.

# yolo_detect.py
- To show the capacity of the card detection.
- Credits to Edje Electronics
- Link to his video: https://www.youtube.com/watch?v=r0RspiLG260&list=LL&index=4
- To execute the script:

```bash
python yolo_detect.py --model model/YuGiOh.pt --source usb0 --resolution 1280x720
```

If you have an NVIDIA card, you can install PyTorch/CUDA to use your graphic card:

```bash
pip install --upgrade torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu128
```
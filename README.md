# Face-Swap-App
Simple face swap app that you could use for fun

## Requirements:
    Python3
    Windows 10

## SETUP:
    1. `pip install virtualenvwrapper-win` to make virtualenvs manageable on Windows
    2. `virtualenv faceswap_env/` to initialize virtualenv
    3. `pip install -r requirements.txt` to install necessary dependencies
    4. `python faceswap.py -h` to view list of options and serves as a test wether dependencies are properly installed

## SETUP Problems: (You might experience this issues)
    1. Issue: No module named 'scandir'
        Fix: `pip install scandir`
    2. Issue: No module named 'scripts.extract'
        Fix: add __ini__.py (could be empty)
    3. Issue: No module named 'face_recognition'
        Fix: `pip install face_recognition`
    4. Issue: CMake must be installed to build the following extensions: dlib
        Fix: @ https://medium.com/@vinuvish/install-dlib-python-windows-77e9349e6cfc

## CHEAT: Preprocessed Data and Pretrained Model
    Since collecting and cleaning data as well as training the model takes so much time and computation. What if we just skip this, and immediately perform face swapping? For this repo, download file at https://anonfile.com/p7w3m0d5be/face-swap.zip. Then extract it.

## How to Face Swap:
    1. `python faceswap.py convert -i face-swap/data/trump/ -o face-swap/output/cage-trump -m face-swap/models/`. The magic of Face swapping cage-trump happens.

## Limitations:
    As of the moment, due to me having less computational power and knowledge. Faceswapping happens only between trump and cage. This is for you to see firsthand the magic of faceswapping without the need of training and preprocessing data.

## Credits:
    -  Code from: https://github.com/llSourcell/deepfakes
    -  Pretrained models from: https://anonfile.com/p7w3m0d5be

# emotion-detection-using-TF

This repository contains a Tensorflow model trained on [FER-2013 dataset](https://www.kaggle.com/msambare/fer2013) for emotion detection.

This dataset consists of 35887 grayscale, 48x48 sized face images with **seven emotions** - angry, disgusted, fearful, happy, neutral, sad and surprised.

## Dependencies

* Python 3, Matplotlib, OpenCV, Tensorflow
* To install the required packages, run  
`$pip install -r requirements.txt`.

## How to use this repo

* First, clone the repository and enter the folder

```bash
git clone https://github.com/Dipeshtamboli/emotion-detection-using-TF.git
cd emotion-detection-using-TF
```

* Then use this saved weights **model.h5** directly for the inference purpose.

```bash
python inference.py --filename img.jpg
```
Here, we need to give the argument for test image name. 
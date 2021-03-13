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

## Algorithm

* First, the **haar cascade** method is used to detect faces in each frame of the webcam feed.

* The region of image containing the face is resized to **48x48** and is passed as input to the CNN.

* The network outputs a list of **softmax scores** for the seven classes of emotions.

* The emotion with maximum score is displayed on the screen.

## Example Output

![Mutiface](sample_images/test_me.jpg)

Here, the sample input image is of the size 4.16 MB and it is till able to detect it.
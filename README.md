# Machine Learning -- Whale recognition

Inspired by the Kaggle competition [here](https://www.kaggle.com/c/happy-whale-and-dolphin/data), I decided to try and create a Machine Learning algorithm capable of identifying marine mammals just by a picture of the dorsal fin. In particular, I used [this dataset](https://www.kaggle.com/datasets/bdsaglam/happy-whale-512?select=sample_submission.csv), that consists of the images of the original dataset with images already resized (hence it is supposedly easier to work with it).

My goal is to build a model from scratches (using an `xresnet34` network) and then comparing it with a pretrained `resnet34`.

For further detail, please look at the ipython notebook.

The `models` folder, contains the model obtained using this algorithm. Sadly, Colab closed unexpectedly right before saving the model obtained with the pretrained model, so it is not in the folder.
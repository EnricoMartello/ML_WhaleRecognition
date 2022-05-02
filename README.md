# Machine Learning -- Whale recognition

Inspired by the Kaggle competition [here](https://www.kaggle.com/c/happy-whale-and-dolphin/data), I decided to try and create a Machine Learning algorithm capable of identifying marine mammals just by a picture of the dorsal fin. In particular, I used [this dataset](https://www.kaggle.com/datasets/bdsaglam/happy-whale-512?select=sample_submission.csv), that consists of the already resized images of the original dataset (hence it is supposedly easier to work with it).

My goal is to build a model from scratches (using an `xresnet34` network) and then comparing it with a pretrained `resnet34`. Once that was done, I unfroze the weights in the pretrained model, and tried a second round of training.

The `models` folder, contains the trained models obtained using this algorithm. Before trying to use Colab, I made an attempt to run the notebook on my laptop, which was a complete failure (e.g. the models in their version 1). 

Next I (wisely) decided to use Colab, that for some reason at first crashed when evaluating summary for the pretrained model (hence there exists no `dorsal_pretrained_resnet34_v2.pth`).

Finally, I was able to follow the whole abovementioned procedure, that led to the determination of the final version of both [models](models/).

## Future development
This is the final project of a 5 week MPAGS course held by Rudo Römer, hence I did it as a beginner, while doing my PhD - please any feedback is much appreciated but be kind :)

As already specified at the end of the notebook, in the future (don't know yet how far this future is) I wanted to try and use a `resnet50` untrained model, and look at the improvements.

## Notes
Note that I used the `kaggle` extension, that is well documented [here](https://www.analyticsvidhya.com/blog/2021/06/how-to-load-kaggle-datasets-directly-into-google-colab/). If you are a beginner, please be smarter than me and use it when using colab: it makes your life much easier.
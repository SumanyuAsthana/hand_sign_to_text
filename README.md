# hand_sign_to_text
5 neural networks I built to categorize videos of hand signs.
This repository contains description and code about 5 neural networks that I built to categorize videos of hand signs.
I have made use of the concept Conv3D LSTM, and transfer learning with models Inception V3 and VGG16.
We have a dataset of 402 videos and the input to each model is of the shape (402, numberOfFrames , resolutionX ,resolutionY ,3) where resolution is the image resolution and numberOfFrames is the number of frames each video is broken into.
The general method is that we first process each image in the dataset i.e. the part which is (resolutionX ,resolutionY ,3) and then we get sequenced data which is (numberOfFrames, processedImages) on which LSTM works.

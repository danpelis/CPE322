# Engineering Design 6 (Iot)

This repository contains the person detection model I trained for my team’s final project in CPE 322. I collected the training images from IMDB and manually marked the people in them using LabelImg. The resulting xml files were then converted into a csv file. Finally, the images and their corresponding csv file were converted in a training.record file, so tensorflow could use it as a training set. A sample config file from the tensorflow repo was modified and used for training. Also, an existing checkpoint file for an SSD Mobilenet was used to decrease training time. The model was then trained and exported with tensorflow. The model was then used in a script by [@cdepalma141](https://github.com/cdepalma141) to detect people in a video feed.

This model was part of a larger system that was meant to first detect a person and then try to identify the person using facial recognition. Slack was also used to send alerts to the user for intruders.

## Links
### I followed steps from the article below:
(He also provided the scripts to convert my training files and i followed the structure of his project for my repo.)

https://towardsdatascience.com/how-to-train-your-own-object-detector-with-tensorflows-object-detector-api-bec72ecfe1d9

### The files I discussed can be found in this repo:
https://github.com/tensorflow/models

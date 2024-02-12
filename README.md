# ASL Recognition
Created by 
- Sparsh Binjrajka, sbinj (at) cs.washington.edu, 
- Duncan Du, wenyudu (at) cs.washington.edu, 
- Aldrich Fan, longxf (at) uw.edu, 
- and Josh Ning, long2000 (at) cs.washington.edu

For a more in-depth look at the project, please navigate to [our website](https://longxf21.github.io/ASL-recognition-dataset/).

## What problem are we trying to solve?

Speech-to-text software exists for many languages around the world and enables us to more-easily communicate with others in the era of digital communication. However, there is a lack of similar technologies for Sign Language. We plan to take a step in solving this by creating a pipeline that detects and identifies the letters of the alphabet in American Sign Language (ASL).

We are creating a machine learning pipeline that detects and identifies the 26 letters of the ASL alphabet in a video or webcam format. There are not many models that have successfully been able to classify signs in real-time. One that did show promising training results turned out to be very biased and did not perform very well when tested by us. As such, we want to create our own dataset to validate and test existing models.

## Existing Works

We found an existing publication on identifying the ASL alphabet using the YOLOv5 model. However, upon further investigation, we were uncertain if the dataset used was trustworthy. The training and testing dataset were taken in the same setting and from similar angles, with most were taken from the same hand. The test result was likely biased and not representative of how the model actually performs. This was further confirmed when we recreated the model and tested it out, getting poor results.

## Methods

The idea behind this was to create a dataset that more closely resembles the environment in which an ASL recognition model might be deployed. We used our dataset to train the YOLOv8 model and, as you can see from the video, it does well for signs that are at a varying distance from the camera and is pretty accurate across all categories. There are a few that don’t quite work well like the letters “M” and “N” but that can be improved.


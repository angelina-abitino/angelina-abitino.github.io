---
layout: project
type: project
image: images/signlanguage.jpg
title: Sign Language Smart Home
permalink: projects/smarthome
# All dates must be YYYY-MM-DD format!
date: 2018-01-17
labels:
  - Microcontroller
  - HTTP
  - Python
  - TensorFlow
  - AI
summary: My goal is to create a smart home system that can recognize commands through sign language.
---

Did you know?
About 500,000 people in the U.S. communicate using american sign language.

American sign language is the 4th most used language in the United States.

Over 90% of deaf children have hearing parents.

Recently, smart home systems have been gaining popularity and are expanding in the kind of tasks they can perform. Even though the current systems have APIs that allow developers to integrate new features, they still rely purely on voice commands. That is why for my senior engineering project I would like to create a smart home system that can take in American Sign Language as commands so that the deaf community can also comfortably utilize smart home systems.

Specifically, I am creating a system that can control a Samsung Hue light with the following commands:
- turn on the light
- turn off the light
- dim the light
- make the light yellow, green, red, or blue
- strobe effect

The AI of my Sign Language Smart Home system is powered with neural networks. I use the pre-trained Inception-v3 convolutional neural net to process spatial features, and a recurrent neural network to process the temporal features.

Here is a schematic of how the system is designed: 
<img class="ui image" src="{{ site.baseurl }}/images/E90schematic.png">

An XBOX Kinect is used as the camera which detects and takes in a video of the signer giving an ASL command. Some computer vision techniques are then used to pre-process the video, and then a series of frames are sent for processing with the dual-network AI system and the predicted command is sent to an Adafruit WiFi shield which communicates through a WiFi Bridge using HTTP protocol to send the command and change the state of the Samsung Hue light.

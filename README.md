# Visual Recognition Automated Emergency Response

Our team tackle the challenge of integrating smart city development of Singapore with crucial and swift resposne to emergency situations such as fire, flooding, traffic accidents, collapse of building and other incidents, using IBM Watson Visual Recognition, we seek to develop an automated and timely response to incidents.

## Contents

1. [Short description](#short-description)
1. [Demo video](#demo-video)
1. [The architecture](#the-architecture)
1. [Long description](#long-description)
1. [Live Demo](#live-demo)
1. [Getting started](#getting-started)
1. [Built with](#built-with)
1. [Authors](#authors)
1. [Acknowledgments](#acknowledgments)

## Short description

### What's the problem?

#### INTEGRATING WITH A SMART ENVIRONMENT

Infrastructure is getting “smart”, with sensors and Internet of things (IoT) increasingly embedded in the built environment (e.g. Punggol Digital District). How might we leverage a network of smart infrastructure in the built environment to make better and more timely sense of emergency incidents (e.g. detection of fires developing, building collapses, falls, road traffic accidents etc.) and to trigger early intervention measures, without the need to activate precious emergency resources?

### How can technology help?

Machine Learning such as IBM Watson Visual Recognition can be trained to detect incidents as they happen in real time via feed from CCTV cameras, and, once detected, can send automated warning to emergency response. This can reduce delay between the incident happening and the response to that incident, leading to early intervention measures.

### The idea

Security cameras, NEA thermal cameras, traffic camera and other cameras in the streets of Singapore can have their feed streamed to the machine learning software trained to detect incidents or any precursors to incidents. Live feed and data from traffic cameras and other cameras is already available publicly such as on [LTA Datamall](https://www.mytransport.sg/content/mytransport/home/dataMall.html). With feeds from cameras across Singapore, we can provide a wide coverage of any instances of incidents occurring. Once an instance is detected, a warning will be sent to the watchroom, along with the image of the camera feed to check the scale and nature of the incident, or to check if it's a false positive.

## Demo video

[![Watch the video](https://www.gannett-cdn.com/-mm-/09608943aa25adf525e933716a119392e8625fb6/c=0-22-773-459/local/-/media/2016/10/22/USATODAY/USATODAY/636127417691080617-YouTube-logo-full-color.png?width=660&height=374&fit=crop&format=pjpg&auto=webp)](https://youtu.be/dlCPb-Vk0Vw)

## The architecture

![Video transcription/translation app](https://i.imgur.com/LAp5XWB.jpg)

1. Security/thermal/traffic camera has feed sent to software.
2. Software with IBM Watson image recognition constantly analyses feed, triggers when an incident is detected.
3. When incident is detected, warning is sent to the watchroom of emergency response, along with feed and location of camera.
4. If the watchroom determines that it's not a false positive, emergency response is sent out.

## Long description

[More detail is available here](https://drive.google.com/file/d/1RsWL1UDfq9W9GvgHDEAoCm1zQr_UQJAU/view?usp=sharing)

## Live Demo

A live demo of the VRAER can be found [here](https://adeelkasban.com/object-detection-live-stream-master/public/index1.html).

## Getting started

Follow these instructions to see a demo of VRAER on your local machine.

### Prerequisites

Install [Node.js](https://nodejs.org/en/download/), [Object Detection Live Stream](https://github.com/cloud-annotations/object-detection-live-stream).

### Step-by-Step

1. Download this repository to your local machine with Node.js and Object Detection Live Stream installed.
2. Copy the 'Public' Folder of this repository to the following folder:

```
C:\Users\(Your username)\object-detection-live-stream\public
```
(If you cannot find that folder, please install Object Detection Live Stream Correctly)

3. Open git Bash, input the following:
```
cd object-detection-live-stream
npm install
npm start
```
4. Enter https://localhost:3000/ to see the live demo.


## Built with

* [IBM Watson Machine Learning](https://www.ibm.com/sg-en/cloud/machine-learning#:~:text=Deploy%20and%20run%20AI%20models,at%20scale%20across%20any%20cloud.) - For object detection in image
* [Node.js](https://nodejs.org/en/) - Server Environment

## Authors

* **Adeel Kasban** - *Developer*
* **Frank Xiao** - *Coordinator*

## Acknowledgments

* Based on [Billie Thompson's README template](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2).

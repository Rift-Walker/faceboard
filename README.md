# FaceBoard
Facial recognition for augmented reality applications.

This project aims to provide a common solution for facial recognition and social network integration.
It is divided into three main parts: a "core" Java library containing common code and business logic, a [Google Cardboard](https://www.google.com/get/cardboard/) app, and a [Google Glass](https://www.google.com/glass/start/) app.

## Core Library
The core of this project will synthesize data from two primary sources:
- OpenCV, running on the device
- Cloud-based services, including:
  - Facebook tagging suggestions
  - Google search results
  - Actual cloud-based facial recognition services?
  - Other social network profiles?

The library will use OpenCV to identify faces in a given frame, and then capture those facial images and hand them to various cloud services, as well as OpenCV's own machine learning algorithms to find the most likely match and provide a data structure containing all the data that could be found on that person.

## Demo Applications
The cardboard application will take input from the camera and overlay facial recognition status and results. A postive match will be indicated by a floating icon near the person's head, which can be expanded to show information

On Google Glass, we will be concerned primarily with the person the user is talking to. A positive match will be indicated by a Glass notification, which can be opened into a more detailed view, which will show a picture and basic information, and can be swiped in various directions to view their social profile feeds.

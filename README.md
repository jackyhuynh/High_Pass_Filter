# High-Pass-Filter

## Introduction
This is a serial of Self-Driving Car technology (the image classifier high pass-filter). This application is extremly helpful to detect edge of Objects and based on that we can 

[Check out video about High pass filter at Udacity.com](https://youtu.be/JOa9ZtV_rB4)

## What exactly is a High-pass Filters?
High-pass filters detect big changes in intensity over a small area, and patterns of intensity can be best seen in a grayscale image.

The filters I’ll be talking about are in the form of matrices, often called convolution kernels, which are just grids of numbers that modify an image. Here is a resource if you'd like to see a wider variety of kernel types in action. Below is an example of a high-pass kernel that does edge detection. It’s a 3x3 kernel, whose elements all sum to zero.

It’s important that, for edge detection, all of the elements sum to 0 because edge filters compute the difference or change between neighboring pixels; they are an approximation for the derivative of an image over space.

![Img](https://github.com/jackyhuynh/High-Pass-Filter/blob/main/images/waymo-gray.jpg)

## High pass Kernal
After apply high pass filter (High pass Kernal):

![Img](https://github.com/jackyhuynh/High-Pass-Filter/blob/main/images/screen-shot-2017-12-18-at-10.54.01-pm.png)

## Convolution
During kernel convolution, the 3x3 kernel is slid over every pixel in the original, grayscale image. The weights in the kernel are multiplied pair-wise around a center pixel, and then added up. This sum becomes the value of a pixel in a new, filtered, output image.

This operation is at the center of convolutional neural networks, which use multiple kernels to extract shape-based features and identify patterns that can accurately classify sets of images. These neural networks are trained on large sets of labelled data, and they learn the most effective kernel weights; the weights that help characterize each image correctly.

Calculating one output pixel value (175) while performing convolution:

![Img](https://github.com/jackyhuynh/High-Pass-Filter/blob/main/images/screen-shot-2017-12-18-at-10.59.26-pm.png)

To handle the edges of images, where the filter cannot exactly overlap, a variety of techniques are used. One of the most common is to extend the edge pixel values of the image out by one and use that to perform a convolution. Another is to pad the image with zeroes, though this creates a darker border in the resulting, filtered image.

## Technology
- Python 
- Jupyter Notebook
- Data Visualization
- Machine Learning
- AI
- Localization
- Prediction
- Open CV

## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites
What things you need to install the software and how to install them
- Jupyter Notebook: If you want just test the code, simply go to google and search for jupiter notebook or another Python online IDE. The Jupyter Notebook is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and narrative text. 
- Anacoda Navigator: Install Anaconda Navigator if you want to develop data sciences using python or R. Anaconda Navigator is a desktop graphical user interface included in Anaconda that allows you to launch applications and easily manage conda packages, environments and channels without the need to use command line commands. 
- OpenCV: OpenCV (Open Source Computer Vision Library) is an open source computer vision and machine learning software library. OpenCV was built to provide a common infrastructure for computer vision applications and to accelerate the use of machine perception in the commercial products. Being a BSD-licensed product, OpenCV makes it easy for businesses to utilize and modify the code. It has C++, Python, Java and MATLAB interfaces and supports Windows, Linux, Android and Mac OS. OpenCV leans mostly towards real-time vision applications and takes advantage of MMX and SSE instructions when available.

### Installing

A step by step series of examples that tell you how to get a development enviroment running

* [Install Anacoda Navigator](https://docs.anaconda.com/anaconda/navigator/install/#:~:text=Installing%20Navigator%20Navigator%20is%20automatically%20installed%20when%20you,install%20anaconda-navigator.%20To%20start%20Navigator,%20see%20Getting%20Started.) - If you haven't downloaded and installed Anacoda Navigator yet, here's how to get started.
* [Jupyter Notebook](https://jupyter.org/try) - Click here to go to the online free Jupiter Notebook.
* [OpenCV](https://opencv.org/)-To run this application we need Open CV installed in the local machine or using anacoda to install Open CV

## Running the tests

Explain how to run the automated tests for this system:
- There is no download IDE need, all you need is download all the src to your machine and run it.
- Using Jupiter Notebook
- Navigate to the file High_Pass_Filter.ipynb
- hit:

```
Ctrl + Enter
```
- The notebook will execute in Markdown form and include some data visualization to show the actual performance of High-pass filter.

## Deployment

The function can be deploy and ready to work with any image. Idea for image recognization for self-driving car sensor.
It turns out that using multiple sensors like radar and lidar at the same time, will give even better results. Using more than one type of sensor at once is called sensor fusion, which is used in Self-Driving Car applications.
Please refer to my notebook for better understanding.

## Built With

* [Jupyter Notebook](https://jupyter.org/try) 
* [Open CV])(https://opencv.org/)

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Truc Huynh** - *Initial work* - [TrucDev](https://github.com/jackyhuynh)

## Format
my README.md format was retrieved from
* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)
See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc


 

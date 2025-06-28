## I. Vision

vision: process by which We capture light through a lens that then emits an electrical signal in our eyes that passes through a cable-like structure (our nervous system), and that signal gets reconstructed to tell us what our surroundings look like in our brains.

To take an image as an input (in this case, the signal captured by our retina) and transform it into information (kicking the ball) is the core of computer vision.


#### Significance of Vision to Humans


#### Pure Programming vs Machine Learning Approach


#### The Motivation Behind Creating Artificial Systems Capable of Simulating Human Vision and Cognition

Computer vision is concerned with developing and understanding algorithms and models in vision systems and their decisions. Used for problems that would be too tedious, time-consuming, expensive, or error-prone for humans to do

Ex:  
- with the popularization of image-to-text and text-to-speech models, we could also make live sports events more accessible for people who have vision disabilities by automatically tracking the ball and its players and describing it in real time. Thus, even simple use cases can have a positive impact on society.


## II. Image


#### Definition of Image

An image is a visual representation of an object, a scene, a person, or even a concept.


One of the more surprising things is that an image is also a function. More precisely, an image is an n-dimensional function. We will first consider it to be two-dimensional n=2. We will call it
F(X,Y), where X and Y are spatial coordinates.


The amplitude of F at a pair of coordinates (x_i,y_i), is the intensity or gray level of the image at that point. The intensity is what gives you the perception of light and dark. Typically, when we have the coordinate pair x_1 and y_1, we refer to them as pixels (picture elements).

- A different type of image is volumetric or 3D images. The number of dimensions in 3D images is equal to three. As a result, we have a F(X,Y,Z) function (x_i, y_i, z_i is called voxel). These images (medical scans, magnetic resonance etc...) can be acquired in 3D; that is, the images are acquired in a way that is reconstructed in a 3D space.  It is also possible to reconstruct a 3D image from a 2D one.


Image channels are simply the different color components that make an image. 

In reference to the F(X,Y), we will have
F for each color component. Each color has its own intensity level. For a channel that picks up the color red, a high intensity means that the color is very red and a low intensity means that there is little to no red in there.


- There are special types of images where the coordinates F(x_i,y_i) do not describe an intensity value, but instead label a pixel. The simplest example of an operation that results in such an image is separating foreground and background. Everything that is foreground receives the label 1, and everything that is background receives the label 0. These images are commonly referred to as labeled images. When there are only two labels, like our example, we call them binary images or masks.

- You may have heard of 4D or even 5D images. This terminology is mostly used by people in the biomedical field and microscopists. The idea is that each new source of information becomes an extra dimension. Thus, a 5D image is a volumetric image (3D) imaged in time (4D) and using different channels (5D).


But how are images represented in computers? Most commonly by matrices. It is easy to picture an image as a 2D numerical array.


- Alternatively, images can be represented as graphs where each node is a coordinate, and the edges are the neighboring coordinates. Take a moment to let that sink in. It also means that the algorithms and models used for graphs can also be used for images! The inverse can also be true - you can transform a graph into an image and analyze it as if it were a picture.



So far, we proposed a rather flexible definition of an image. This definition can accommodate different ways of acquiring visual data, but they all highlight the same crucial aspect: images are data points that contain a lot of spatial information. The key differences are the spatial resolution (either 2D or 3D), their color systems (RGB or others), and whether they have a time component attached to them.



#### Images vs Other Data Types

If you’ve been tuned in, you may have caught on to the idea that videos are a visual representation of images with a time component attached. For 2D image acquisition, you can add a time dimension such that F(X,Y,T) becomes your imaging function.


images and videos differ in how they sample this temporal information. 
- An image is a static representation at a single point in time, while 
- a video is a sequence of images played at a rate (frames per second) that creates an illusion of motion.


#### Images vs Tabular Data





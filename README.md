# Self_Driving_Car
The goal of the project is to train a Deep Neural Network to replicate the human steering behavior while driving, thus being able to drive autonomously on a simulator.
The network takes as input the frame of the frontal camera ( a roof-mounted camera) and will predict the steering direction at each instant.
# Dependencies
* socketio
* eventlet
* numpy
* pandas
* flask
* keras
* Tensorflow
* base64
* io
* openCV
* PIL
* Python 3
* imgaug

For the purpose of simulation and training the neural network, i have used [Udacity simulator](https://github.com/udacity/self-driving-car-sim).
To run this, start simulator in autonomous mode, and run on terminal/cmd ``` python drive_car.py ```

## Dataset
The dataset consists of images (captured from the simulator) and steering angle. [

##  Data preprocessing
*	crop the	image	 
* Convert	RGB	to	YUV	
* Gaussian	Blur 
* Resize	the	image	
* Normalize	the	image	

## Data Augmentation
* After	selecting	the	final	set	of	frames,	we	augment	the	data	by	adding	artificial	shifts	and	rotations to	teach	the	network	how	to	recover	from	a	poor	position	or	orientation.	
* Data	Augmentation techiques :	Zoom,	Width	shift,	Heightshift,	Image	brightness	and	Flipped	image.	
* All	of	these	are	implemented	in	order	to	diversify our dataset so that car moves more acuurately and smoothly.



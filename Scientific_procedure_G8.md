GROUP 8 - BootStrapers
HI!CKATHON 2022  
05/03/2022  

# I.	OVERVIEW

## 1.	Project Background and Description
 	Describe how this project came about, and the purpose.
    
The project aims to detail and quantify one of the major causes of sustainable development: transport. Many employees travel to their workplace by car. As this mode of transport has a high rate of CO2 emissions, it is important to specify its contours in order to propose more effective measurement tools and, ultimately, to provide concrete solutions to reduce the pollution caused by this activity. The project consists of providing companies with a tool enabling them to identify the carbon impact of their employees' travel. 


## 2.	Project Scope
 	 Scope answers questions including what will be done, what won’t be done, and what the result will look like.

Our work can de divided in 3 different parts linked to the three main steps of the tool we have built :

1. bounding box construction & car detection
Using YOLO  the first team identified whether each of the photos provided had a car in its scope and what its coordinates were in the image.

2. car model recognition
The second team used RESNET They trained it on Data_Train and other open source images to build a tool capable of identifying from images where a car is depicted the model of the car.

3.Once the car model has been obtained and thanks to the database provided, our tool can then determine from a single image whether it is a car and if so what its consumption is.



## 3.	Presentation of the group
 	Include your specialization at school, etc.

| First name | Last name | Year of studies & Profile | School        | Skills                 |
| ---------- | --------- | ------------------------- | ------        | ------                 |
| Hugo       | Danet     | M1                        | Telecom       | programming & AI       |
| Remi       | Jaylet    | M2                        | Telecom x HEC       | programming            |
| Zakaria    | Atlassi   | M1                        | HEC           | businness              |
| David      | Wiechmann | M1                        | HEC x Supaero | programming & business |


## 4.	Task Management
 	Describe how you interacted and collaborated as a team, and the effect of every member’s unique background on the project.
    
The varied network of students with different backgrounds, from business schools and engineering schools. In addition, within the engineering schools themselves, each student has a different speciality, which has enabled many synergies to be established.

For part 1 "bounding box construction & car detection" which required work on an already trained neural network -> David Wiechmann student o with basic knowledge in python but without mastering neural network development tools.

For part 2 & 3 "car model recognition" -> Hugo Danet and Remi Jaylet, two students from Telecom Paris, were in charge of training and parameterizing the RESNET model.

The Business Analysis and market projection part was developed by Zakaria Atlassi. He was also responsible for the liaison and knowledge sharing between task 1 and task 2&3.



# II.	PROJECT MANAGEMENT

## 1.	Data Understanding
 	Provided the initial collection of data has already occurred, this step includes identifying and defining the relevant data, exploring the range, scale, formats, contents, and biases of the data, and evaluating the quality and validity of the resulting data.
    
Our focus was to be able to train the most efficiently possible our RCNN to be able to have a powerfull model and being able to identify with great accuracy the model of a given car. For that we decided to train our model with data available online (open-source).

## 2.	Data Pre-processing
 	Explain how the selection of data was manipulated and modified to remove redundant features and improve the quality of the data. Describe the preprocessing techniques used, such as data augmentation.
    
To be able to detect the objects in a given image, we used yolo and only kept the elements that were important for our model afterwards for the recognition. We de dicated much time to this part as the metric seemed to be particularly sensitive to false-positive. This part is particularly accurate and is even quite generalisable to other use case. 

## 3.	Modeling Development
 	Describe how you selected algorithms, how you calibrated them according to the data and how - in fine - you selected the best AI model using a well-defined set of metrics.
    
We elaborated a ResNet model for the recognition of the car models. 

## 4.	 Deployment Strategy
 	What best practices/norms did you follow? How do you plan on deploying your IA solution?
    
We developped everything on Jupyter Notebook (did not used git). 
We tried to create the clearest code possible for the readers.

# III.	CARBON FOOTPRINT LIMITATION
 	Describe the taken measures/actions during the development of your solution in view of limiting the carbon footprint.
As the cars don't have the same emissions, it seem to us necessary to sensibilise people on the choice of their cars and eventually carpooling for the employees working in the same company that are going to work at the same place.

# IV.	CONCLUSION
 	Tell us about the actual results, their limitations as well as future perspectives and improvements.
Our model managed to have significantly good results in a very short time.
We managed to develop a sophisticated model thanks to the augmentation of the dataset that made a rather accurate model.

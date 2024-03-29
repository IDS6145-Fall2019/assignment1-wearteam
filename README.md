# Assignment 1 - Designing Models and Analyzing Data (Template)
(remove: **text between brackets to be removed**)

> * Participant name: Michael Schwartz
> * Project Title: Ticket Kiosk Passenger Flow Simulation

# General Introduction

The first part of this assignment explores designing models (and basic Python/Git features). 

We will look at **subway model in a city** system. A **subway system** is an underground, tube, or metro, underground railway system used to transport large numbers of passengers within urban and suburban areas - modern subways use different types of electronic data collection sensors to supply information which is used to manage assets and resources efficiently. 

The second part of the assignment explores data analysis. Data analysis and visualization is key to both the input and output of simulations. This assignment explores different random number generators, distributions, visualizations, and statistics. Additionally, it will look at getting you accustomed to specifying input and output variables to a system. We will also practice working with real data.


# Part 1: Designing a Model - Subway System


![Image of Subway City System](images/subway_model.png)

## (Part 1.1): Requirements (Experimental Design) **(10%)**
As the world's population increases, consumption of resources also increases. In order to combat climate change, improve air quality and still serve people by transporting them, use of public transportation needs to increase. As public transportation use increases, the problem of queueing in subway systems becomes more severe. The number of queueing events and time spent on each event directly impact the experiences of passengers, which impacts the overall use of public transportation systems.
For this assignment, I chose to use the example of Hangzou Metro Line 1 Wulin Square Station. Yang, Li, and Zhao (2014) indicate that their models show when pedestrian flow rate is at 1500 people/hour, opening two ticket windows is the best solution. When pedestrian flow rate increases to 2500 people/hour, opening four ticket windows is optimal.

The objective for this simulation are to find the optimal set of solutions for pedestrian flow through the subway ticket kiosk area of Wulin Square Station.
Inputs were obtained from Yang, Li, and Zhao (2014). According to the authors between 500 and 2500 passengers use the Wulin Square Station each hour, depending on time of day.
Most passengers do not need to get in a queue for a ticket; however, approximately 15% do. For this simulation, we will presume 15% of 500-2500 passengers need to queue for a ticket.
Wulin Square Station has six ticket windows, but only two to four are used, depending on pedestrian flow rate.
Outputs for this simulation include the average length of queue, time to complete ticket purchase and pass through ticket kiosk area, and ticket kiosk utilization rate.
Necessary functions to analyze this simulation data are calculations for ticket kiosk use rate and average length of queue.

Reference
Yang, Y., Li, J., & Zhao, Q. (2014). Study on passenger flow simulation in urban subway station based on anylogic. Journal of Software, 9(1), 140-146.

## (Part 1.2) Subway (My Problem) Model **(10%)**

(remove: add a high-level overview of your model, the part below should link to the model directory markdown files)
(remove: Look at the [**Object Diagram**](model/object_diagram.md) for how to structure this part of Part 2 for each diagram. Only the Object diagram has the template, the rest are blank. )

* [**Object Diagram**](model/object_diagram.md) - provides the high level overview of components
* [**Class Diagram**](model/class_diagram.md) - provides details of (what are you providing details of)
* [**Behavior Diagram**](model/behavior_diagram.md) - provides details of (what are you providing details of)
* [**Agent / User case** (if appropriate)](model/agent_usecase_diagram.md) - provides details of (what are you providing details of)

## (Part 1.3) Subway (My Problem) Simulation **(10%)**

(remove: Describe how you would simulate this - including type of simulation, rough details, inputs, outputs, and how it will help you analyze your experimental hypothesis, or nullify your null hypothesis.)


## (Part 1.4) Subway City (My Problem) Model **(10%)**
[**Code template**](code/README.md) - Starting coding framework for the (insert your exact problem here.)
You are expected to create the python files - the code should run without errors, create and object(s) for your system, but not provide function detail.



## (Part 1.5) Specifying the Inputs to a System **(10%)**

* IVs: number of passengers per hour, number of available ticket kiosks
DVs: ticket kiosk use rate, average queue length, time to complete ticket purchase process
* Data are from Yang, Li, & Zhao (2014)
* Important statistics to capture: number of passengers per hour at peak and average times, % of passengers who are required to enter the ticket queue, number of available ticket kiosks, total number of ticket kiosks, average length of queue, average time to complete ticket purchase process
* I plan to analyze the model's output in AnyLogic, which follows the methodology of prior research
* I will visualize data with line graphs showing the change over time for various scenarios (i.e., passenger flow rates). The line will represent average queue length or ticket purchase time. The x axis will represent the number of passengers per hour. The y axis will represent the number of available ticket kiosks.
* I will use an infographic to present the data by presenting the average length of queue as stick figures standing along subway tracks that extend horizontally across the page. Each track represents a different number of available ticket kiosks (e.g., line 1 represents 1 window is open, line 2 represents 2 windows are open, etc.). The average time to purchase a ticket is represented by trains that are on the tracks but in the background (the stick figure people are superimposed on the figures of the trains). Above the train tracks are two round analog clocks, one to represent midnight to noon and the other representing noon to midnight. Each clock is divided into 12 parts and in each part is a number that represents the average number of passengers per hour.



# Part 2: Creating a Model from Code

## (Part 2.1) **P**ortable **O**rganic **T**rouble-free **S**elf-watering System (**POTS**) Model **(10%)**
Here [**we provide an overview**](code/POTS_system/README.md) of the **P**ortable **O**rganic **T**rouble-free **S**elf-watering System (**POTS**) Model and provide a source code template for the code found in  [**the following folder**](code/POTS_system/). Please create a **class** diagram of this model (replace the placeholder diagram). (you can use paper and pencil or a digital tool).



# Part 3: Data Analysis

## (Part 3.1) - Real Data **(10%)**

Find a datasource that looks at part of this model - subway stations locations / escalator number, heights, widths / volume of passangers - ridership numbers   (*fits* - we are pretty loose here, it can be anything.)

* Write up a paragraph that describes the data and how it fits into your system.
* Load the data into Python
* Calculate a few useful statistic on the data - keep it simple- STD, means, etc..., this is just designed * to get used to working with real data. Explain the insights you derive from these statistics.
* Visualize the raw data - visualize a few critical aspects of the data to better describe what it is, what it is showing, and why its useful to your system.
* Calculate and plot some summary statistics that better describe the data.

(Add your plots and visualization here)
(Put your data into the data directory)


## (Part 3.2) -  Plotting 2D Random Number Generators **(15%)**

This portion of the assignment looks at generating random numbers in Python and understanding how to properly plot them. Plot two different random numbers, pseudo random and quasi random, for five different N values. There should be 10 subplots, all properly formatted 2D plots. Note, each of the N points will have two coordinates, an x and a y, therefore you will need to generate two random numbers for each point. You should replace the image with your results in a simalar format. Discuss how the patterns differ. Feel free to change the N values from the suggested N values in the image to state your case.



![Image of 2d template City](images/2Dtemplate.png)


## (Part 3.3) -  Plotting 1D Random Distributions **(15%)**

import numpy as np
import scipy.stats
from scipy.stats import truncnorm
import matplotlib.pyplot as plt

x=linspace(0,100,2)
y=exp(-(x-0.5)**2/(2.0*(0.1/(2*sqrt(2*log(2))))**2))

plt.hist(gaussian)
plt.hist(poisson)
plt.show()


X = truncnorm(a=-range/scale, b=+range/scale, scale=scale).rvs(size=size)
X = X.round().astype(int)
Now, choose three different distributions to plot in 1D, or as a histogram. Choose a pseudo-random generator and generate three different distributions. Example distributions are Uniform (part 8), Normal, Exponential, Poisson, and Chi-Squared, but feel free to use any three distributions of your choice. Again, plot each distribution for five different Ns. This will result in 15 different subplots, formatted similar to the image in Part 8. Include your properly formmated 1D plots below and breifly describe what we are looking at and how things change as N is changed.

Repeat the above using a quasi-random generator. Discuss the similarities and differences.

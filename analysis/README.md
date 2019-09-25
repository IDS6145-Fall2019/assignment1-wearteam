## Smart City (My Problem) Simulation

'''
Discrete event simulation is needed to solve this problem. Discrete event simulation is useful for discovering how much
of a resource, or set of resources, a decision maker (in this case, the smart city algorithm) needs to initiate an
action. For the subway queueing simulation, the decision to modify the number of available ticket kiosks is made by
assessing the number of passengers waiting in line to buy a ticket. Agent based simulation is also useful for solving
this problem. Passengers make multiple decisions when purchasing a subway ticket. The first decision is whether or not
they want to ride the subway (based on ticket kiosk wait time). The second decision is which line best helps them reach
their goal (minimizing wait time to buy a ticket). For this simulation we will presume that every passenger intends to
buy a ticket and will pick the shortest available ticket kiosk line.

This simulation type was chosen because the decisions and actions of buying a subway ticket are easily divided into
discrete steps: enter ticket kiosk area, decide to purchase ticket, choose the optimal queue to wait in, enter queue,
wait in the queue, purchase ticket, exit ticket kiosk area.

I would collect data from available inputs, set initial parameters for determining optimal queue length and wait time,
run the simulation, analyze the results, and modify the parameters until an optimal solution was found. I would then
rerun the simulation to determine the optimal solutions for different sets of parameters until realistic use cases were
addressed.
'''

#initialize
import numpy
import cv2
import pygame
from pygame.locals import *

pygame.init()

screen = pygame.display.set_mode((640,447),0,32)

#read image
img = cv2.imread("subway_queue.jpg")

#show image
cv2.imshow("subway_queue.jpg", img)

#close and exit
cv2.waitKey(0)
cv2.destroyAllWindows()

C:\Users\michael\PycharmProjects\assignment1-wearteam\images\subway_queue.jpg
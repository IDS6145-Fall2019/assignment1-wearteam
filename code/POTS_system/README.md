## **P**ortable **O**rganic **T**rouble-free **S**elf-watering System (**POTS**) Model

#initialize
import numpy
import cv2
import pygame
from pygame.locals import *

pygame.init()

screen = pygame.display.set_mode((3024,4032),0,32)

#read image
img = cv2.imread("POTS_model.jpg")

#show image
cv2.imshow("POTS_model.jpg", img)

#close and exit
cv2.waitKey(0)
cv2.destroyAllWindows()

C:\Users\michael\PycharmProjects\assignment1-wearteam\images\POTS_model.jpg
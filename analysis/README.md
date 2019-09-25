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

Inputs to the simulation are number of passengers, number of available ticket kiosks and average time per customer per kiosk. The output is the number of passengers who are able to buy a ticket in under a set period of time (i.e. customers per minute).

This simulation type helps with analysis because it quickly and easily allows for examination of how to optimize a key bottleneck in subway systems. Optimal solutions are arrived at more quickly and inexpensively than randomly trying solutions with real people in a real subway system.
'''

(../images/subway_queue.jpg)
# Travelling Salesman Problem
This repository contains Jupyter Notebooks with solutions for various Travelling Salesman and Route Optimisation Problems. Implementations include:
- Roundtrip for one or multiple salesmen 
- Pickup and Delivery to one location

The problems to be solved are being created on a 100x100 grid with various number of locations. One or more locations are chosen as the start location and one location is chosen as the destination location.

An initial solution to the problem is being created, fulfilling all constraints. Better solutions are being searched with the ruin-and-recreate principle. 
Randomly chosen locations are being removed from the solution (ruin) and locations not part of the solution are being reinserted into the solution (recreate). A new solution is accepted if the objective has improved (e.g., reduction of total distance).

Notebooks termed "Roundtrip" solve problems with one or more salesmen that return to their start location.

Notebooks termed "Pickup_and_Delivery" solve problems where one or more salesmen do a pick up at locations and a delivery to a destination location (e.g., collecting garbage and delivering it to a landfill).

Implemented constraints in Pickup_and_Delivery - all_restriction.ipynb:
- Cost for additional salesmen
- Cost for additional routes
- Cost for missed pickups
- Maximum load per trip
- Maximum travelled distance per salesman

-----
#### Solution for a roundtrip problem with one salesman and 30 locations (one start location)

![Roundtrip](https://github.com/cschweimer/TravellingSalesmanProblem/blob/main/Results/Roundtrip.png)

-----
#### Solution for a Pickup_and_Delivery problem with one salesman and 25 locations (one start and one delivery location)

![Pickup_and_Delivery](https://github.com/cschweimer/TravellingSalesmanProblem/blob/main/Results/Pickup_and_Delivery.png)

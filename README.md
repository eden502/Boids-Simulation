# Boids-Simulation


Boids is an artificial life simulation, originally developed by Craig Reynolds in 1986.
'Boid' is the term Reynolds used to describe a 'Bird-oid' object.
The purpose of this simulation is to present an emergent behaviour of a flock of birds or a school of fish - 
where the complex behaviour of the group arises from the interaction of individuals adhering to a set of 3 simple rules.
The rules are:

<img src="https://user-images.githubusercontent.com/62388816/155971768-4c5b9d0b-429e-4ba9-ba4e-be8bfd269f59.png" width="30%"></img> <img src="https://user-images.githubusercontent.com/62388816/155971789-5e46fc4a-799b-4c7b-b47d-4a4aa2b6256e.png" width="30%"></img> <img src="https://user-images.githubusercontent.com/62388816/155971799-0c911287-901a-49a0-9590-12e048ef04d3.png" width="30%"></img> 


Separation:
  Each bird attempts to maintain a reasonable amount of distance between itself and any nearby birds, to prevent overcrowding.

Alignment:
  Birds try to change their position so that it corresponds with the average alignment of other nearby birds.
  
Cohesion:
  Every bird attempts to move towards the average position of other nearby birds.

In addition to the 3 rules, each boid will only react to other boids within its perception radius - the distance around each boid in which it sees other boids.
  
 The program:
 
 Launching the program will promt a boid count selection - up to 100 boids in a single simulation.
 Each boid is represented by a small gray circle with a straight line pointing out of it.
 The line represents the direction and speed that the boid is moving - longer line = higher speed.
 
 <img src="https://user-images.githubusercontent.com/62388816/155972499-b5d0f811-41e6-4dd1-8bb8-e471bc3539a9.png" width="45%"></img> 
 
After the program starts, the boids will move in random direction at random speeds until the user will apply rules. 
Clicking on each one of the rules will enable/disable it for the entire flock (red means off, green means on).
Additional options are:
  1) P Radius = Perception radius for each boid - increasing it will make each boid interact with more flockmates.
  2) Boundary = Enable/disable boid's ability to move past the edge of the screen.
  3) Clicking on a boid (good luck catching one) will paint it red, and present its perception radius by a large white circle around it.
      The boid will only react to other boids within that circle
      
 <img src="https://user-images.githubusercontent.com/62388816/155973292-66765095-0621-4fbc-95e6-3f321f3f61e5.png" width="45%"></img> 
 
 Running the simulation:
 There are two ways to run the simulation.
 1) If you don't have Processing IDE installed:
    1.1) Download 'Boids Application.zip'
    1.2) Extract 'application.windows'
    1.3) Run 'Boids.exe'
    1.4) Enjoy :)  (Readme file in the zip also explains how to run)
 2) If you have Processing IDE installed:
    2.1) Donwnload Boids.java
    2.2) Import it to a new Processing project
    3.3) Run :)
    
    
    
 
 
 
 
The program was written in Processing ver 4.0b2
  
Imporant notes:
1. This is just my implementation for the idea, there are many impressive implementations out there.
2. It was not written with efficiency in mind - currenly each boid is checking the values of all the other boids in each freme.

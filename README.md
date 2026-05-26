# Solar-System-Simulation
DESCRIPTION
-----------
A 2D solar system simulation built with Python and Pygame.
It models gravitational attraction between planets using Newton's
law of gravitation, and includes a controllable rocket that
responds to thrust and gravity in real time.

This program uses PYGAME, which is a graphics/GUI library and
will NOT run in Ed's online environment.

Required library (outside Python's built-ins):
  - pygame  (graphics and GUI)
 
Install it with:
  pip install pygame

HOW TO RUN
----------
1. Make sure Python 3 and pip are installed on your system.
 
2. Install the required library:
     pip install pygame
 
3. Ensure the following files are all in the SAME folder:
     - main.py          (the main simulation script)
     - background.png   (background image for the space scene)
 
   NOTE: The program will crash if background.png is missing,
   as it is loaded at startup with pygame.image.load().
 
4. Run the program from the terminal:
     python main.py
 
   Or on some systems:
     python3 main.py
 
CONTROLS
--------
  A            - Accelerate rocket (in current direction of travel)
  S            - Decelerate rocket (retrograde thrust)
  M            - Switch between map scenarios (Scenario 1 / 2)
  Z            - Toggle zoom mode
  LEFT arrow   - Cycle camera focus to previous object
  RIGHT arrow  - Cycle camera focus to next object
  UP arrow     - Zoom in (increase scale)
  DOWN arrow   - Zoom out (decrease scale)
  Close window - Quit the simulation
 
 
FEATURES
--------
  - Simulates gravitational attraction between all bodies
  - Planets: Sun, Earth, Mars, Mercury, Venus, Jupiter
  - Controllable rocket affected by gravity and thrust
  - Orbit trails drawn for each body
  - Camera can follow any planet or the rocket
  - Two different map scenarios (press M to switch)
  - On-screen HUD showing speed, thrust state, and camera target
  - Real distance to the Sun displayed per planet (in km)
 
 
NOTES
-----
  - The simulation uses a timestep of 1 day per frame update,
    so orbits evolve quickly.
  - Distances and masses are based on real astronomical values.
  - The rocket's thrust is simplified and not to physical scale.
 

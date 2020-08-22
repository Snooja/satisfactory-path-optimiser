# satisfactory-path-optimiser
Satisfactory Critical Path Optimiser

# Purpose
This repo is intended for a tool which will help you optimising your satisfactory produciton lines.
Example usage would be the user inputs they want to produce 10/min reinforced iron plate.
This tool would split out the resources, buildings, and conveyor belts for this in a graph plot.
In this example this would be
* 120/min iron ore
* 4 smelters producing 120 iron ingots/min
* 8 constructors
    * 3 constructors producing 60 iron plate/min
    * 2 constructors producing 30 pipe/min
    * 3 constructors producing 120 screws/min
* 2 assemblers producing 10 reinforced iron plate/min
* mark 2 conveyor belt required between the 120 screw/min merger output and splitter input

# Development Roadmap
1. Manually optimise a 10/min reinforced iron plate production line using no overclocking
2. Re-do this programatically using either a lookup table or specific class objects
3. Extend and test this to both other production line examples
4. Create a basic graph plot for this using the networkx package
4.1 Use different edge weights to differentiate between 60/min a > 120/min conveyor belts
5. Create a dash or other visualiation web app dashboard interface for this tool
6. Add optimisation for overclocking

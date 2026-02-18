# Visualizing F1 Qualifying Data

Formula One is the highest level of single-seater motorsport racing in the world. Each race weekend follows a structured format that includes 3 practice sessions, a qualifying session, and the Sunday race (Grand Prix). Qualifying is an intense, hour-long event that determines the starting grid for the race. Drivers aim to set the fastest lap to get to start closer to the start line. This means drivers and teams push the cars to the absolute limit, free from the usual race interruptions such as overtaking (cars battling for positions on track) and pit stops (mandatory tire changes during the race).  

I wanted to visualize qualifying speed topographically, where the height represents how fast the car is going at a specific point on the circuit. By studying how speed changes around the track, teams can identify how to change their car setups to excel during qualifying. For example, if a circuit has many tight turns, engineers can tweak the setup of the car to create more “downforce”. Downforce helps to press the tires onto the track, increasing the amount of traction available to the driver and allowing them to take corners at higher speeds. Additionally, the downforce also helps to improve the F1 car’s stability, making it more difficult for the vehicle to spin out of control.

Since official Formula One telemetry data is owned and distributed exclusively by the FIA, I used FastF1, which collects and organizes the read-only live data used by broadcasters for live timings. I picked three circuits from the 2024 season: Miami, USA (5.41 km), Monza, Italy (5.79 km) and Silverstone, UK (5.89km). These tracks were chosen because they have similar lengths but represent very different circuit characteristics. Miami is a modern track with multiple tight corners; Monza is a historic track with a lot of long straights, and Silverstone is a healthy mix of both. I used the FastF1 library to access each circuit’s qualifying session data. From there, I selected the fastest lap from that session and saved both the car’s speed and distance and positional data on the track (X, Y coordinates). Finally, I exported the dataset as a CSV file to work on Mathematica. The same process was repeated twice for the two other tracks. 
## Files Included
- `.ipynb` Jupyter notebook for collecting and cleaning data
- Wolfram/Mathematica code file for making the 3D Objects

## Data Source & Attribution
This project uses data derived from an external GitHub repository and this project does not claim ownership of the source data. All rights belong to the original author(s).  
https://docs.fastf1.dev/


# Handwash - Arctic Fox Blog Solution

<p align="center">
    <img src="https://icii.io/wp-content/uploads/2022/09/New-Arctic-Fox-Logo.Blue_.For-Animation.WithBehindForGaps-1.svg" alt="Arctic Fox Logo" style="width:300px;"/>
</p>

This repo is a tutorial that implements an example handwash sensor. The sensor detects when to run water if either the left or right hand are within the appropriate distance. In this tutorial you will get an introduction to creating a custom automation and using the Calculate automation. 
<br>
<br>
<br>

# Setup
To setup the tutorial, follows these steps: 
1) Fork this repo, **make sure to uncheck main branch only** 
2) Launch the repo in a codespace, wait for the codespace to finish building and extensions finish installing
3) Click the Arctic Fox silhouette on the left, click Activate Arctic Fox on the bottom of the Arctic Fox panel, and enter your Arctic Fox email and password, press Activate (enter not yet supported...) 

# Description
Many designs require setting internal registers, setting gain parameters, and multiplying various values. In this tutorial, we cover a simplified example of this situation.

To motivate the tutorial, we use the example of a handwash sensor that determines when to turn a sink on or off. The sensor:
1. Detects the distance a customer's hands are from the spout
2. Multiplies the distance reading by a gain
3. If the distance * gain is less than a threshold, the water is turned on

# Steps
The tutorial contains the following steps in the following files: 
- Verilog/HandwashSensor.v
  - Steps 1a, 1b, 2, 4, 5
- Automations/HoldWhenAccept.v 
  - Step 3
- Verilog/HandwashSensorTest.v 
  - Step 6

You can run the result in a Verilog simulator. We have included the folder IpCores for simulating in Vivado. 

# View Solution
*Before viewing the solution, make sure you've complete the **Setup*** 

To view the solution, git commit changes on the main branch, and then do: 

> git checkout solution

To go back to the tutorial, do: 

> git checkout main

## Trouble Shooting
If you accidentally make changes to the solution and are having trouble switching back to the tutorial, do an add, then stash, then checkout: 
> git add . 

> git stash 

> git checkout main 

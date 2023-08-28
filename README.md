# dino-jumper

Here's a general outline of how we approached this project:

Hardware Setup:

Place LDRs in strategic positions to detect the presence of obstacles on the screen. You'll need one LDR per obstacle lane. Here, we use two LDRs for two lanes where obstacles can appear. And one LDR as background detector, so a total of three LDRs.
Connect each LDR to an analog input pin on a microcontroller (i.e., Arduino) that will process the sensor data.
Calibration:

Calibrate the LDRs to determine the threshold values for obstacle detection. You'll need to experiment to find the LDR values that correspond to an obstacle being present in each lane.
Microcontroller Programming:

Read the analog values from the LDRs using the microcontroller.
Compare the analog values with the calibrated threshold values to determine if an obstacle is present in each lane.
Control Algorithm:

Implement a decision-making algorithm that determines when to trigger the dinosaur's jump action based on the LDR readings.

Communication with the Game:

Since the Dino Game is a web-based application, you'll need to simulate keyboard input to trigger the dinosaur's jump. 
We use a servo motor to interface the computer by pressing the spacebar key on keyboard mechanically when the control algorithm decides to jump.
Testing and Refinement:

Test the system with the Dino Game and observe how well it performs. Adjust the threshold values, the control algorithm, and other parameters as needed to ensure accurate obstacle detection and reliable jumping.
Fine-Tuning:

This step might involve iteratively refining the calibration and algorithm to make the automated jumping more accurate and responsive.
Technology Used:  Arduino

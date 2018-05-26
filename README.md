# SDCND_Term2_EKF
## Extended Kalman Filter Project
A Kalman filter is used to estimate the state of a moving object of interest with noisy lidar and radar measurements. 
- Here the RMSE values are lower than the tolerance value mentioned in the project rubric. 

This project involves the Term 2 Simulator which can be downloaded [here](https://github.com/udacity/self-driving-car-sim/releases)
Follow the instructions preesent in the classroom section 'uWebSocketIO Starter Guide' for the environment setup.

Once the install for uWebSocketIO is complete, the main program can be built and run by doing the following from the project top directory.
1. mkdir build
2. cd build
3. cmake ..
4. make
5. ./ExtendedKF

## Run the Project:
1. Clone this repo.
2. Make a build directory: `mkdir build && cd build`
3. Compile: `cmake .. && make` 
   * On windows, you may need to run: `cmake .. -G "Unix Makefiles" && make`
4. Run it: `./ExtendedKF `

INPUT: values provided by the simulator to the c++ program
["sensor_measurement"] => the measurement that the simulator observed (either lidar or radar)

OUTPUT: values provided by the c++ program to the simulator
["estimate_x"] <= kalman filter estimated position x
["estimate_y"] <= kalman filter estimated position y
["rmse_x"]
["rmse_y"]
["rmse_vx"]
["rmse_vy"]

Then run the project from the build directory on the sample data files using:
./ExtendedKF ../data/obj_pose-laser-radar-synthetic-input.txt ../output/output1.txt

## Result
The result for the input file 'obj_pose-laser-radar-synthetic-input.txt' is
RMSE
X: 0.0961
Y: 0.0862
VX:0.4493
VY:0.4069
The output is available in file output\output1.txt
The output plot is shown in Output_obj_pose-laser-radar-synthetic-input.JPG present in 'output\Output_obj_pose-laser-radar-synthetic-input.JPG'

I have not committed the complete Eigen folder. The codes are available in classroom example Git project repository.





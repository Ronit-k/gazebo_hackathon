# gazebo_hackathon

### This provides a solution to Robotics Simulation Challenge : <a href = https://drive.google.com/file/d/15DJpeVqscW1H3fR2jJF_0PlTyiXfsDqr/view>Problem Statement</a>

To see the simulation in action follow the following steps:

(run roscore in the background)

Clone this repo on to your system:   
``` git clone https://github.com/Ronit-k/gazebo_hackathon.git```

go to the workspace ***Robotic_Arm***   
``` cd gazebo_hackathon/Robotic_Arm ```

build the workspace   
``` catkin build ``` 
> *if any warnings appear, try to build again

source the setup file   
``` source devel/setup.bash ```

to see the robotic arm in an empty gazebo world   
``` roslaunch src/robot_arm_urdf/launch/arm_urdf.launch```

to see the robotic arm in the ***demo_world***, provided      
``` roslaunch src/robot_arm_urdf/launch/gazebo_demo_world.launch```

<hr>

Now to see the simulation in action, first make the python script **pick_place.py** executable  
``` sudo chmod +x src/moveit_robot_arm_sim/scripts/pick_place.py ```

then   
``` roslaunch src/moveit_robot_arm_sim/launch/full_robot_arm_sim.launch ```
and on to a new terminal window, execute the python script      
``` src/moveit_robot_arm_sim/scripts/pick_place.py ```

<a href="https://drive.google.com/file/d/1NDSAC670Lq5m8mmNqCxAuCifo4bfoWCK/view?usp=sharing/view">click here</a> to see the simulation

# Robotics_Project3
This is a demonstration of the AMCL algorithm by using the amcl ROS package

To execute the Project:

1. Clone the Repository Folder "Robotics_Project3" to your /home/<user> directory

        cd ~
        git clone https://github.com/andreslc47/Robotics_Project3.git

2. Enter to the folder: 

        cd ~/Robotics_Project3/
  
3. Compile the Workspace by using the script provided:

        ./compile_all
 
4. Copy the default.rviz file to rviz directory (You might replace the existing one):

        cp default.rviz /opt/ros/kinetic/share/rviz

5. Open 4 terminals.

    5.1. First Terminal: 

        cd ~/Robotics_Project3/
        source devel/setup.bash
        roslaunch my_robot world.launch
  
    5.2. Second Terminal:

        cd ~/Robotics_Project3/
        source devel/setup.bash
        roslaunch my_robot amcl.launch

    5.3. Third Terminal:

        cd ~/Robotics_Project3/
        source devel/setup.bash
        rviz

    5.4. Fourth Terminal:

        cd ~/Robotics_Project3/
        source devel/setup.bash
        rosrun teleop_twist_keyboard teleop_twist_keyboard.py

6.  Move the robot by using the keys indicatd by teleop_twist_keyboard.

7. To close Gazebo and RViz:
  
        cd ~/Robotics_Project3/
        ./pkill_all

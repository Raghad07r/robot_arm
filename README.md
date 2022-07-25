# robot_arm

ROS packages that can be used to plan and execute motion trajectories for a robot arm in simulation and real-life.

## Dependencies
run this instruction inside your workspace:

```$ rosdep install --from-paths src --ignore-src -r -y```

make sure you installed all these packages:

 melodic distro

```
$ sudo apt-get install ros-melodic-moveit
$ sudo apt-get install ros-melodic-joint-state-publisher ros-melodic-joint-state-publisher-gui
$ sudo apt-get install ros-melodic-gazebo-ros-control joint-state-publisher
$ sudo apt-get install ros-melodic-ros-controllers ros-melodic-ros-control
```
<img width="960" alt="2022-07-22 (8)" src="https://user-images.githubusercontent.com/107891623/180715127-00ebdd50-33b6-49ea-b4cf-9a855e015734.png">
<img width="960" alt="2022-07-22 (9)" src="https://user-images.githubusercontent.com/107891623/180717334-16543a80-9313-4149-9eca-f19fd9c14383.png">

Configuring Arduino with ROS

- Install Arduino IDE in Ubuntu
https://www.arduino.cc/en/software
to install run ```$ sudo ./install.sh``` after unzipping the folder

- Launch the Arduino IDE

- Install the arduino package and ros library
http://wiki.ros.org/rosserial_arduino/Tutorials/Arduino%20IDE%20Setup

- Make sure to change the port permission before uploading the Arduino code
```$ sudo chmod 777 /dev/ttyUSB0```

### Controlling the robot arm by joint_state_publisher
```$ roslaunch robot_arm_pkg check_motors.launch```

### Controlling the robot arm by Moveit and kinematics
```$ roslaunch moveit_pkg demo.launch```

![raghad html](https://user-images.githubusercontent.com/107891623/180715230-a78a9e23-1baf-49e3-99ff-c939f009e44c.jpeg)

###The result

![image](https://user-images.githubusercontent.com/107891623/180716403-d8944ae0-20be-41c1-99bf-406895954da3.png)

![image](https://user-images.githubusercontent.com/107891623/180716264-306b03ac-7e5a-4232-902b-709c25b45ce6.png)

![image](https://user-images.githubusercontent.com/107891623/180716234-6f060c37-1477-4b80-9e3b-82fdfaf0ca68.png)



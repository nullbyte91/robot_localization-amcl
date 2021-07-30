## Where Am I? - Udacity - Robotics Software Engineer Nanodegree Program - Project Three

### Demo Videos
| 👉 [Where Am I](https://youtu.be/M7n_G1pHcQw) |
| ------------------------------------------------------------ |
| [![Where Am I Demo](https://github.com/nullbyte91/robot_localization-amcl/blob/master/images/udacit_p3.png)](https://youtu.be/M7n_G1pHcQw) |


### 🗃 Project structure
```python
.
├── images
│   └── udacit_p3.png
├── my_robot
│   ├── CMakeLists.txt
│   ├── config
│   │   ├── base_local_planner_params.yaml
│   │   ├── costmap_common_params.yaml
│   │   ├── global_costmap_params.yaml
│   │   ├── local_costmap_params.yaml
│   │   └── __MACOSX
│   ├── launch
│   │   ├── amcl.launch
│   │   ├── robot_description.launch
│   │   └── world.launch
│   ├── maps
│   │   ├── my_robot.pgm
│   │   └── my_robot.yaml
│   ├── meshes
│   │   └── hokuyo.dae
│   ├── model
│   │   └── ball
│   │       ├── model.config
│   │       └── model.sdf
│   ├── package.xml
│   ├── rviz
│   │   └── my_robot_config.rviz
│   ├── urdf
│   │   ├── my_robot.gazebo
│   │   └── my_robot.xacro
│   └── worlds
│       ├── empty.world
│       ├── test_world.world
│       ├── UdacityOffice_withball.world
│       └── UdacityOffice.world
├── pgm_map_creator
├── README.md
└── teleop_twist_keyboard]
```

### 🖖 Quick Start
```bash
mkdir -p catkin_ws/src && pushd catkin_ws/src
git clone https://github.com/nullbyte91/robot_localization-amcl.git
cd ..

# Build package
catkin_make

# Terminal 1
source devel/setup.bash
roslaunch my_robot world.launch

# Terminal 2
source devel/setup.bash
roslaunch my_robot amcl.launch

# Provide navigation goal from RVIZ
```



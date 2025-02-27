# TurtleBot3
This is a custom package for TurtleBot3 to experiment with navigation algorithms such as [simple_planner](https://github.com/datledoan/simple_planner) and [regulated_pure_pursuit_controller](https://github.com/datledoan/regulated_pure_pursuit_controller_ros) in simulation.

# Build and run
- Install move_base_flex
    ```sh
    sudo apt install ros-noetic-mbf-costmap-nav
    ```
- Clone and build [simple_planner](https://github.com/datledoan/simple_planner) and [regulated_pure_pursuit_controller](https://github.com/datledoan/regulated_pure_pursuit_controller_ros). If you want to use another global_planner or local_planner, modify the configurations in `turtlebot3/turtlebot3_navigation/param/default_planner.yaml` and `turtlebot3/turtlebot3_navigation/param/move_base_flex.yaml`
- Build and run:
    ```sh
    cd your_ws/src
    git clone https://github.com/datledoan/turtlebot3
    cd ..
    catkin build
    source devel/setup.bash
    roslaunch turtlebot3_navigation turtlebot3_navigation.launch
    ```

# Document
- [ROBOTIS e-Manual for TurtleBot3](http://turtlebot3.robotis.com/)
- [turtlebot3](https://github.com/ROBOTIS-GIT/turtlebot3)


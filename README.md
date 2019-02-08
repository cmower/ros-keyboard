# ros-keyboard

Simple keyboard driver for ROS using Pygame.

# Usage

Clone `ros-keyboard` repository to your catkin workspace using 
```
  $ git clone git@github.com:cmower/ros-keyboard.git keyboard
```

Add the following to your launch file.
```
	<include file="$(find keyboard)/launch/keyboard.launch"/>
```
By default the keyboard node runs at 100Hz. If you would like to change this to 150Hz (for example), then use
```
	<arg name="keyboard_hz" value="150"/>
	<include file="$(find keyboard)/launch/keyboard.launch" pass_all_args="true"/>
```


# Requirements

* Pygame, see [here](https://www.pygame.org/news), `$ pip install pygame`. 

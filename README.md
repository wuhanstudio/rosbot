## ROSBot

### Build


```
$ sudo apt-get install ros-noetic-desktop-full ros-noetic-teleop-twist-keyboard
```

```
$ cd catkin_ws/src
$ git clone https://github.com/wuhanstudio/rosbot
$ cd ..
$ rosdep install --from-paths src --ignore-src -r -y
$ catkin_make
$ source devel/setup.sh
```

### Lane Tracking

```
$ roslaunch rosbot lane.launch
```

![](docs/lane.png)

### Small Office

```
$ roslaunch rosbot office.launch
```

![](docs/office.png)

### Small Town

```
$ . /usr/local/share/citysim/setup.sh
```

```
$ roslaunch rosbot city.launch
```

![](docs/city.png)


### Control

```
$ rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```

# ros_erle_takeoff_land

if you are using mavros 0.12 use the branch `mavros0.12`

```
git checkout mavros0.12
```

## Compile

```
mkdir -p takeoff_land_ws/src && cd takeoff_land_ws/src
git clone https://github.com/erlerobot/ros_erle_takeoff_land
cd ..
catkin_make_isolated --pkg ros_erle_takeoff_land
```

## How to use it

```
source takeoff_land_ws/devel_isolated/ros_erle_takeoff_land/setup.bash
rosrun ros_erle_takeoff_land ros_erle_takeoff_land
```

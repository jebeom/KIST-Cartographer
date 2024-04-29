# KIST-Cartographer

I have created a 2D map by merging data from two LiDARs mounted on a mobile manipulator platform, as shown in the diagram below. You can modify the lua file and launch file appropriately to not only create a 2D map but also a 3D map.

and you will need the cartographer and cartographer_ros packages, so please install them based on the [this link](https://google-cartographer-ros.readthedocs.io/en/latest/compilation.html)

## How to make 2D map

```
roslaunch cartographer_ros moma_2d.launch
```

You can see the map being created by adding the **map topic** to Rviz.

## How to save the map
Once the map is complete, you can save it using the command below.

```
rosrun map_server map_saver -f /path/to/your/file/(file_name)
```

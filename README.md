Please follow directions specified on each submodule.
To launch the demo, execute each command on a new terminal:
````
$ roslaunch trikey_dreamer dreamer_gazebo.launch
$ ROS_NAMESPACE=stereo rosrun stereo_image_proc stereo_image_proc
$ rosrun image_view stereo_view image:=image_raw _approximate_sync:=True
````

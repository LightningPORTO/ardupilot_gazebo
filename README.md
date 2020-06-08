## bashrc :
````
echo 'source /usr/share/gazebo/setup.sh' >> ~/.bashrc
echo 'export GAZEBO_MODEL_PATH=~/ardupilot_gazebo/models' >> ~/.bashrc
echo 'export GAZEBO_RESOURCE_PATH=~/ardupilot_gazebo/worlds:${GAZEBO_RESOURCE_PATH}' >> ~/.bashrc
````
##### COPTER

On 1st Terminal
````
sim_vehicle.py -v ArduCopter -f gazebo-iris --map --console
````

On 2nd Terminal

````
cd ardupilot_gazebo/worlds
gazebo iris_arducopter_runway.world
````

##### VTOL

On 1st Terminal
````
sim_vehicle.py -v ArduPlane -f gazebo-quadplane --console
````

On 2nd Terminal

````
cd ardupilot_gazebo/worlds
gazebo vtol_arduplane_runway.world
````


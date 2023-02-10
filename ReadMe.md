# Snake Model
The Repository gives model of snake robot with 7 joints.
## Model information
Each consecutive joint is pi/2 out of phase from previous joint.
Thus all the odd number of joints are in one plane and all even joints are in one plane.

Quick table of model description
|parameter          | Value                              |
|-------------------|------------------------------------|
| Degree of freedom | 7(joints)+3(position of base link) |
| Number of joints  | 7                                  |
| number of links   | 8                                  |
| Nature of joints  | revolute                           |

Information for axis of all joints and links is in the image below
![snake_axis_image](https://github.com/marneneha/snake_model/blob/master/image_of_snake_model.png)
All the joints are revoluts joints with motion describe below
![snake_model_motion](https://github.com/marneneha/snake_model/blob/master/sname_model_gif.gif)
## Prerequisite

- OS: Unbuntu 
- ROS
- Gazebo(Inbuilt in Ubuntu)
## How to run
- Clone
   - Either clone the Repository in the catkin workspace using the command
   ```
   git clone https://github.com/marneneha/snake_model.git
   ```
   OR
   - Create a catkin workspace and clone the repository in the src folder using following command
   
   ``` 
    mkdir –p ~/catkin_ws/src
    cd ~/catkin_ws/src
    git clone https://github.com/marneneha/snake_model.git
    ```
- Build and source
```
    cd ~/catkin_ws/
    catkin build snake
    source devel/setup.bash    
```
- Launch
```
roslaunch snake template_launch.launch
```
You should see following result
## Result
![](https://github.com/marneneha/snake_model/blob/master/Result_launch%20_of_snake_model_repo.png)
This repository only contains model and you can build your own planner and controller over it.  Implementation of snake motion can be found [here](https://github.com/marneneha/snake)

[^1]: Project credits: Neha Marne, Fabrizzio Coronado
[^2]: Software used: Solidworks and sw2ref
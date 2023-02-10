The Repository gives model of snake robot with 7 joints.
Each consecutive joint is pi/2 out of phase from previous joint.
Thus all the odd number of joints are in one plane and all even joints are in one plane.

Quick table of model is given below
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

This repository only contains model and implementation of snake motion can be found here

Project credits: Neha Marne, Fabrizzio Coronado
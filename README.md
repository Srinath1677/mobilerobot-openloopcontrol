# MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure

## Step1:
Use from robomaster import robot

<br/>

## Step2:
Choose the x,y,z - axis movement distance(meters)

<br/>
## Step3:
Give ep_chassis.move to move straight.


<br/>
## Step4:
Give time.sleep() for a break

<br/>
## Step5:
Give ep_chassis.drive_speed to have a circular movement.

<br/>

## Program
```python
from robomaster import robot
import time
from robomaster import camera
if _name_ == '_main_':
ep_robot = robot.Robot()
ep_robot.initialize(conn_type="ap")
ep_chassis = ep_robot.chassis
ep_led = ep_robot.led
ep_camera = ep_robot.camera
print("Video streaming started.....")
ep_camera.start_video_stream(display=True, resolution = camera.STREAM
ep_chassis.move(x=2.5, y=0, z=0, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=0,g=255,b=255,effect="on")
ep_chassis.move(x=0.5, y=0, z=80, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=255,g=100,b=0,effect="on")
ep_chassis.move(x=1.0, y=0, z=0, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=150,g=150,b=150,effect="on")
ep_chassis.move(x=0, y=-1.5, z=0, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=150,g=150,b=150,effect="on")
ep_chassis.move(x=0, y=0, z=-118, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=150,g=150,b=150,effect="on")
ep_chassis.move(x=-1.6, y=0, z=0, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=150,g=150,b=150,effect="on")
ep_chassis.move(x=0, y=0, z=-45, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=150,g=150,b=150,effect="on")
ep_chassis.move(x=0, y=1.5, z=0, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=150,g=150,b=150,effect="on")
ep_chassis.move(x=2.1, y=0, z=0, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=150,g=150,b=150,effect="on")
ep_chassis.move(x=0, y=0, z=84, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=150,g=150,b=150,effect="on")
ep_chassis.move(x=0.6, y=0, z=0, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=150,g=150,b=150,effect="on")
ep_chassis.move(x=0, y=0, z=0, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=150,g=150,b=150,effect="on")
time.sleep(4)
ep_camera.stop_video_stream()
print("Stopped video streaming.....")
ep_robot.close()
```

## MobileRobot Movement Image:

![robo](./img/robomaster.png)

Insert image here


<br/>
<br/>
<br/>
<br/>

## MobileRobot Movement Video:

Upload your video in Youtube and paste your video-id here

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](https://www.youtube.com/watch?v=YOUTUBE_VIDEO_ID_HERE)

<br/>
<br/>
<br/>
<br/>

## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.


<br/>
<br/>

```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```

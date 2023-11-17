# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
Program Developed By: Mahalakshmi.K
Register Number: 212222240057
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
  pos=[[1,30],[2,40],[3,90]]
  robot = getRobot()
  robot.driveJoints(0,0,0,0,0,0)
  delay(5)
  for i in pos:
    robot.Controller.moveJoint(i[0],i[1])
    delay(5)

## Output
### 1. Generic Articulated Robot

![g](https://github.com/maha712/Movement-of-Robot-Joints/assets/121156360/d45126b5-b155-4c40-bd32-5ab5646d52b6)


### 2. robot.driveJoints(0,0,0,0,0,0)

![WhatsApp Image 2023-11-01 at 8 04 45 AM (1)](https://github.com/maha712/Movement-of-Robot-Joints/assets/121156360/1d9109a1-f6c5-4f91-a392-5fda3dd5ef0d)

### 3. Movement of Joint1

![WhatsApp Image 2023-11-01 at 8 04 45 AM (2)](https://github.com/maha712/Movement-of-Robot-Joints/assets/121156360/4be94d4b-fb95-41cc-8cb6-47bb307068db)

### 3. Movement of Joint2

![WhatsApp Image 2023-11-01 at 8 04 45 AM (3)](https://github.com/maha712/Movement-of-Robot-Joints/assets/121156360/60c98c36-380c-41aa-b6ea-1e21b1b1706b)

### 3. Movement of Joint3

![WhatsApp Image 2023-11-01 at 8 04 45 AM](https://github.com/maha712/Movement-of-Robot-Joints/assets/121156360/75e0cfb0-6ca2-4762-8264-59713ccd27c3)


## Result 
Thus the different robots joints are moved with the help of python list.



# ispy_robot

This code allows a NAO robot to inspect the area in front of it, segment each object from the background, and keep track of the position of the object in space. The code also saves images of each object as it moves across the robot's field of vision.

## Demo
Click the link or video below to watch the demo. The robot looks around and points to each object, naming its color.
<a href="http://www.youtube.com/watch?feature=player_embedded&v=wSN6pFF994I
" target="_blank"><img src="http://img.youtube.com/vi/wSN6pFF994I/0.jpg" 
alt="Robot Demo" width="480" height="360" border="10" /></a>

https://www.youtube.com/watch?v=wSN6pFF994I

## About

This is a collection of modules for NAO robots that are required for the iSpy game in the HiLT lab. More info: https://github.com/iamadamhair/ispy_python

These files are intended to reside in `~/modules/`

In order to load them, you must edit the file `~/naoqi/preferences/autoload.ini` file to include the modules under the `[python]` section, e.g.:

    [python]
    /home/nao/modules/segmentation_module.py
    /home/nao/modules/sound_receiver_module.py

Because NAO robots do not have Git, you may install this repository with the following commands. Please note that you will have to edit `autoload.ini` manually.

    rm -rf modules/
    wget -O modules.zip https://github.com/jacobbrunson/ispy_robot/archive/master.zip
    unzip modules.zip
    mv ispy_robot-master/ modules/
    rm modules.zip

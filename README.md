# lane following
This is the lab assignment 4 for SUSTech EE346. My SID: 11813118.

# Usage

## 1. Clone the source code
  cd ~/catkin_ws/src
  
  git clone https://github.com/XeonCn/lane_following.git
  
## 2. Catkin make the lane following package
  cd ..
  
  catkin_make

## 3. Add course models
   export GAZEBO_MODEL_PATH=${GAZEBO_MODEL_PATH}:~/catkin_ws/src/lane_following/models
   
## 4. Launch the gazebo map
   source ~/catkin_ws/devel/setup.bash
   
   roslaunch lane_following race_track.launch 

## 5. Run lane following python node
   
   cd ~/catkin_ws/src/lane_following/scripts/
   
   chmod +x lane_following_part1.py lane_following_part2.py lane_following_part3.py
   
   cd ~/catkin_ws
   
   source devel/setup.bash
   
   sudo pip install opencv-contrib-python
   
   rosrun lane_following lane_following_part1.py
   
   or rosrun lane_following lane_following_part2.py
   
   or rosrun lane_following lane_following_part3.py

 ![image](https://github.com/zhaojieting/linefollowing/blob/main/data/demo.gif)

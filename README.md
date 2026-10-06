# Camera_Manual_MindCloud

## Cameras in Robotics :

Cameras are important sensors in modern robotics. They allow robots to observe their surroundings and collect visual information about objects, people, surfaces, obstacles, and environments.

Robot cameras can be used for tasks such as object detection, navigation, inspection, measurement, manipulation, mapping, and human-robot interaction. Different robotic applications require different types of cameras depending on lighting, distance, accuracy, speed, and environmental conditions.


## How Camera Works ?

In general, different types of cameras operate on a similar principle: light reflected from an object is captured and converted into information (color intensity), which can then be processed by a computing unit. Structurally, this processing unit may be integrated into the camera or housed externally.

**if the point cloud tells** 
**you Could not transform from [oakd_depth] to [base_link]**

**here put an image**

First Check the tf Transform is not broken between the fixed frame and the camera frame 

✅ 🔥 FIX #1: Add Static Transform

ros2 run tf2_ros static_transform_publisher 0 0 0 0 0 0 base_link oakd_depth

✅ 🔥 FIX #2: Set RViz Fixed Frame

set the camera frame or the base_link 

ros2 run tf2_tools view_frames

base_link → oakd_depth

ros2 topic echo /points2 --once

**here put an image**


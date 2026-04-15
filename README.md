# Camera_Manual_MindCloud

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


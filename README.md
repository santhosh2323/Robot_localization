# Robot_localization
The Repository contains workspace and algorithms to integrate imu and gps data from kitti/oxts dataset to EKF &amp; UKF node for benchmark analysis

# INTEGRATION

    git clone https://github.com/santhosh2323/Robot_localization.git
    Inside the Robot_localization Folder find the compressed robot_localization.zip file
    Unzip and place it inside your ROS workspace/src folder
    compile your workspace using catkin_make

# RUNNING

    TO RUN EKF:
      roslaunch robot_localization ekf_complete.launch
      
      which contains --- rviz 
                         ekf.launch - ekf node
                         navsat.launch - navsat node
                         rviz plotter.py -for plotting trajectory in rviz
                         ground_truth_plotter.py - for plotting ground truth trajectory
                         filtered_odom_plotter.py - for plotting filtered odom trajectory
                         rosbag node - for playing rosbag of dataset

    TO RUN UKF:
      roslaunch robot_localization ukf_complete.launch
      
      which contains --- rviz 
                         ukf.launch - ekf node
                         navsat.launch - navsat node
                         rviz plotter.py -for plotting trajectory in rviz
                         ground_truth_plotter.py - for plotting ground truth trajectory
                         filtered_odom_plotter.py - for plotting filtered odom trajectory
                         rosbag node - for playing rosbag of dataset
                         
      

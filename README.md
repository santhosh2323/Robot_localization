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
                         ekf.launch - for launching ekf node
                         navsat.launch - for launching navsat node
                         rviz plotter.py - for plotting ground_truth & filtered/odom trajectories in rviz
                         ground_truth_plotter.py - node for plotting ground truth trajectory
                         filtered_odom_plotter.py - node for plotting filtered odom trajectory
                         rosbag node - for playing rosbag of dataset

    TO RUN UKF:
      roslaunch robot_localization ukf_complete.launch
      
      which contains --- rviz 
                         ukf.launch - for launching ukf node
                         navsat.launch - for launching navsat node
                         rviz plotter.py -for plotting ground_truth & filtered/odom trajectories in rviz
                         ground_truth_plotter.py - node for plotting ground truth trajectory
                         filtered_odom_plotter.py - node for plotting filtered odom trajectory
                         rosbag node - for playing rosbag of dataset

# OUTPUT


EKF OUTPUT:

![ekf_output_1_without_noise](https://github.com/user-attachments/assets/d50fc862-05ee-485e-b515-051452c47868)

            
UKF OUTPUT:

![UKF_output_2_without_noise](https://github.com/user-attachments/assets/aeff6010-909e-4bf0-84a9-fc7051ec03f0)

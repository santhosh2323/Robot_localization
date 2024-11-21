# Robot_localization
The Repository contains ros-package and algorithms to integrate imu and gps data from kitti/oxts dataset with EKF &amp; UKF node for benchmark analysis

# INTEGRATION

    git clone https://github.com/santhosh2323/Robot_localization.git
    Inside the Robot_localization Folder find the compressed robot_localization.zip file
    Unzip and place it inside your ROS workspace/src folder
    compile your workspace using catkin_make

# RUNNING

    TO RUN EKF:
      roslaunch robot_localization ekf_complete.launch
      
      which contains --- rviz - to launch rviz for visualizations
                         ekf.launch - for launching ekf node
                         navsat.launch - for launching navsat node
                         rviz plotter.py - for plotting ground_truth & filtered/odom trajectories in rviz
                         ground_truth_plotter.py - node for plotting ground truth trajectory
                         filtered_odom_plotter.py - node for plotting filtered odom trajectory
                         rosbag node - for playing rosbag of dataset

    TO RUN UKF:
      roslaunch robot_localization ukf_complete.launch
      
      which contains --- rviz - to launch rviz for visualizations
                         ukf.launch - for launching ukf node
                         navsat.launch - for launching navsat node
                         rviz plotter.py -for plotting ground_truth & filtered/odom trajectories in rviz
                         ground_truth_plotter.py - node for plotting ground truth trajectory
                         filtered_odom_plotter.py - node for plotting filtered odom trajectory
                         rosbag node - for playing rosbag of dataset
# PARAMETERS TUNNING RESULT
 The pose estimation involves parameters tuning in EKF & UKF yaml file to get desired output.Below are the iterations result of tunning various parameters.

# ITERATION 1:

![ekf_output_1_with_noise](https://github.com/user-attachments/assets/546dda26-8c47-493e-b593-36e1f375dfd0)


# ITERATION 2:

![i2](https://github.com/user-attachments/assets/45e92b4d-c850-4e01-a05a-4c5175add64a)


# ITERATION 3:

![iteration1](https://github.com/user-attachments/assets/6a98eb68-9161-46c2-8163-5db0fe0692bd)


# ITERATION 4:

![1](https://github.com/user-attachments/assets/b58435ce-e17d-4e42-9293-ed2827466480)


# ITERATION 5:

![2](https://github.com/user-attachments/assets/359a0660-64f4-4492-a61c-74cbefefc738)

    
# OUTPUT


# EKF OUTPUT:

![ekf_output_1_without_noise](https://github.com/user-attachments/assets/d50fc862-05ee-485e-b515-051452c47868)


            
# UKF OUTPUT:

![UKF_output_2_without_noise](https://github.com/user-attachments/assets/aeff6010-909e-4bf0-84a9-fc7051ec03f0)

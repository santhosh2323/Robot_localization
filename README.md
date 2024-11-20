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
    
![ekf_output_1_with_noise](https://github.com/user-attachments/assets/546dda26-8c47-493e-b593-36e1f375dfd0)

![EKF_Output_2_with_noise](https://github.com/user-attachments/assets/c3caab17-2979-4c53-b25a-1c5997d87b23)

![iteration1](https://github.com/user-attachments/assets/6a98eb68-9161-46c2-8163-5db0fe0692bd)



    
# OUTPUT


# EKF OUTPUT:

![ekf_output_1_without_noise](https://github.com/user-attachments/assets/d50fc862-05ee-485e-b515-051452c47868)


            
# UKF OUTPUT:

![UKF_output_2_without_noise](https://github.com/user-attachments/assets/aeff6010-909e-4bf0-84a9-fc7051ec03f0)

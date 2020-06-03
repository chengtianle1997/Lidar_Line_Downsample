# Lidar_Line_Downsample
Lidar line downsampling for KITTI dataset, transfer lidar the number of lidar lines from 64 to 32, 16, 8, etc.

All of the functions are in kitti_foundation.py
The output results will be saved in the depth and rgb folder.

# projection_example1()
Use projection_example1() to paint a 16-bit lidar-line projection image in PNG format. 
This function required you to change the image_path (rgb image) and velo_path (bin file for point cloud which is provided by KITTI dataset) in line 775 and line 776.
You can change the down_rate in line 531, for example, down_rate = 8 means the number of lidar_lines will be downsampled to 64/8 = 8.
The des_width and des_height in line 746 and line 747 is the width and height of the final output

# projection_example2()
Use projection_example2() to generate a lidar-line projection video in AVI format. 
Others are the same as function projection_example1()

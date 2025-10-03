# Master-Thesis Is Pseudo-LiDAR better than LiDAR ?

The advancement of autonomous systems, particularly in autonomous driving, critically depends on robust and accurate 3D object detection. This thesis investigates the evolution of
3D object detection methodologies, transitioning from classical geometry-driven techniques to
modern deep learning-based approaches. The research was motivated by the need to modernize an initial experimental setup provided by Astemo, which relied on traditional geometric
methods. This thesis was conducted in collaboration with Astemo (formerly Hitachi Astemo),
Munich, Germany, and the German Research Center for Artificial Intelligence (DFKI), Kaiserslautern, Germany.
A key contribution of this work is the development and comprehensive evaluation of advanced
deep neural networks for 3D object detection using Velodyne LiDAR point clouds. The detection backbone was implemented using the OpenPCDet framework, integrating and benchmarking prominent models such as PV-RCNN, PointPillars, and PointRCNN. This evaluation
was conducted on both proprietary LiDAR data from Astemo (formatted as ROS bags) and
the public Kitti dataset. The Robot Operating System (ROS) was utilized for real-time visualization across both datasets and enabled frame-accurate mAP calculation for the Astemo
dataset through synchronized timestamp alignment.
Furthermore, this research explores image-based 3D object detection through the generation
and utilization of pseudo-LiDAR representations. Dense depth maps were generated from
stereo image pairs using PSMNet, subsequently transformed into 3D pseudo-point clouds, and
employed for end-to-end training based on the methodology proposed by Qian et al. 2020. The
pseudo-LiDAR detection system was retrained and validated on the Kitti dataset.
Quantitative evaluation of all approaches was performed using the mean Average Precision
(mAP) metric. This thesis presents a full-stack comparison, analyzing the performance of
classical versus learning-based methods, and real LiDAR versus pseudo-LiDAR modalities.
The strengths and limitations of these approaches are assessed within the context of real-time
perception systems, with particular focus on the current potential and inherent constraints
of stereo vision for 3D object perception. The findings provide valuable insights into the
efficacy of various 3D detection strategies, informing future development in autonomous system
perception.

Square Cupola AprilTag: A High-Precision Fiducial Marker
This repository contains the research results for "Square Cupola AprilTag: A High-Precision Fiducial Marker for Pose Estimation Based on Accuracy Experiments of AprilTag".
Overview
Precise pose estimation is crucial for UAVs, but standard fiducial markers like AprilTag have limitations in detection angles and accuracy. To overcome this, we propose the Square Cupola AprilTag, a high-precision fiducial marker with a three-dimensional structure. This design enables detection over a broader range of angles. Our core contribution is a novel marker and an optimal data fusion method, based on accuracy experiments of the standard AprilTag. This approach significantly reduces pose estimation errors and enhances robustness, especially in challenging reflective environments, providing a reliable solution for UAV visual tracking.
<p align="center">
<img src="Media/prototype.png" width="400" alt="Square Cupola AprilTag Prototype">
</p>
Key Results
1. Improved Pose Estimation Accuracy
Compared to the standard AprilTag, our Square Cupola AprilTag demonstrates a significant reduction in pose estimation error and variance. As shown below, the z-axis position error is reduced by up to four times at a distance of 3.4m. Furthermore, the orientation estimation is more stable, with the rx-axis orientation error consistently remaining below 3.7°, effectively resolving the singularity issue present in the standard AprilTag under certain viewing angles.
<p align="center">
<img src="Media/z%20error.png" alt="Z-axis Error Comparison" width="600"/>
<br/><em>Comparison of z-axis position error between Standard AprilTag and Square Cupola AprilTag.</em>
</p>
<p align="center">
<img src="Media/rx%20error.png" alt="RX-axis Error Comparison" width="600"/>
<br/><em>Comparison of rx-axis orientation error between Standard AprilTag and Square Cupola AprilTag.</em>
</p>
2. UAV Target Tracking Performance
We validated the effectiveness of our marker in simulated UAV tracking scenarios. The UAV successfully tracks a ground vehicle moving in both a straight line (at 0.7 m/s) and a circular path (radius 1m, angular frequency 0.2 rad/s). The system maintains a low tracking error, with a position error of less than 0.07 m in the linear case and 0.16 m in the circular case, demonstrating the precision and reliability of our method for dynamic target tracking using only a monocular camera.
<p align="center">
<b>Linear Motion Tracking</b>
</p>
<p align="center">
<video src="Media/linear%20tracking.mp4" width="600" controls></video>
<br/>
<img src="Media/linear.png" alt="Linear Tracking Error" width="600"/>
<br/><em>Tracking error for a target in uniform linear motion.</em>
</p>
<p align="center">
<b>Circular Motion Tracking</b>
</p>
<p align="center">
<video src="Media/circular%20tracking.mp4" width="600" controls></video>
<br/>
<img src="Media/circular.png" alt="Circular Tracking Trajectory" width="600"/>
<br/><em>Tracking trajectory for a target in uniform circular motion.</em>
</p>
3. Robustness in High-Reflectivity Environments
The Square Cupola AprilTag exhibits superior robustness in challenging lighting conditions. When strong light is directed at a 45° angle, the standard AprilTag fails detection due to reflective interference. In contrast, our marker's polyhedral geometry ensures that other faces of the cupola remain detectable, allowing for continuous and reliable pose estimation. This makes it highly suitable for real-world applications where lighting cannot be controlled.
<p align="center">
<img src="Media/high%20reflective%20environment.png" alt="Detection in Reflective Environment" width="600"/>
<br/><em>Standard AprilTag (left) fails under reflection, while Square Cupola AprilTag (right) remains detectable.</em>
</p>
Publication
This work has been accepted by the International Conference on Aerospace System Science and Engineering (ICASSE 2025) and will be presented orally.
License
This project is licensed under the MIT License.

# Iterative-Closest-Point-ICP-

## Overview
Iterative Closest Point (ICP) is an algorithm used to align two sets of points by estimating the transformation (rotation and translation) between them. It iteratively refines the alignment by minimizing the distance between corresponding points in the two sets.

## Code Explanation
* ``` bash
  icp_matching(previous_points, current_points)
  ```
  The icp_matching function takes two sets of points (previous and current frames) as input and returns the estimated rotation matrix R and  translation vector T that aligns the current points to the previous points.

* ``` bash
  update_homogeneous_matrix(Hin, R, T)
  ```
  The update_homogeneous_matrix function updates the homogeneous transformation matrix Hin by concatenating the rotation matrix R and translation vector T.

* ``` bash
  nearest_neighbor_association(previous_points, current_points)
  ```
  The nearest_neighbor_association function performs the nearest neighbor association between the previous and current points. It calculates the residual errors and finds the best matching indices.

* ``` bash
  svd_motion_estimation(previous_points, current_points)
  ```
  The svd_motion_estimation function estimates the motion (rotation and translation) between the previous and current points using Singular Value Decomposition (SVD) method.

## Result 
<table>
  <tr>
    <td>
      <img src="https://github.com/Naveench7/Vision-based-state-estimation-of-the-quadrotor/assets/100085132/88a73a04-be45-44c6-9d3c-9b9aa7bc2c87" width="500" height="500">
    </td>
    <td>
      <img src="https://github.com/Naveench7/Vision-based-state-estimation-of-the-quadrotor/assets/100085132/2936b6ba-4cfc-4304-8483-c5f13cc66495" width="500" height="500">
    </td>
  </tr>
</table>



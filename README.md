# Optimal Transport
 Variants of the Sinkhorn Algorithm on point clouds

# Abstract
Entropic optimal transport is an increasingly popular method for approximating the distances between two distributions. It is used in a range of applications, such as computer vision, computer graphics, generative adversarial networks, and economics. Many variants for solving entropic optimal transport exist, notably the Sinkhorn Algorithm for its fast computational speed [1]. However, the vanilla form of Sinkhorn suffers from numerical instability on close approximations and does not scale well to large datasets. In this paper, we combine the log stabilized epsilon scaling algorithm introduced in [2] with the symbolic matrices of the KeOps library [3] on the GPU for efficient and stable optimal transport. We then compare our results with [1].

# Example
Below, the distrubution of the heart (seen on the left in color) is distribution onto the circle (grayscale) using optimal transport. 

![before_after_heart](https://github.com/abhelman/Optimal-Transport/assets/113809366/2d3fd4c3-342d-4348-a1e8-8c240d23517e)


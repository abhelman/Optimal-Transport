# Optimal Transport
 Variants of the Sinkhorn Algorithm on point clouds

# Abstract
Entropic optimal transport is an increasingly popular method for approximating the distances between two distributions. It is used in a range of applications, such as computer vision, computer graphics, generative adversarial networks, and economics. Many variants for solving entropic optimal transport exist, notably the Sinkhorn Algorithm for its fast computational speed [1]. However, the vanilla form of Sinkhorn suffers from numerical instability on close approximations and does not scale well to large datasets. In this paper, we combine the log stabilized epsilon scaling algorithm introduced in [2] with the symbolic matrices of the KeOps library [3] on the GPU for efficient and stable optimal transport. We then compare our results with [1].

# Efficient, Mostly Accurate Optimal Tranport
[Optimal_Transport_Writeup.pdf
](https://github.com/abhelman/Optimal-Transport/blob/6d39c898b036f1873a374b20bb4dda0b8fe8a5f7/Optimal_Transport_Writeup.pdf)

# Example
Below, the distrubution of a heart (seen on the left in color) is transported onto the distribution of a circle (grayscale) using optimal transport. 

![before_after](https://github.com/abhelman/Optimal-Transport/assets/113809366/160b2358-7046-4ea2-9815-2b13ef116e4e)

# Sources

[1] M. Cuturi, Sinkhorn Distances : Lightspeed Computation of Optimal Transport, Advances in Neural Information Processing Systems (NIPS) 26, 2013

[2] Schmitzer, B. (2016). Stabilized Sparse Scaling Algorithms for Entropy Regularized Transport Problems. arXiv preprint arXiv:1610.06519.

[3] Jean Feydy, Thibault Sejourne, Francois-Xavier Vialard,
Shun-ichi Amari, Alain Trouve, and Gabriel Peyre. Inter- ´
polating between optimal transport and mmd using sinkhorn
divergences. In The 22nd International Conference on Artificial Intelligence and Statistics, pages 2681–2690, 2019

[4 ] Charlier, B., Feydy, J., and Glaunès, J. (2018). Kernel
operations on the gpu, with autodiff, without memory overflows. http://www.kernel-operations.
io. Accessed: 2018-10-04.

[5] Flamary, R., \& Courty, N. (2017). POT: Python optimal transport library.

[6] https://optimaltransport.github.io/slides-peyre/CourseOT.pdf

[7] Wang, Ying, and Korhan Cengiz. "Implementation of the Spark technique in a matrix distributed computing algorithm." Journal of Intelligent Systems 31.1 (2022): 660-671.

[8] Schmitzer, B.(2020). MultiScaleOT. https://bernhard-schmitzer.github.io/MultiScaleOT/build/html/index.html

[9] Cisneros, Hugo. https://hugocisneros.com/blog/the-elegance-of-optimal-transport/

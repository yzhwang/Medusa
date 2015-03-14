# Medusa
Medusa: Building GPU-based Parallel Sparse Graph Applications with Sequential C/C++ Code

##Introduction##
The graphics processing unit (GPU) has been adopted to accelerate sparse graph processing algorithms such as BFS and shortest path. However, it is difﬁcult to write correct and efﬁcient GPU programs and even more difﬁcult for graph processing due to the irregularities of graph structures. To simplify graph processing on GPUs, we introduce Medusa, a programming framework which enables developers to leverage the capabilities of GPUs by writing sequential C/C++ code. Medusa focuses on sparse graph, which is more challenging than the dense graph for GPU processing, due to its more irregular computation and memory access patterns.

Medusa offers a small set of user-deﬁned APIs, and embraces a runtime system to automatically execute those APIs in parallel on the GPUs. We further develop a series of graph-centric optimizations based on the architecture features of GPU for efﬁciency. Additionally, Medusa is extended to execute on multiple GPUs within a machine or a cluster. Our empirical studies demonstrate the programmability and efﬁciency of Medusa for a series of common graph operations.

##Platform##
The current version of Medusa is implemented using the following platform.

Programming Language - CUDA, C/C++
Build - MS Visual Studio/gcc, CUDA nvcc

##Datasets##
We provide a set of graph files to test Medusa. These graphs are also used in our papers. The graph files are stored in the GTGraph output format.

random.1mv.16me
Wikitalk
rmat.1mv.16me
roadNet-CA


##Project News##
[2012-8-23] Medusa is now on Google Code.
[2012-8-29] Technical Report on the design and implementation of Medusa is available.
[2012-8-30] First release (Version 0.1) of Medusa source code available.
[2013-2-28] Version 0.2 now available.
[2014-3-12] C Code for coverting a GTGraph format graph to a METIS format graph.
[2015-3-14] Migrate project from [google code](https://code.google.com/p/medusa-gpu/) to GitHub.

##ublications##
Jianlong Zhong, Bingsheng He, Towards GPU-Accelerated Large-Scale Graph Processing in the Cloud. CloudCom? 2013.
Jianlong Zhong, Bingsheng He, Kernelet: High-Throughput GPU Kernel Executions with Dynamic Slicing and Scheduling. Accepted by IEEE Transactions on Parallel and Distributed Systems, 2013. [pdf].
Jianlong Zhong, Bingsheng He, Parallel Graph Processing on Graphics Processors Made Easy. Accepted by VLDB 2013, Demonstrations Track.
Jianlong Zhong, Bingsheng He, Medusa: Simplified Graph Processing on GPUs. Accepted by IEEE Transactions on Parallel and Distributed Systems, April, 2013. [manuscript] [supplementary file].
Jianlong Zhong, Bingsheng He, An overview of Medusa: simplified graph processing on GPUs. PPoPP 2012: Proceedings of 17th ACM SIGPLAN Symposium on Principles and Practice of Parallel Programming (Poster paper, 2 pages) [full text].
Jiangming Jin, Stephen John Turner, Bu-Sung Lee, Jianlong Zhong, Bingsheng He, HPC Simulations of Information Propagation Over Social Networks. Procedia CS 9: 292-301 (2012) [full text].
Jianlong Zhong, Bingsheng He, GViewer: GPU-Accelerated Graph Visualization and Mining. SocInfo? 2011: 304-307 [full text]
More Recent Projects on Parallel & Distributed Graph Processing
Google Pregel
GraphLab
GPS: A Graph Processing System
Medusa is developed by the Parallel and Distributed Computing Center, Nanyang Technological University. Contact: ZHONG Jianlong (jzhong2@ntu.edu.sg).
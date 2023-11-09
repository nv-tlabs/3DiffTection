# 3DiffTection

<div align="center">
Official code and tool release for: 


**3DiffTection: 3D Object Detection with Geometry-Aware Diffusion Features**

[Chenfeng Xu](https://chenfengx.com/), [Huan Ling](http://www.cs.toronto.edu/~linghuan/)\, [Sanja Fidler](http://www.cs.toronto.edu/~fidler/), [Or Litany](https://orlitany.github.io)


[[project page](https://research.nvidia.com/labs/toronto-ai/3difftection/)] [[paper](https://arxiv.org/abs/2311.04391)]
</div>


<img src = "https://research.nvidia.com/labs/toronto-ai/3difftection/resources/image%20(4).png" width="100%"/>

We present 3DiffTection, a cutting-edge method for 3D detection from single images, grounded in features from a 3D-aware diffusion model. Annotating large-scale image data for 3D object detection is both resource-intensive and time-consuming. Recently, large image diffusion models have gained traction as potent feature extractors for 2D perception tasks. However, since these features, originally trained on paired text and image data, are not directly adaptable to 3D tasks and often misalign with target data, our approach bridges these gaps through two specialized tuning strategies: geometric and semantic. For geometric tuning, we refine a diffusion model on a view synthesis task, introducing a novel epipolar warp operator. This task meets two pivotal criteria: the necessity for 3D awareness and reliance solely on posed image data, which are readily available (e.g., from videos). For semantic refinement, we further train the model on target data using box supervision. Both tuning phases employ a ControlNet to preserve the integrity of the original feature capabilities. In the final step, we harness these capabilities to conduct a test-time prediction ensemble across multiple virtual viewpoints. Through this methodology, we derive 3D-aware features tailored for 3D detection and excel in identifying cross-view point correspondences.

[![Watch the video](https://research.nvidia.com/labs/toronto-ai/3difftection/resources/det.png)](https://research.nvidia.com/labs/toronto-ai/3difftection/resources/3difftection.mp4)
Click above image to see video demo!

Code coming soon.



### Citations

Please use the following citation if you use our data or code:

```
@article{xu20233difftection,
      title={3DiffTection: 3D Object Detection with Geometry-Aware Diffusion Features}, 
      author={Chenfeng Xu and Huan Ling and Sanja Fidler and Or Litany},
      year={2023},
      archivePrefix={arXiv},
      primaryClass={cs.CV}}
```



### License

Copyright © 2022, NVIDIA Corporation. All rights reserved.

This work is made available under the Nvidia Source Code License-NC. Please see our main [LICENSE](./LICENSE) file.

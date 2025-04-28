# Awesome Gaussian SLAM Resources

A curated list of papers and open-source resources focused on gaussian based slam system, focusing on slam systems with gaussian based mapping representation with any utilities. The ambition is keeping pace with the anticipated surge of research in the coming months. If you have any additions or suggestions, feel free to contribute. Additional resources like blog posts, videos, etc. are also welcome.

## Table of contents

- [Seminal Introduction Material](#introduction)

  - [Nerf](#nerf)
  - [3D Gaussian Splatting](#3d-gaussian-splatting)
    <br>

- [Survey](#survey)
- [Optimization](#gaussian-optimization)
- [Gaussian SLAM](#gaussian-slam)
- [Navigation](#navigation)
- [Poses](#poses)
- [Large-Scale](#large-scale)
- [3D Reconstruction](#3d-reconstruction)
- [Gaussian Surfel ](#gaussian-surfel)
- [3D Generation ](#3d-generations)
<br>

- [Data](#data)
- [Courses](#courses)

<br>

- [Open Source Implementations](#open-source-implementations)

  - [Unofficial Implementations](#unofficial-implementations)
  - [2D Gaussian Splatting](#2d-gaussian-splatting)
  - [Game Engines](#game-engines)
  - [Viewers](#viewers)
  - [Utilities](#utilities)
  - [Tutorial](#tutorial)
  - [Framework](#framework)
  - [Other](#other)
    <br>

- [Blog Posts](#blog-posts)
- [Tutorial Videos](#tutorial-videos)
- [Credits](#credits)

<details span>
<summary><b>Update Log:</b></summary>
<br>
 **July 11, 2024**
 - Initial version
<br>
 **July 16, 2024**
 - Add survey and theory sections
<br>
 **August 9, 2024**
 - Add relevant papers and viewers
<br>
 **September 27, 2024**
 - Add relevant papers, reorganize sections
<br>
 **November 07, 2024**
 - Add relevant papers, add 3d generation section
<br>
 **January 2, 2025**
 - Add relevant papers and rename sections
</details>

<br>

## Introduction:

### Nerf:
- [NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis](https://www.matthewtancik.com/nerf), Mildenhall et al., ECCV 2020 | [📄 Paper](https://arxiv.org/abs/2003.08934.pdf) | [💻 Code](https://github.com/bmild/nerf)

### 3D Gaussian Splatting:
- [3D Gaussian Splatting for Real-Time Radiance Field Rendering](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/), Kerbl et al., SIGGRAPH 2023 | [📄 Paper](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/3d_gaussian_splatting_high.pdf) | [💻 Code](https://github.com/graphdeco-inria/gaussian-splatting) | [🎥 Short Presentation](https://youtu.be/T_kXY43VZnk?si=DrkbDFxQAv5scQNT) | [🎥 Explanation Video](https://www.youtube.com/live/xgwvU7S0K-k?si=edF8NkYtsRbgTbKi)
<br>


## Survey:
- **3D Scene Generation: A Survey**, Wen et al., arXiv 2025  | [📄 Paper](https://www.arxiv.org/abs/2505.05474) | [🌐 Project Page](https://github.com/hzxie/Awesome-3D-Scene-Generation)

- **The Role of World Models in Shaping Autonomous Driving: A Comprehensive Survey**, Tu et al., arXiv 2025  | [📄 Paper](https://arxiv.org/abs/2502.10498) | [🌐 Project Page](https://github.com/LMD0311/Awesome-World-Model)

- **Embodied Intelligence for 3D Understanding: A Survey on 3D Scene Question Answering**, Li et al., arXiv 2025  | [📄 Paper](https://arxiv.org/abs/2502.00342)

- **Scene reconstruction techniques for autonomous driving: a review of 3D Gaussian splatting**, Zhu et al., Artificial Intelligence Review 2024 | [📄 Paper](https://link.springer.com/content/pdf/10.1007/s10462-024-10955-4.pdf)

- **A Survey on 3D Gaussian Splatting**, Chen et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2401.03890.pdf)

- **How NeRFs and 3D Gaussian Splatting are Reshaping SLAM: a Survey**, Tosi et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2402.13255)

- **3D Gaussian Splatting: Survey, Technologies, Challenges, and Opportunities**, Chen et al., TPAMI 2024 | [📄 Paper](https://arxiv.org/pdf/2407.17418.pdf) | [🌐 Project Page](https://github.com/qqqqqqy0227/awesome-3DGS)

- **3D Gaussian as a New Vision Era: A Survey**, Fei et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2402.07181.pdf)

- **Recent Advances in 3D Gaussian Splatting**, Wu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.11134.pdf)

- **How NeRFs and 3D Gaussian Splatting are Reshaping SLAM: a Survey**, Tosi et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2402.13255)

- **Gaussian Splatting: 3D Reconstruction and Novel View Synthesis, a Review**, Dalal et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2405.03417.pdf)

- **Learning-based 3D Reconstruction in Autonomous Driving: A Comprehensive Survey**, Liao et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.14537)

## Gaussian Optimization:
## 2025:
- **[ICRA '25]R3GS: Gaussian Splatting for Robust Reconstruction and Relocalization in Unconstrained Image Collections**, Yan et al., arXiv 2025 | [📄 Paper](https://www.arxiv.org/abs/2505.15294) | [🌐 Project Page]() | | [💻 Code]()

- **[CVPRW '25]SparSplat: Fast Multi-View Reconstruction with Generalizable 2D Gaussian Splatting**, Jena et al., arXiv 2025 | [📄 Paper](https://www.arxiv.org/abs/2505.02175) | [🌐 Project Page](https://shubhendu-jena.github.io/SparSplat/) | | [💻 Code](https://github.com/Shubhendu-Jena/SparSplat)

- **[CVPR '25]Steepest Descent Density Control for Compact 3D Gaussian Splatting**, Wang et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2505.05587) | [🌐 Project Page](https://vita-group.github.io/SteepGS/) | | [💻 Code]()

- **[ICML '25]HybridGS: High-Efficiency Gaussian Splatting Data Compression using Dual-Channel Sparse Representation and Point Cloud Encoder**, Yang et al., arXiv 2025 | [📄 Paper](https://www.arxiv.org/abs/2505.01938) | [🌐 Project Page]() | | [💻 Code](https://github.com/Qi-Yangsjtu/HybridGS)

- **[ICLR '25]PCGS: Progressive Compression of 3D Gaussian Splatting**, Chen et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.08511) | [🌐 Project Page](https://yihangchen-ee.github.io/project_pcgs/) | | [💻 Code](https://github.com/YihangChen-ee/PCGS)

- **StyleMe3D: Stylization with Disentangled Priors by Multiple Encoders on 3D Gaussians**, Zhuang et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2504.15281) | [🌐 Project Page](https://styleme3d.github.io/) | | [💻 Code](https://github.com/AIGCResearch/styleme3d)

- **ADGaussian: Generalizable Gaussian Splatting for Autonomous Driving with Multi-modal Inputs**, Song et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2504.00437) | [🌐 Project Page](https://maggiesong7.github.io/research/ADGaussian/) | | [💻 Code]()

- **[ICLR '25]CAT-3DGS: A Context-Adaptive Triplane Approach to Rate-Distortion-Optimized 3DGS Compression**, Zhan et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.00357) | [🌐 Project Page]() | | [💻 Code]()

- **[CVPR '25]COB-GS: Clear Object Boundaries in 3DGS Segmentation Based on Boundary-Adaptive Gaussian Splitting**, Zhang et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.19443) | [🌐 Project Page]() | | [💻 Code](https://github.com/ZestfulJX/COB-GS)

- **[CVPR '25]BG-Triangle: Bézier Gaussian Triangle for 3D Vectorization and Rendering**, Wu et al., arXiv 2025 | [📄 Paper](https://www.arxiv.org/abs/2503.13961) | [🌐 Project Page](https://wuminye.github.io/projects/BGTriangle/) | | [💻 Code](https://github.com/wuminye/bg-triangle)

- **[CVPR '25]DashGaussian: Optimizing 3D Gaussian Splatting in 200 Seconds**, Chen et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.18402) | [🌐 Project Page](https://dashgaussian.github.io/) | | [💻 Code]()

- **Drag Your Gaussian: Effective Drag-Based Editing with Score Distillation for 3D Gaussian Splatting**, Qu et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.18672) | [🌐 Project Page](https://quyans.github.io/Drag-Your-Gaussian/) | | [💻 Code](https://github.com/Quyans/Drag-Your-Gaussian)

- **See In Detail: Enhancing Sparse-view 3D Gaussian Splatting with Local Depth and Semantic Regularization**, He et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.11508)

- **HAC++: Towards 100X Compression of 3D Gaussian Splatting**, Chen et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.12255) | [🌐 Project Page](https://yihangchen-ee.github.io/project_hac++/) | | [💻 Code](https://github.com/YihangChen-ee/HAC-plus)

- **MoDec-GS: Global-to-Local Motion Decomposition and Temporal Interval Adjustment for Compact Dynamic 3D Gaussian Splatting**, Kwak et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.03714) | [🌐 Project Page](https://kaist-viclab.github.io/MoDecGS-site/) | | [💻 Code]()

## 2024:
- **[NeurIPS' 24]3DGS-Enhancer: Enhancing Unbounded 3D Gaussian Splatting with View-consistent 2D Diffusion Priors**, Liu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2410.16266) | [🌐 Project Page](https://xiliu8006.github.io/3DGS-Enhancer-project/) | | [💻 Code](https://github.com/xiliu8006/3DGS-Enhancer)

- **MaskGaussian: Adaptive 3D Gaussian Representation from Probabilistic Masks**, Liu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2412.20522) | [🌐 Project Page]() | | [💻 Code](https://github.com/kaikai23/MaskGaussian)

- **Turbo-GS: Accelerating 3D Gaussian Fitting for High-Quality Radiance Fields**, Lu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2412.13547) | [🌐 Project Page](https://ivl.cs.brown.edu/research/turbo-gs) | | [💻 Code](https://github.com/inspirelt/Turbo-GS)

- **LeanGaussian: Breaking Pixel or Point Cloud Correspondence in Modeling 3D Gaussians**, Wu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2404.16323) | [🌐 Project Page](https://kenkunliu.github.io/DIG3D/) | | [💻 Code](https://github.com/jwubz123/DIG3D)

- **[NeurIPS' 24]DiffGS: Functional Gaussian Splatting Diffusion**, Zhou et al., arXiv 2024 | [📄 Paper](https://arxiv.org/html/2410.19657v1) | [🌐 Project Page](https://junshengzhou.github.io/DiffGS/) | | [💻 Code](https://github.com/weiqi-zhang/DiffGS)

- **[ECCV' 24]MVSGaussian: Fast Generalizable Gaussian Splatting Reconstruction from Multi-View Stereo**, Liu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2405.12218) | [🌐 Project Page](https://mvsgaussian.github.io/) | | [💻 Code](https://github.com/TQTQliu/MVSGaussian) | [🎥 Video](https://www.youtube.com/watch?v=4TxMQ9RnHMA)

- **No Pose, No Problem: Surprisingly Simple 3D Gaussian Splats from Sparse Unposed Images**, Ye et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2410.24207) | [🌐 Project Page](https://noposplat.github.io/) | [💻 Code](https://github.com/cvg/NoPoSplat)

- **Octree-GS: Towards Consistent Real-time Rendering with LOD-Structured 3D Gaussians**, Ren et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2403.17898) | [🌐 Project Page](https://city-super.github.io/octree-gs/) | [💻 Code](https://github.com/city-super/Octree-GS)

- **TetSphere Splatting: Representing High-Quality Geometry with Lagrangian Volumetric Meshes**, Guo et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2405.20283) | [💻 Code](https://github.com/gmh14/tssplat)

- **MVSplat: Efficient 3D Gaussian Splatting from Sparse Multi-View Images**, Chen et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2403.14627) | [🌐 Project Page](https://donydchen.github.io/mvsplat/) | [💻 Code](https://github.com/donydchen/mvsplat)

- **3D Gaussian Ray Tracing: Fast Tracing of Particle Scenes**, Moenne-Loccoz et al., arXiv 2024 | [📄 Paper](https://www.arxiv.org/abs/2407.07090) | [🌐 Project Page](https://gaussiantracer.github.io/) | [🎥 Video](https://gaussiantracer.github.io/#supp_video)

- **3D Gaussian Splatting as Markov Chain Monte Carlo**, Ye et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2404.09591) | [🌐 Project Page](https://ubc-vision.github.io/3dgs-mcmc/) | [💻 Code](https://github.com/ubc-vision/3dgs-mcmc)

- **AbsGS: Recovering Fine Details for 3D Gaussian Splatting**, Ye et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2404.10484) | [🌐 Project Page](https://ty424.github.io/AbsGS.github.io/) | [💻 Code](https://github.com/TY424/AbsGS)

- **[CVPR '24 Highlight]Scaffold-GS: Structured 3D Gaussians for View-Adaptive Rendering**, Lu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2312.00109) | [🌐 Project Page](https://city-super.github.io/scaffold-gs/) | [💻 Code](https://github.com/city-super/Scaffold-GS)

- **Gaussian Splatting Lucas-Kanade**, Xie et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2407.11309v1)

- **InstantSplat: Sparse-view SfM-free Gaussian Splatting in Seconds**, Fan et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2403.20309) | [🌐 Project Page](https://instantsplat.github.io/) | [💻 Code](https://github.com/NVlabs/InstantSplat) | [🎥 Video](https://www.youtube.com/watch?v=JdfrG89iPOA&t=347s) | [🤗 Demo](https://huggingface.co/spaces/kairunwen/InstantSplat)

- **Texture-GS: Disentangling the Geometry and Texture for 3D Gaussian Splatting Editing**, Xu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.10050) | [🌐 Project Page](https://slothfulxtx.github.io/TexGS/) | [💻 Code](https://github.com/slothfulxtx/Texture-GS)

- **[CVPR '24]CoGS: Controllable Gaussian Splatting**, Yu et al., CVPR 2024 | [📄 Paper](https://arxiv.org/abs/2312.05664) | [🌐 Project Page](https://cogs2024.github.io/) | [💻 Code](https://github.com/Heng14/CoGS)

- **[CVPR '24]4D Gaussian Splatting for Real-Time Dynamic Scene Rendering**, Wu et al., CVPR 2024 | [📄 Paper](https://arxiv.org/abs/2310.08528.pdf) | [🌐 Project Page](https://guanjunwu.github.io/4dgs/) | [💻 Code](https://github.com/hustvl/4DGaussians)

- **Trim 3D Gaussian Splatting for Accurate Geometry Representation**, Fan et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2406.07499.pdf) | [🌐 Project Page](https://trimgs.github.io/) | [💻 Code](https://github.com/YuxueYang1204/TrimGS)

- **[CVPR '24 Best Student Paper]Mip-Splatting Alias-free 3D Gaussian Splatting**, Yu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2311.16493.pdf) | [🌐 Project Page](https://niujinshuchong.github.io/mip-splatting/) | [💻 Code](https://github.com/autonomousvision/mip-splatting)

- **[CVPR '24]COLMAP-Free 3D Gaussian Splatting**, Fu et al., arXiv 2023 | [📄 Paper](https://arxiv.org/abs/2312.07504) | [🌐 Project Page](https://oasisyang.github.io/colmap-free-3dgs/) | [💻 Code](https://github.com/NVlabs/CF-3DGS) | [🎥 Video](https://www.youtube.com/watch?v=mGeVQS4ExK4)


## Gaussian SLAM:
## 2025
- **[ICRA '25]  Hier-SLAM: Semantic Gaussian Splatting SLAM with Hierarchical Categorical Representation**, Li et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2409.12518) | [💻 Code](https://github.com/LeeBY68/Hier-SLAM) | [🎥 Video](https://www.youtube.com/watch?v=Lp0QPMDTTHk)

- **GauS-SLAM: Dense RGB-D SLAM with Gaussian Surfels**, Su et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2505.01934) | [💻 Code](https://github.com/gaus-slam/gaus-slam) | [🌐 Project Page](https://gaus-slam.github.io/)

- **[CVPR '25] SLAM3R: Real-Time Dense Scene Reconstruction from Monocular RGB Videos**, Liu et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2412.09401) | [💻 Code](https://github.com/PKU-VCL-3DV/SLAM3R) | [🤗 Demo]()

- **[CVPR '25] St4RTrack: Simultaneous 4D Reconstruction and Tracking in the World**, Feng et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2504.13152) | [🌐 Project Page](https://st4rtrack.github.io/) | [💻 Code]()

- **[CVPR '25] WildGS-SLAM: Monocular Gaussian Splatting SLAM in Dynamic Environments**, Zheng et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2504.03886) | [🌐 Project Page](https://wildgs-slam.github.io/) | [💻 Code](https://github.com/GradientSpaces/WildGS-SLAM) | [🎥 Video](https://www.youtube.com/watch?v=xXuolzFvddQ&t=11s)

- **[ICRA '25] HS-SLAM: Hybrid Representation with Structural Supervision for Improved Dense SLAM**, Gong et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.21778) | [🌐 Project Page](https://zorangong.github.io/HS-SLAM/) | [💻 Code]() | [🎥 Video]()

- **4D Gaussian Splatting SLAM**, Li et al., arXiv 2025 | [📄 Paper](https://www.arxiv.org/abs/2503.16710) | [🌐 Project Page]() | [💻 Code](https://github.com/yanyan-li/4DGS-SLAM) | [🎥 Video]()

- **[ICRA '25] OpenGS-SLAM: Open-Set Dense Semantic SLAM with 3D Gaussian Splatting for Object-Level Scene Understanding**, Yang et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.01646) | [🌐 Project Page](https://young-bit.github.io/opengs-github.github.io/) | [💻 Code](https://github.com/YOUNG-bit/open_semantic_slam) | [🎥 Video](https://www.youtube.com/watch?v=uNJ4vTpfGU0)

- **GigaSLAM: Large-Scale Monocular SLAM with Hierachical Gaussian Splats**, Deng et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.08071) | [🌐 Project Page]() | [💻 Code](https://github.com/DengKaiCQ/GigaSLAM)

- **RGB-Only Gaussian Splatting SLAM for Unbounded Outdoor Scenes**, Yu et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.15633) | [🌐 Project Page](https://3dagentworld.github.io/opengs-slam/) | [💻 Code](https://github.com/3DAgentWorld/OpenGS-SLAM)

- **DenseSplat: Densifying Gaussian Splatting SLAM with Neural Radiance Prior**, Li et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.09111) 

- **PINGS: Gaussian Splatting Meets Distance Fields within a Point-Based Implicit Neural Map**, Pan et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.05752) | [🌐 Project Page]() | [💻 Code](https://github.com/PRBonn/PINGS)

- **MapGS: Generalizable Pretraining and Data Augmentation for Online Mapping via Novel View Synthesis**, Zhang et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.06660) | [🌐 Project Page](https://henryzhangzhy.github.io/mapgs/)

- **SplatMAP: Online Dense Monocular SLAM with 3D Gaussian Splatting**, Hu et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.07015) | [🎥 Video](https://www.youtube.com/watch?v=Pr_kyWQQkGo)

- **GS-LIVO: Real-Time LiDAR, Inertial, and Visual Multi-sensor Fused Odometry with Gaussian Mapping**, Hong et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.08672) | [💻 Code](https://github.com/HKUST-Aerial-Robotics/GS-LIVO) 

- **VINGS-Mono: Visual-Inertial Gaussian Splatting Monocular SLAM in Large Scenes**, Wu et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.08286) 

- **Scaffold-SLAM: Structured 3D Gaussians for Simultaneous Localization and Photorealistic Mapping**, Wen et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.05242) 

## 2024:
- **[CVPR '25]MASt3R-SLAM: Real-Time Dense SLAM with 3D Reconstruction Priors**, Murai et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2412.12392) | [🌐 Project Page](https://edexheim.github.io/mast3r-slam/) | [💻 Code](https://github.com/rmurai0610/MASt3R-SLAM) | [🎥 Video](https://www.youtube.com/watch?v=wozt71NBFTQ)

- **HI-SLAM2 Geometry-Aware Gaussian SLAM for Fast Monocular Scene Reconstruction**, Zhang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2411.17982) | [🌐 Project Page](https://hi-slam2.github.io/) | [💻 Code](https://github.com/Willyzw/HI-SLAM2)

- **DGS-SLAM: Gaussian Splatting SLAM in Dynamic Environment**, Kong et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2411.10722) | [🌐 Project Page](https://changjianjiang01.github.io/LI-GS/) | | [🎥 Video](https://www.youtube.com/watch?v=Mq3qZTTcN3E) | [💻 Code](https://github.com/kmk97/DGS-SLAM)

- **DG-SLAM: Robust Dynamic Gaussian Splatting SLAM with Hybrid Pose Optimization**, Xu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2411.08373) | [💻 Code](https://github.com/fudan-zvg/DG-SLAM)

- **LI-GS: Gaussian Splatting with LiDAR Incorporated for Accurate Large-Scale Reconstruction**, Jiang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2409.12899) | [🌐 Project Page](https://changjianjiang01.github.io/LI-GS/) | [🎥 Video](https://www.youtube.com/watch?v=DSsTCbD4mJQ)

- **MGSO: Monocular Real-time Photometric SLAM with Efficient 3D Gaussian Splatting**, Hu et al., arXiv 2024 | [📄 Paper](https://www.arxiv.org/abs/2409.13055)

- **GSFusion: Online RGB-D Mapping Where Gaussian Splatting Meets TSDF Fusion**, Wei and Leutenegger, arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2408.12677) | [🌐 Project Page](https://gs-fusion.github.io/) | [💻 Code](https://github.com/GS-Fusion/GSFusion) | | [🎥 Video](https://www.youtube.com/watch?v=rW8o_cRPZBg)

- **Visual SLAM with 3D Gaussian Primitives and Depth Priors Enabling Novel View Synthesis**, Qu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2408.05635)

- **IG-SLAM: Instant Gaussian SLAM**, Sarikamis and Alatan, arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2408.01126)

- **EndoGSLAM: Real-Time Dense Reconstruction and Tracking in Endoscopic Surgeries using Gaussian Splatting**, Wang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2403.15124)

- **SGS-SLAM: Semantic Gaussian Splatting For Neural Dense SLAM**, Li et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2402.03246.pdf) | [🎥 Video](https://www.youtube.com/watch?v=y83yw1E-oUo)

- **SemGauss-SLAM: Dense Semantic Gaussian Splatting SLAM**, Zhu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.07494.pdf)

- **Compact 3D Gaussian Splatting For Dense Visual SLAM**, Deng et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.11247.pdf)

- **NEDS-SLAM: A Novel Neural Explicit Dense Semantic SLAM Framework using 3D Gaussian Splatting**, Ji et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.11679.pdf)

- **High-Fidelity SLAM Using Gaussian Splatting with Rendering-Guided Densification and Regularized Optimization**, Sun et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.12535.pdf)

- **RGBD GS-ICP SLAM**, Ha et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.12550.pdf) | [💻 Code](https://github.com/Lab-of-AI-and-Robotics/GS_ICP_SLAM) | [🎥 Short Presentation](https://youtu.be/e-bHh_uMMxE?si=bU4_Su4J91WQ2MEX)

- **EndoGSLAM: Real-Time Dense Reconstruction and Tracking in Endoscopic Surgeries using Gaussian Splatting** Wang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.15124.pdf) | [🌐 Project Page](https://endogslam.loping151.com/) | [💻 Code](https://github.com/Loping151/EndoGSLAM)

- **CG-SLAM: Efficient Dense RGB-D SLAM in a Consistent Uncertainty-aware 3D Gaussian Field**, Ren et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.16095.pdf) | [🌐 Project Page](https://zju3dv.github.io/cg-slam/) | [💻 Code](https://github.com/hjr37/CG-SLAM)

- **MM3DGS SLAM: Multi-modal 3D Gaussian Splatting for SLAM Using Vision, Depth, and Inertial Measurements** Sun et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2404.00923) | [🌐 Project Page](https://vita-group.github.io/MM3DGS-SLAM/) | [💻 Code (not yet)]()

- **Gaussian-LIC: Photo-realistic LiDAR-Inertial-Camera SLAM with 3D Gaussian Splatting**, Lang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2404.06926.pdf)

## 2023:
- **[CVPR '24] GS-SLAM: Dense Visual SLAM with 3D Gaussian Splatting**, Yan et al., arXiv 2023 | [📄 Paper](https://arxiv.org/pdf/2311.11700.pdf) | [🌐 Project Page](https://gs-slam.github.io/)

- **[CVPR '24] SplaTAM: Splat, Track & Map 3D Gaussians for Dense RGB-D SLAM**, Keetha et al., arXiv 2023 | [📄 Paper](https://arxiv.org/pdf/2312.02126.pdf) | [🌐 Project Page](https://spla-tam.github.io/) | [💻 Code](https://github.com/spla-tam/SplaTAM) | [🎥 Explanation Video](https://www.youtube.com/watch?v=35SX8DTdQLs)

- **[CVPR '24] Gaussian Splatting SLAM**, Matsuki et al., arXiv 2023 | [📄 Paper](https://www.imperial.ac.uk/media/imperial-college/research-centres-and-groups/dyson-robotics-lab/hide-et-al_GaussianSplattingSLAM_Dec2023.pdf) | [🌐 Project Page](https://rmurai.co.uk/projects/GaussianSplattingSLAM/) | [💻 Code](https://github.com/muskie82/MonoGS) | [🎥 Short Presentation](https://youtu.be/x604ghp9R_Q?si=fPtz4kgBKFfcnQf3)

- **Gaussian-SLAM: Photo-realistic Dense SLAM with Gaussian Splatting**, Yugay et al., arXiv 2023 | [📄 Paper](https://arxiv.org/pdf/2312.10070) | [🌐 Project Page](https://vladimiryugay.github.io/gaussian_slam/) | [💻 Code](https://github.com/VladimirYugay/Gaussian-SLAM) | [🎥 Short Presentation](https://www.youtube.com/watch?v=RZK1o_ija7M)

- **[CVPR '24] Photo-SLAM: Real-time Simultaneous Localization and Photorealistic Mapping for Monocular, Stereo, and RGB-D Cameras**, Huang et al., arXiv 2023 | [📄 Paper](https://arxiv.org/pdf/2311.16728.pdf) | [🌐 Project Page](https://huajianup.github.io/research/Photo-SLAM/) | [💻 Code](https://github.com/HuajianUP/Photo-SLAM)

<br>

## Navigation:
## 2025:
- **GS-GVINS: A Tightly-integrated GNSS-Visual-Inertial Navigation System Augmented by 3D Gaussian Splatting**, Zhou et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.10975)

## 2024:
- **Wonderland: Navigating 3D Scenes from a Single Image**, Liang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2412.12091) | [🌐 Project Page](https://snap-research.github.io/wonderland/) | [💻 Code]()

- **GaussNav: Gaussian Splatting for Visual Navigation**, Lei et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.11625.pdf) | [🌐 Project Page](https://xiaohanlei.github.io/projects/GaussNav/) | [💻 Code](https://github.com/XiaohanLei/GaussNav)

- **3DGS-ReLoc: 3D Gaussian Splatting for Map Representation and Visual ReLocalization**, Jiang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.11367.pdf)

- **Beyond Uncertainty: Risk-Aware Active View Acquisition for Safe Robot Navigation and 3D Scene Understanding with FisherRF**, Liu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.11396.pdf)

- **3DGS-Calib: 3D Gaussian Splatting for Multimodal SpatioTemporal Calibration**, Herau et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.11577.pdf)

- **[CVPR '24] HUGS: Holistic Urban 3D Scene Understanding via Gaussian Splatting** Zhou et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.12722.pdf) | [🌐 Project Page](https://xdimlab.github.io/hugs_website/)| [💻 Code](https://github.com/hyzhou404/HUGS)

- **HO-Gaussian: Hybrid Optimization of 3D Gaussian Splatting for Urban Scenes**, Li et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.20032.pdf)

- **SGD: Street View Synthesis with Gaussian Splatting and Diffusion Prior**, Yu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.20079.pdf)


## Poses:
## 2025:
- **Targetless LiDAR-Camera Calibration with Anchored 3D Gaussians**, Jung et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.08982) | [🌐 Project Page](https://zang09.github.io/tlc-calib-site/) | [💻 Code]()

- **CityLoc: 6 DoF Localization of Text Descriptions in Large-Scale Scenes with Gaussian Representation**, Ma et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2504.04597v1) 

## 2024:
- **[ECCV '24]GGRt: Towards Generalizable 3D Gaussians without Pose Priors in Real-Time**, Li et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.10147) | [🌐 Project Page](https://3d-aigc.github.io/GGRt/)

- **GS-Pose: Cascaded Framework for Generalizable Segmentation-based 6D Object Pose Estimation**, Cai et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.10683) | [🌐 Project Page](https://dingdingcai.github.io/gs-pose/) | [💻 Code](https://github.com/dingdingcai/GS-pose) | [🎥 Short Presentation](https://youtu.be/SnJazusDLM8)


## Large Scale:
## 2025:
- **Large-Scale Gaussian Splatting SLAM**, Xin et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2505.09915) | [🌐 Project Page](https://lsg-slam.github.io/)| [💻 Code]()

- **BlockGaussian: Efficient Large-Scale Scene Novel View Synthesis via Adaptive Block-Based Gaussian Splatting**, Wu et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2504.09048) | [🌐 Project Page](https://sunshinewyc.github.io/BlockGaussian/)| [💻 Code](https://github.com/SunshineWYC/BlockGaussian)

- **CityGS-X: A Scalable Architecture for Efficient and Geometrically Accurate Large-Scale Scene Reconstruction**, Gao et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.23044) | [🌐 Project Page](https://lifuguan.github.io/CityGS-X/)| [💻 Code](https://github.com/gyy456/CityGS-X)

- **[ICLR 25]DynamicCity: Large-Scale LiDAR Generation from Dynamic Scenes**, Bian et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2410.18084v1) | [🌐 Project Page](https://dynamic-city.github.io/)| [💻 Code](https://github.com/3DTopia/DynamicCity)

- **OG-Gaussian: Occupancy Based Street Gaussians for Autonomous Driving**, Shen et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.14235)

## 2024:
- **GaussianWorld: Gaussian World Model for Streaming 3D Occupancy Prediction**, Zuo et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2412.10373) | [💻 Code](https://github.com/zuosc19/GaussianWorld)

- **[ECCV 2024]Gaussian Grouping: Segment and Edit Anything in 3D Scenes**, Ye et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2312.00732) | [🌐 Project Page](https://ymq2017.github.io/gaussian-grouping/)| [💻 Code](https://github.com/lkeab/gaussian-grouping)

- **CityGaussianV2: Efficient and Geometrically Accurate Reconstruction for Large-Scale Scenes**, Liu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2411.00771) | [🌐 Project Page](https://dekuliutesla.github.io/CityGaussianV2/)| [💻 Code](https://github.com/DekuLiuTesla/CityGaussian)

- **Momentum-GS: Momentum Gaussian Self-Distillation for High-Quality Large Scene Reconstruction**, Fan et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2411.00771) | [🌐 Project Page](https://jixuan-fan.github.io/Momentum-GS_Page/)| [💻 Code](https://github.com/Jixuan-Fan/Momentum-GS)

- **[ECCV 2024]Street Gaussians: Modeling Dynamic Urban Scenes with Gaussian Splatting**, Yan et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2401.01339) | [🌐 Project Page](https://zju3dv.github.io/street_gaussians/) | [💻 Code](https://github.com/zju3dv/street_gaussians)

- **GigaGS: Scaling up Planar-Based 3D Gaussians for Large Scene Surface Reconstruction**, Chen et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2409.06685) | [💻 Code (Not Ready)](https://github.com/Open3DVLab/GigaGS)

- **[SIGGRAPH '24] A Hierarchical 3D Gaussian Representation for Real-Time Rendering of Very Large Datasets**, Kerbl et al., arXiv 2024 | [📄 Paper (Low Resolution)](https://repo-sam.inria.fr/fungraph/hierarchical-3d-gaussians/hierarchical-3d-gaussians_low.pdf) | [📄 Paper (High Resolution)](https://repo-sam.inria.fr/fungraph/hierarchical-3d-gaussians/hierarchical-3d-gaussians_high.pdf) | [🌐 Project Page](https://repo-sam.inria.fr/fungraph/hierarchical-3d-gaussians/)

- **Fed3DGS: Scalable 3D Gaussian Splatting with Federated Learning**, Suzuki et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.11460) | [💻 Code](https://github.com/DensoITLab/Fed3DGS)

- **Creating Seamless 3D Maps Using Radiance Fields**, Sathyan et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.11364.pdf)

- **HGS-Mapping: Online Dense Mapping Using Hybrid Gaussian Representation in Urban Scenes**, Wu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.20159.pdf)

- **CityGaussian: Real-time High-quality Large-Scale Scene Rendering with Gaussians**, Liu et al., arXiv 2024 |[📄 Paper](https://arxiv.org/pdf/2403.20159.pdf) | [🌐 Project Page](https://dekuliutesla.github.io/citygs/) | [💻 Code](https://github.com/DekuLiuTesla/CityGaussian)

- **MM-Gaussian: 3D Gaussian-based Multi-modal Fusion for Localization and Reconstruction in Unbounded Scenes**, Wu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2404.04026.pdf)

- **On Scaling Up 3D Gaussian Splatting Training**, Zhao et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2406.18533) | [🌐 Project Page](https://daohanlu.github.io/scaling-up-3dgs/) | [💻 Code](https://github.com/nyu-systems/Grendel-GS)
<br>


## 3D Reconstruction:
## 2025:
- **[CVPR' 25] DiffusionSfM: Predicting Structure and Motion via Ray Origin and Endpoint Diffusion**, Zhao et al., arXiv 2025 | [📄 Paper](https://www.arxiv.org/abs/2505.05473) | [🌐 Project Page](https://qitaozhao.github.io/DiffusionSfM) | [💻 Code](https://github.com/QitaoZhao/DiffusionSfM) | [🤗 Demo](https://huggingface.co/spaces/qitaoz/DiffusionSfM)

- **[ICLR' 25] MoDGS: Dynamic Gaussian Splatting from Casually-captured Monocular Videos with Depth Priors**, Liu et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2406.00434) | [🌐 Project Page](https://modgs.github.io/) | [💻 Code](https://github.com/MobiusLqm/MoDGS) | [🎥 Video](https://www.youtube.com/watch?si=IDZ6v6hLszZYFFoi&v=oBN3p716c_k&feature=youtu.be)

- **CasualHDRSplat: Robust High Dynamic Range 3D Gaussian Splatting from Casually Captured Videos**, Gong et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2504.17728) | [🌐 Project Page](https://lingzhezhao.github.io/CasualHDRSplat/) | [💻 Code](https://github.com/WU-CVGL/CasualHDRSplat)

- **PRISM: A Unified Framework for Photorealistic Reconstruction and Intrinsic Scene Modeling**, Dirik et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2504.14219) | [🌐 Project Page]() | [💻 Code]()

- **[RSS '25]Novel Demonstration Generation with Gaussian Splatting Enables Robust One-Shot Manipulation**, Yang et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2504.13175) | [🌐 Project Page](https://yangsizhe.github.io/robosplat/) | | [💻 Code](https://github.com/OpenRobotLab/robosplat)

- **[CVPR '25] V2V3D: View-to-View Denoised 3D Reconstruction for Light-Field Microscopy**, Zhao et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2504.07853) | [🌐 Project Page](https://joey1998hub.github.io/V2V3D/) | | [💻 Code]()

- **[CVPR '25] HiMoR: Monocular Deformable Gaussian Reconstruction with Hierarchical Motion Representation**, Liang et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2504.06210) | [🌐 Project Page](https://pfnet-research.github.io/himor/) | | [💻 Code]()

- **[CVPR '25] PartRM: Modeling Part-Level Dynamics with Large Cross-State Reconstruction Model**, Gao et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.19913) | [🌐 Project Page](https://partrm.c7w.tech/) | | [💻 Code](https://github.com/GasaiYU/PartRM)

- **Dynamic Point Maps: A Versatile Representation for Dynamic 3D Reconstruction**, Sucar et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.16318) | [🌐 Project Page](https://www.robots.ox.ac.uk/~vgg/research/dynamic-point-maps/) | | [💻 Code]()

- **GaussianCAD: Robust Self-Supervised CAD Reconstruction from Three Orthographic Views Using 3D Gaussian Splatting**, Zhou et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.05161v1) | [🌐 Project Page]() | | [💻 Code]()

- **MTGS: Multi-Traversal Gaussian Splatting**, Li et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.12552) | [🌐 Project Page]() | | [💻 Code]()

- **Amodal3R: Amodal 3D Reconstruction from Occluded 2D Images**, Wu et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.13439) | [💻 Code]() | [🌐 Project Page](https://sm0kywu.github.io/Amodal3R/) | [🤗 Demo](https://huggingface.co/spaces/Sm0kyWu/Amodal3R)

- **[CVPR '25] VGGT: Visual Geometry Grounded Transformer**, Wang et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.12894) | [💻 Code](https://github.com/facebookresearch/vggt) | [🌐 Project Page](https://vgg-t.github.io/) | [🤗 Demo](https://huggingface.co/spaces/facebook/vggt)

- **[CVPR '25] BARD-GS: Blur-Aware Reconstruction of Dynamic Scenes via Gaussian Splatting**, Lu et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.12894) | [💻 Code](https://github.com/vulab-AI/BARD-GS) | [🌐 Project Page](https://vulab-ai.github.io/BARD-GS/)

- **CAST: Component-Aligned 3D Scene Reconstruction from an RGB Image**, Yao et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.12894) | [💻 Code](https://github.com/NIRVANALAN/GaussianAnything) | [🌐 Project Page](https://sites.google.com/view/cast4) | [🎥 Video](https://www.youtube.com/watch?v=cloVLY6lWdI&feature=youtu.be)

- **[CVPR '25] MUSt3R: Multi-view Network for Stereo 3D Reconstruction**, Cabon et al., arXiv 2025 | [📄 Paper](https://www.arxiv.org/abs/2503.01661) | [🌐 Project Page]() | [💻 Code](https://github.com/naver/must3r)

- **Difix3D+: Improving 3D Reconstructions with Single-Step Diffusion Models**, Wu et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.03639v1) | [💻 Code]() | [🌐 Project Page](https://research.nvidia.com/labs/toronto-ai/difix3d/) | [🎥 Video](https://research.nvidia.com/labs/toronto-ai/difix3d/#demo_video)

- **Leverage Cross-Attention for End-to-End Open-Vocabulary Panoptic Reconstruction**, Yu et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.01119) | [🌐 Project Page](https://yuxuan1206.github.io/panopticrecon_pp/) | [💻 Code](https://github.com/yuxuan1206/PanopticRecon_plus) | [🎥 Video](https://www.bilibili.com/video/BV1pP61YuEbm/?vd_source=16bffa885f8d40c0678b340384dd56db)

- **FLARE: Feed-forward Geometry, Appearance and Camera Estimation from Uncalibrated Sparse Views**, Zhang et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.12138) | [🌐 Project Page](https://zhanghe3z.github.io/FLARE/) | [💻 Code](https://github.com/ant-research/FLARE) | [🤗 Demo](https://huggingface.co/AntResearch/FLARE)

- **Building Rome with Convex Optimization**, Han and Yang, arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.04640) | [🌐 Project Page](https://computationalrobotics.seas.harvard.edu/XM/) | [💻 Code]()

- **[CVPR '25]Fast3R: Towards 3D Reconstruction of 1000+ Images in One Forward Pass**, Yang et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.13928) | [🌐 Project Page](https://fast3r-3d.github.io/) | [💻 Code](https://github.com/facebookresearch/fast3r) | [🤗 Demo](https://fast3r.ngrok.app/)

- **Light3R-SfM: Towards Feed-forward Structure-from-Motion**, Elflein et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.14914)

- **VideoLifter: Lifting Videos to 3D with Fast Hierarchical Stereo Alignment**, Cong et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.01949) | [🌐 Project Page](https://videolifter.github.io/) | [💻 Code]()

- **[AAAI' 25]FatesGS: Fast and Accurate Sparse-View Surface Reconstruction using Gaussian Splatting with Depth-Feature Consistency**, Huang et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.04628) | [🌐 Project Page](https://alvin528.github.io/FatesGS/) | [💻 Code](https://github.com/yulunwu0108/FatesGS)

## 2024:
- **LiftImage3D: Lifting Any Single Image to 3D Gaussians with Video Generation Priors**, Chen et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2412.09597) | [🌐 Project Page](https://liftimage3d.github.io/) | [💻 Code](https://github.com/AbrahamYabo/LiftImage3D)

- **ReconX: Reconstruct Any Scene from Sparse Views with Video Diffusion Model**, Liu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2408.16767) | [🌐 Project Page](https://liuff19.github.io/ReconX/) | [💻 Code](https://github.com/liuff19/ReconX) | [🎥 Video](https://www.youtube.com/watch?v=UuL2nP5rJcI) | [🤗 Demo]()

- **CoSurfGS:Collaborative 3D Surface Gaussian Splatting with Distributed Learning for Large Scene Reconstruction**, Gao et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2412.17612) | [🌐 Project Page](https://gyy456.github.io/CoSurfGS/) | [💻 Code](https://github.com/zju3dv/CoSurfGS)

- **[ECCV' 24]latentSplat: Autoencoding Variational Gaussians for Fast Generalizable 3D Reconstruction**, Wewer et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2403.16292) | [🌐 Project Page](https://geometric-rl.mpi-inf.mpg.de/latentsplat/) | [💻 Code](https://github.com/Chrixtar/latentsplat)

- **Splatt3R: Zero-shot Gaussian Splatting from Uncalibrated Image Pairs**, Smart et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2408.13912) | [🌐 Project Page](https://splatt3r.active.vision/) | [💻 Code](https://github.com/btsmart/splatt3r)

- **[3DV' 25] 3D Reconstruction with Spatial Memory**, Wang and Agapito, arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2408.16061) | [🌐 Project Page](https://splatt3r.active.vision/) | [💻 Code](https://github.com/btsmart/splatt3r)

- **[CVPR' 25] CraftsMan: High-fidelity Mesh Generation with 3D Native Generation and Interactive Geometry Refiner**, Li et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2405.14979) | [🌐 Project Page](https://craftsman3d.github.io/) | [💻 Code](https://github.com/wyysf-98/CraftsMan3D) | [🤗 Demo](https://huggingface.co/spaces/wyysf/CraftsMan3D) | [🎥 Video](https://www.youtube.com/watch?v=WhEs4tS4mGo)

- **QGS: Quadratic Gaussian Splatting for Efficient and Detailed Surface Reconstruction**, Zhang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2411.16392) | [🌐 Project Page](https://quadraticgs.github.io/QGS/) | [💻 Code](https://github.com/QuadraticGS/QGS)

- **SplatFormer Point Transformer for Robust 3D Gaussian Splatting**, Chen et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2411.06390) | [🌐 Project Page](https://sergeyprokudin.github.io/splatformer/) | [💻 Code](https://github.com/ChenYutongTHU/SplatFormer)

- **[CVPR 2024 Oral, Best Paper Runner-Up] pixelSplat: 3D Gaussian Splats from Image Pairs for Scalable Generalizable 3D Reconstruction**, Charatan et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2312.12337) | [🌐 Project Page](https://davidcharatan.com/pixelsplat/) | [💻 Code](https://github.com/dcharatan/pixelsplat)

- **PGSR: Planar-based Gaussian Splatting for Efficient and High-Fidelity Surface Reconstruction**, Chen et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2406.06521.pdf) | [🌐 Project Page](https://zju3dv.github.io/pgsr/) | [💻 Code](https://github.com/zju3dv/PGSR)

- **Gaussian Opacity Fields: Efficient and Compact Surface Reconstruction in Unbounded Scenes**, Yu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2404.10772) | [🌐 Project Page](https://niujinshuchong.github.io/gaussian-opacity-fields/) | [💻 Code](https://github.com/autonomousvision/gaussian-opacity-fields)

- **3DGSR: Implicit Surface Reconstruction with 3D Gaussian Splatting**, Lyu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2404.00409) | [💻 Code](https://github.com/CVMI-Lab/3DGSR)

- **RTG-SLAM: Real-time 3D Reconstruction at Scale using Gaussian Splatting**, Peng et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2404.19706) | [💻 Code](https://github.com/Lab-of-AI-and-Robotics/GS_ICP_SLAM)

- **SA-GS: Semantic-Aware Gaussian Splatting for Large Scene Reconstruction with Geometry Constrain**, Xiong et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2405.16923) | [🌐 Project Page](https://saliteta.github.io/SA-GS-public/) | [💻 Code](https://github.com/saliteta/SA-GS-CODE/)

- **[CVPR '24]SuGaR: Surface-Aligned Gaussian Splatting for Efficient 3D Mesh Reconstruction and High-Quality Mesh Rendering**, Guedon and Lepetit, arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2311.12775) | [🌐 Project Page](https://anttwo.github.io/sugar/) | [💻 Code](https://github.com/waczjoan/gaussian-mesh-splatting)

- **GaMeS: Mesh-Based Adapting and Modification of Gaussian Splatting**, Waczynska et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2402.01459) | [💻 Code](https://github.com/Anttwo/SuGaR)

- **Direct Learning of Mesh and Appearance via 3D Gaussian Splatting**, Lin and Li, arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2405.06945)



## Gaussian Surfel:
## 2024:
- **[SIGGRAPH '24]High-quality Surface Reconstruction using Gaussian Surfels**, Dai et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2404.17774) | [🌐 Project Page](https://turandai.github.io/projects/gaussian_surfels/) | [💻 Code](https://github.com/turandai/gaussian_surfels)

- **[SIGGRAPH '24]2D Gaussian Splatting for Geometrically Accurate Radiance Fields**, Huang et al., SIGGRAPH 2024 | [📄 Paper](https://arxiv.org/pdf/2402.03246.pdf) | [🌐 Project Page](https://surfsplatting.github.io/) | [💻 Code](https://github.com/hbb1/2d-gaussian-splatting)

## 2023:
- **[CVPR '23]SurfelNeRF: Neural Surfel Radiance Fields for Online Photorealistic
Reconstruction of Indoor Scenes**, Gao et al., CVPR 2023 | [📄 Paper](https://openaccess.thecvf.com/content/CVPR2023/papers/Gao_SurfelNeRF_Neural_Surfel_Radiance_Fields_for_Online_Photorealistic_Reconstruction_of_CVPR_2023_paper.pdf) | [🌐 Project Page](https://gymat.github.io/SurfelNeRF-web/) | [💻 Code](https://github.com/Gymat/SurfelNeRF/tree/unofficial)

## Theory:
- **Surfels: Surface Elements as Rendering Primitives**, Pfister et al., CGIT 2000 | [📄 Paper](https://www.cs.umd.edu/~zwicker/publications/Surfels-SIG00.pdf)

## Surfel based SLAM:
- **Efficient Surfel-Based SLAM using 3D Laser Range Data in Urban Environments**, Behley and Stachniss, RSS 2018 | [📄 Paper](https://jbehley.github.io/papers/behley2018rss.pdf) | [🌐 Project Page](https://jbehley.github.io/projects/surfel_mapping/index.html) | [💻 Code](https://github.com/jbehley/SuMa)

- **Real-time Scalable Dense Surfel Mapping**, Wang et al., arXiv 2019 | [📄 Paper](https://arxiv.org/abs/1909.04250) | [💻 Code](https://github.com/HKUST-Aerial-Robotics/DenseSurfelMapping)

- **Surfel-based RGB-D Reconstruction and SLAM with Global and Local Consistency**, Yang, Msc thesis 2019 | [📄 Paper](https://www.cs.cmu.edu/~kaess/pub/Yang19thesis_ms.pdf)


## 3D Generations:
## 2025:
- **[TECHINICAL REPORT] Step1X-3D: Towards High-Fidelity and Controllable Generation of Textured 3D Assets**, Li et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2505.07747) | [💻 Code](https://github.com/stepfun-ai/Step1X-3D) | [🌐 Project Page](https://stepfun-ai.github.io/Step1X-3D/) | [🤗 Demo](https://huggingface.co/spaces/stepfun-ai/Step1X-3D)

- **[SIGGRAPH '25] 3D-Fixup: Advancing Photo Editing with 3D Priors**, Cheng et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2505.10566) | [💻 Code]() | [🌐 Project Page](https://3dfixup.github.io/)

- **Bolt3D: Generating 3D Scenes in Seconds**, Szymanowicz et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.14445) | [💻 Code]() | [🌐 Project Page](https://szymanowiczs.github.io/bolt3d)

- **Scenethesis: A Language and Vision Agentic Framework for 3D Scene Generation**, Ling et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2505.02836) | [💻 Code]() | [🌐 Project Page](https://research.nvidia.com/labs/dir/scenethesis/)

- **[ICLR '25] 3DitScene: Editing Any Scene via Language-guided Disentangled Gaussian Splatting**, Zhang et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2405.18424) | [💻 Code](https://github.com/zqh0253/3DitScene) | [🌐 Project Page](https://zqh0253.github.io/3DitScene/) | [🤗 Demo](https://huggingface.co/spaces/qihang/3Dit-Scene)

- **[CVPR '25] ERUPT: Efficient Rendering with Unposed Patch Transformer**, Shugaev et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.24374) | [💻 Code]() | [🌐 Project Page]()

- **3DAffordSplat: Efficient Affordance Reasoning with 3D Gaussians**, Wei et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2504.11218) | [💻 Code](https://github.com/HCPLab-SYSU/3DAffordSplat) | [🤗 Data]()

- **[CVPR '25] GEN3C: 3D-Informed World-Consistent Video Generation with Precise Camera Control**, Ren et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.03751) | [💻 Code]() | [🌐 Project Page](https://research.nvidia.com/labs/toronto-ai/GEN3C/)

- **[CVPR '25] PhysGen3D: Crafting a Miniature Interactive World from a Single Image**, Chen et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.20746) | [💻 Code](https://github.com/by-luckk/PhysGen3D) | [🌐 Project Page](https://by-luckk.github.io/PhysGen3D/)

- **Hi3DGen: High-fidelity 3D Geometry Generation from Images via Normal Bridging**, Ye et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.22236) | [💻 Code](https://github.com/Stable-X/Hi3DGen) | [🌐 Project Page](https://stable-x.github.io/Hi3DGen/) | [🤗 Demo](https://huggingface.co/spaces/Stable-X/Hi3DGen)

- **[CVPR '25] VideoScene: Distilling Video Diffusion Model to Generate 3D Scenes in One Step**, Wang et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2504.01956) | [💻 Code](https://github.com/hanyang-21/VideoScene) | [🌐 Project Page](https://hanyang-21.github.io/VideoScene/)

- **WorldScore: A Unified Evaluation Benchmark for World Generation**, Duan et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2504.00983) | [💻 Code](https://github.com/haoyi-duan/WorldScore) | [🌐 Project Page](https://haoyi-duan.github.io/WorldScore/) | [🤗 Leaderboard](https://huggingface.co/spaces/Howieeeee/WorldScore_Leaderboard)

- **WonderTurbo: Generating Interactive 3D World in 0.72 Seconds**, Ni et al., arXiv 2025 | [📄 Paper](https://www.arxiv.org/abs/2504.02261) | [💻 Code](https://github.com/GigaAI-research/WonderTurbo) | [🌐 Project Page](https://wonderturbo.github.io/)

- **DeepMesh: Auto-Regressive Artist-mesh Creation with Reinforcement Learning**, Zhao et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.15265) | [💻 Code](https://github.com/zhaorw02/DeepMesh) | [🌐 Project Page](https://zhaorw02.github.io/DeepMesh/) | [🎥 Video](https://www.youtube.com/watch?v=6grL7bSbQ2w)

- **Controllable 3D Outdoor Scene Generation via Scene Graphs**, Liu et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.07152) | [💻 Code](https://github.com/yuhengliu02/control-3d-scene) | [🌐 Project Page](https://yuheng.ink/project-page/control-3d-scene/)

- **GAS: Generative Avatar Synthesis from a Single Image**, Lu et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.06957) | [💻 Code](https://github.com/humansensinglab/GAS) | [🌐 Project Page](https://humansensinglab.github.io/GAS/)

- **FlexWorld: Progressively Expanding 3D Scenes for Flexiable-View Synthesis**, Chen et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.13265) | [💻 Code](https://github.com/ML-GSAI/FlexWorld) | [🌐 Project Page](https://ml-gsai.github.io/FlexWorld/)

- **TripoSG: High-Fidelity 3D Shape Synthesis using Large-Scale Rectified Flow Models**, Li et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.06608) | [💻 Code](https://github.com/VAST-AI-Research/TripoSG) | [🌐 Project Page](https://yg256li.github.io/TripoSG-Page/) | [🎥 Video](https://lidan233.github.io/caddreamer/static/videos/CADDreamer-Video.mp4) | [🤗 Demo](https://huggingface.co/spaces/VAST-AI/TripoSG)

- **[CVPR '25]CADDreamer: CAD object Generation from Single-view Images**, Li et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.20732) | [💻 Code](https://github.com/lidan233/CADDreamer) | [🌐 Project Page](https://lidan233.github.io/caddreamer/) | [🎥 Video](https://lidan233.github.io/caddreamer/static/videos/CADDreamer-Video.mp4)

- **CAST: Component-Aligned 3D Scene Reconstruction from an RGB Image**, Yao et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.12894) | [💻 Code](https://github.com/NIRVANALAN/GaussianAnything) | [🌐 Project Page](https://sites.google.com/view/cast4) | [🎥 Video](https://www.youtube.com/watch?v=cloVLY6lWdI&feature=youtu.be)

- **[IROS '25]Uni-Gaussians: Unifying Camera and Lidar Simulation with Gaussians for Dynamic Driving Scenarios**, Yuan et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.08317)

- **[CVPR '25]Taming Video Diffusion Prior with Scene-Grounding Guidance for 3D Gaussian Splatting from Sparse Inputs**, Zhong et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2503.05082) | [💻 Code](https://github.com/zhongyingji/guidedvd-3dgs) | [🌐 Project Page](https://zhongyingji.github.io/guidevd-3dgs/)

- **GaussianAnything: Interactive Point Cloud Latent Diffusion for 3D Generation**, Lan et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2411.08033) | [💻 Code](https://github.com/NIRVANALAN/GaussianAnything) | [🌐 Project Page](https://nirvanalan.github.io/projects/GA/) | [🤗 Demo](https://huggingface.co/spaces/yslan/GaussianAnything-AIGC3D)

- **Difix3D+: Improving 3D Reconstructions with Single-Step Diffusion Models**, Wu et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.03639v1) | [💻 Code]() | [🌐 Project Page](https://research.nvidia.com/labs/toronto-ai/difix3d/) | [🎥 Video](https://research.nvidia.com/labs/toronto-ai/difix3d/#demo_video)

- **Towards Physical Understanding in Video Generation: A 3D Point Regularization Approach**, Chen et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.03639v1) | [💻 Code](https://github.com/snap-research/PointVidGen) | [🌐 Project Page](https://snap-research.github.io/PointVidGen/)

- **Fractal Generative Models**, Li et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.17437) | [💻 Code](https://github.com/LTH14/fractalgen)

- **TANGLED: Generating 3D Hair Strands from Images with Arbitrary Styles and Viewpoints**, Long et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2502.06392) | [🌐 Project Page](https://sites.google.com/view/tangled1) | [💻 Code]() | [🎥 Video](https://www.youtube.com/watch?v=msigozrOV7U) 

- **Hunyuan3D 2.0: Scaling Diffusion Models for High Resolution Textured 3D Assets Generation**, Zhao et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.12202) | [🌐 Project Page](https://3d-models.hunyuan.tencent.com/) | [💻 Code](https://github.com/Tencent/Hunyuan3D-2) | [🤗 Demo](https://huggingface.co/spaces/tencent/Hunyuan3D-2) 

- **Orchid: Image Latent Diffusion for Joint Appearance and Geometry Generation**, Krishnan et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.13087v1) | [🌐 Project Page](https://orchid3d.github.io/) | [💻 Code]()

- **CityDreamer4D: Compositional Generative Model of Unbounded 4D Cities**, Xie et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.08983) | [🌐 Project Page](https://www.infinitescript.com/project/city-dreamer-4d) | [💻 Code](https://github.com/hzxie/CityDreamer4D) | [🎥 Video](https://www.youtube.com/watch?v=PF6W0Nd27Tk) 

- **SPAR3D: Stable Point-Aware Reconstruction of 3D Objects from Single Images**, Huang et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.04689) | [🌐 Project Page](https://spar3d.github.io/) | [💻 Code](https://github.com/Stability-AI/stable-point-aware-3d) | [🎥 Video](https://www.youtube.com/watch?v=mlO3Nc3Nsng) | [🤗 Demo](https://huggingface.co/spaces/stabilityai/stable-point-aware-3d)

- **GPT4Scene: Understand 3D Scenes from Videos with Vision-Language Models**, Hu et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2412.19505) | [🌐 Project Page](https://huxiaotaostasy.github.io/DrivingWorld/index.html) | [💻 Code](https://github.com/Qi-Zhangyang/gpt4scene)

- **[NVIDIA]Cosmos World Foundation Model Platform for Physical AI**, Agarwal et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2501.03575) | [🌐 Project Page](https://research.nvidia.com/labs/dir/cosmos1/) | [💻 Code](https://github.com/NVIDIA/Cosmos) | [🎥 Video](https://www.youtube.com/watch?v=9Uch931cDx8) | [🤗 Demo](https://huggingface.co/collections/nvidia/cosmos-6751e884dc10e013a0a0d8e6)

## 2024:
- **[CVPR '25] MultiGO: Towards Multi-level Geometry Learning for Monocular 3D Textured Human Reconstruction**, Zhang et al., arXiv 2025 | [📄 Paper](https://arxiv.org/abs/2412.03103) | [💻 Code]() | [🌐 Project Page](https://multigohuman.github.io/)

- **[CVPR '25]MIDI: Multi-Instance Diffusion for Single Image to 3D Scene Generation**, Huang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2412.03558) | [💻 Code](https://github.com/VAST-AI-Research/MIDI-3D) | [🌐 Project Page](https://huanngzh.github.io/MIDI-Page/) | [🤗 Demo](https://huggingface.co/spaces/VAST-AI/MIDI-3D)

- **Prometheus: 3D-Aware Latent Diffusion Models for Feed-Forward Text-to-3D Scene Generation**, Yang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2412.21117) | [🌐 Project Page](https://freemty.github.io/project-prometheus/) | [💻 Code](https://github.com/XDimLab/Prometheus) | [🎥 Video](https://www.youtube.com/watch?v=N_L_ecSiIJA)

- **PanoDreamer: 3D Panorama Synthesis from a Single Image**, Paliwal et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2412.04827) | [💻 Code](https://github.com/avinashpaliwal/PanoDreamer) | [🌐 Project Page](https://people.engr.tamu.edu/nimak/Papers/PanoDreamer/index.html) | [🎥 Video](https://www.youtube.com/watch?v=EyVfFCg4aF8) 

- **[CVPR' 25]StdGEN: Semantic-Decomposed 3D Character Generation from Single Images**, He et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2411.05738) | [🌐 Project Page](https://stdgen.github.io/ | [💻 Code](https://github.com/hyz317/StdGEN) | [🎥 Demo](https://huggingface.co/spaces/hyz317/StdGEN)

- **[NeurIPS' 24]GenWarp: Single Image to Novel Views with Semantic-Preserving Generative Warping**, Seo et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2405.17251) | [🌐 Project Page](https://genwarp-nvs.github.io/) | [💻 Code](https://github.com/sony/genwarp) | [🤗 Demo](https://huggingface.co/spaces/Sony/genwarp)

- **PartGen: Part-level 3D Generation and Reconstruction with Multi-View Diffusion Models**, Chen et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2412.18608) | [🌐 Project Page](https://silent-chen.github.io/PartGen/) | [💻 Code]() | [🎥 Explanation Video](https://www.youtube.com/watch?v=Ma_Nk85L3d4)

- **[CVPR '25]Generative Gaussian Splatting for Unbounded 3D City Generation**, Xie et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2406.06526) | [🌐 Project Page](https://www.infinitescript.com/project/gaussian-city/) | [💻 Code](https://github.com/hzxie/GaussianCity) | [🤗 Demo](https://huggingface.co/spaces/hzxie/gaussian-city) | [🎥Video](https://www.youtube.com/watch?v=anDwIXlfjUA)

- **[ECCV '24]SplatFields: Neural Gaussian Splats for Sparse 3D and 4D Reconstruction**, Mihajlovic et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2409.11211) | [🌐 Project Page](https://markomih.github.io/SplatFields/) | [💻 Code](https://github.com/markomih/SplatFields)

- **[ECCV '24]Pyramid Diffusion for Fine 3D Large Scene Generation**, Liu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2311.12085) | [🌐 Project Page](https://yuheng.ink/project-page/pyramid-discrete-diffusion/) | [💻 Code](https://github.com/yuhengliu02/pyramid-discrete-diffusion) | [🎥 Video](https://www.youtube.com/watch?v=9EmUq4cnyGM) 

- **LaRa: Efficient Large-Baseline Radiance Fields**, Chen et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2407.04699) | [🌐 Project Page](https://apchenstu.github.io/LaRa/) | [💻 Code](https://github.com/autonomousvision/LaRa)

- **Real3D: Scaling Up Large Reconstruction Models with Real-World Images**, Jiang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2406.08479) | [🌐 Project Page](https://hwjiang1510.github.io/Real3D/) | [💻 Code](https://github.com/hwjiang1510/Real3D) | [🤗 Demo](https://huggingface.co/spaces/hwjiang/Real3D)

- **CAT4D: Create Anything in 4D with Multi-View Video Diffusion Models**, Wu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2412.12096) | [🌐 Project Page](https://cat-4d.github.io/) | [💻 Code](https://github.com/aigc3d/AniGS)

- **AniGS: Animatable Gaussian Avatar from a Single Image with Inconsistent Gaussian Reconstruction**, Qiu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2412.02684) | [🌐 Project Page](https://lingtengqiu.github.io/2024/AniGS/) | [💻 Code](https://github.com/aigc3d/AniGS) | [🎥 Video](https://www.youtube.com/watch?v=e9qgMMvYMr4)

- **PanSplat: 4K Panorama Synthesis with Feed-Forward Gaussian Splatting**, Zhang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2412.12096) | [🌐 Project Page](https://chengzhag.github.io/publication/pansplat/) | [💻 Code](https://github.com/chengzhag/PanSplat)

- **DrivingWorld: Constructing World Model for Autonomous Driving via Video GPT**, Qi et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2501.01428) | [🌐 Project Page](https://gpt4scene.github.io/) | [💻 Code](https://github.com/YvanYin/DrivingWorld)

- **[3DV' 25]RealmDreamer: Text-Driven 3D Scene Generation with Inpainting and Depth Diffusion**, Shriram et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2404.07199) | [🌐 Project Page](https://realmdreamer.github.io/) | [💻 Code](https://github.com/jaidevshriram/realmdreamer)

- **InfiniCube: Unbounded and Controllable Dynamic 3D Driving Scene Generation with World-Guided Video Models**, Lu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2412.03934) | [🌐 Project Page](https://research.nvidia.com/labs/toronto-ai/infinicube/) | [💻 Code]()

- **[AAAI' 25]SceneX: Procedural Controllable Large-scale Scene Generation**, Zhou et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2403.15698) | [🌐 Project Page](https://zhouzq1.github.io/SceneX/) | [💻 Code](https://github.com/zhouzq1/SceneX)

- **[CVPR' 24]One-2-3-45++: Fast Single Image to 3D Objects with Consistent Multi-View Generation and 3D Diffusion**, Liu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2311.07885) | [🌐 Project Page](https://sudo-ai-3d.github.io/One2345plus_page/) | [💻 Code](https://github.com/SUDO-AI-3D/One2345plus) | [🤗 Demo](https://www.sudo.ai/3dgen)

- **[CVPR' 24]DIRECT-3D: Learning Direct Text-to-3D Generation on Massive Noisy 3D Data**, Liu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2406.04322) | [🌐 Project Page](https://direct-3d.github.io/) | [💻 Code](https://github.com/qihao067/direct3d)

- **PanoDreamer: 3D Panorama Synthesis from a Single Image**, Paliwal et al., arXiv 2024 | [📄 Paper](http://arxiv.org/abs/2412.04827v1) | [🌐 Project Page](https://people.engr.tamu.edu/nimak/Papers/PanoDreamer) | [💻 Code](https://github.com/avinashpaliwal/PanoDreamer)

- **[CVPR '25]Structured 3D Latents for Scalable and Versatile 3D Generation**, Xiang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2412.01506) | [🌐 Project Page](https://trellis3d.github.io/) | [💻 Code](https://github.com/microsoft/TRELLIS)

- **DimensionX: Create Any 3D and 4D Scenes from a Single Image with Controllable Video Diffusion**, Sun et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2411.04928) | [🌐 Project Page](https://chenshuo20.github.io/DimensionX/) | [💻 Code](https://github.com/wenqsun/DimensionX) | [🤗 Demo](https://huggingface.co/spaces/fffiloni/DimensionX)

- **Segment Any 4D Gaussians**, Ji et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2407.04504v2) | [🌐 Project Page](https://jsxzs.github.io/sa4d/) | [💻 Code](https://github.com/jsxzs/SA4D)

- **[ECCV 2024 Oral] LGM: Large Multi-View Gaussian Model for High-Resolution 3D Content Creation**, Ren et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2402.05054) | [🌐 Project Page](https://me.kiui.moe/lgm/) | [💻 Code](https://github.com/3DTopia/LGM)

- **[NeurIPS' 24] SCube: Instant Large-Scale Scene Reconstruction using VoxSplats**, Ren et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2410.20030) | [🌐 Project Page](https://research.nvidia.com/labs/toronto-ai/scube/) | [💻 Code](https://github.com/nv-tlabs/SCube)

- **DiffusionGS: Baking Gaussian Splatting into Diffusion Denoiser for Fast and Scalable Single-stage Image-to-3D Generation**, Cai et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2411.14384v1) | [🌐 Project Page](https://caiyuanhao1998.github.io/project/DiffusionGS/) | [💻 Code](https://github.com/caiyuanhao1998/Open-DiffusionGS)

- **VistaDream Sampling multiview consistent images for single-view scene reconstruction**, Wang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2410.16892) | [🌐 Project Page](https://vistadream-project-page.github.io/l) | [💻 Code](https://github.com/WHU-USI3DV/VistaDream)

- **[ICLR' 24]DreamFlow: High-Quality Text-to-3D Generation by Approximating Probability Flow**, Lee et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2403.14966) | [🌐 Project Page](https://kyungmnlee.github.io/dreamflow.github.io/) | [💻 Code]()

## 2023:
- **[CVPR' 24]XCube: Large-Scale 3D Generative Modeling using Sparse Voxel Hierarchies**, Ren et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2312.03806) | [🌐 Project Page](https://research.nvidia.com/labs/toronto-ai/xcube/) | [💻 Code](https://github.com/nv-tlabs/XCube) | [🎥 Video](https://www.youtube.com/watch?v=GX0lzwy8nUI)

- **[CVPR' 24]Wonder3D: Single Image to 3D using Cross-Domain Diffusion**, Long et al., arXiv 2023 | [📄 Paper](https://arxiv.org/abs/2310.15008) | [🌐 Project Page](https://www.xxlong.site/Wonder3D/) | [💻 Code](https://github.com/xxlong0/Wonder3D) | [🤗 Demo](https://huggingface.co/spaces/flamehaze1115/Wonder3D-demo)


## Data
- [Digital Twin Catalog for object reconstruction](https://www.projectaria.com/datasets/dtc/)

- [uCO3D High resolution object dataset with more than 1000 categories](https://github.com/facebookresearch/uco3d)

- [NERDS 360 Multi-View dataset for Outdoor Scenes](https://zubair-irshad.github.io/projects/neo360.html)

<br>


## Courses
- [MIT Inverse Rendering Lectures (Module 2)](https://www.scenerepresentations.org/courses/inverse-graphics-23/)

<br>


## Open Source Implementations
### Unofficial Implementations

|                                                                                             | Language       | License    |
| ------------------------------------------------------------------------------------------- | -------------- | ---------- |
| [Taichi 3D Gaussian Splatting](https://github.com/wanmeihuali/taichi_3d_gaussian_splatting) | taichi         | Apache-2.0 |
| [Gaussian Splatting 3D](https://github.com/heheyas/gaussian_splatting_3d)                   | Python/CUDA    |            |
| [3D Gaussian Splatting](https://github.com/WangFeng18/3d-gaussian-splatting)                | Python/CUDA    | MIT        |
| [fast](https://github.com/MrNeRF/gaussian-splatting-cuda)                                   | C++/CUDA       | Inria/MPII |
| [nerfstudio](https://github.com/nerfstudio-project/gsplat)                                  | Python/CUDA    | Apache-2.0 |
| [taichi-splatting](https://github.com/uc-vision/taichi-splatting)                           | taichi/PyTorch | Apache-2.0 |
| [OpenSplat](https://github.com/pierotofy/OpenSplat)                                         | C++/CPU or GPU | AGPL-3.0   |
| [3D Gaussian Splatting](https://github.com/joeyan/gaussian_splatting)                       | Python/CUDA    | MIT        |
| [Grendel Distributed 3DGS](https://github.com/nyu-systems/Grendel-GS)                       | Python/CUDA    | Apache-2.0 |
| [GauStudio]https://github.com/GAP-LAB-CUHK-SZ/gaustudio)                       | Python/CUDA    | MIT |

### 2D Gaussian Splatting
- [jupyter notebook 2D GS splatting](https://github.com/OutofAi/2D-Gaussian-Splatting)
- [2.5D GS splatting](https://github.com/hugoycj/2.5d-gaussian-splatting)
- [2d Gaussian diff rasterization](https://github.com/Yubel426/diff-gaussian-rasterization/tree/2dgs)

### Gaussian Style Transfer

- [Direct Gaussian Style Optimization (DGSO): Stylizing 3D Gaussian Splats](https://github.com/An-u-rag/stylized-gaussian-splatting) - Applying style transfer during gaussian optimization to produce stylized gaussian splats of a scene.

### Game Engines

- [Unity](https://github.com/aras-p/UnityGaussianSplatting)
- [PlayCanvas](https://github.com/playcanvas/engine/tree/main/extras/splat)
- [Unreal](https://github.com/xverse-engine/XV3DGS-UEPlugin)

### Viewers

- [WebGL Viewer 1](https://github.com/antimatter15/splat)
- [WebGL Viewer 2](https://github.com/kishimisu/Gaussian-Splatting-WebGL)
- [WebGL Viewer 3](https://github.com/BladeTransformerLLC/gauzilla)
- [WebGPU Viewer 1](https://github.com/cvlab-epfl/gaussian-splatting-web)
- [WebGPU Viewer 2](https://github.com/MarcusAndreasSvensson/gaussian-splatting-webgpu)
- [WebGPU Viewer 3](https://github.com/KeKsBoTer/web-splat)
- [Three.js](https://github.com/mkkellogg/GaussianSplats3D)
- [A-Frame](https://github.com/quadjr/aframe-gaussian-splatting)
- [Nerfstudio Unofficial](https://github.com/yzslab/nerfstudio/tree/gaussian_splatting)
- [Nerfstudio Viser](https://github.com/nerfstudio-project/viser)
- [Blender (Editor)](https://github.com/ReshotAI/gaussian-splatting-blender-addon/tree/master)
- [WebRTC viewer](https://github.com/dylanebert/gaussian-viewer)
- [iOS & Metal viewer](https://github.com/laanlabs/metal-splats)
- [jupyter notebook](https://github.com/shumash/gaussian-splatting/blob/mshugrina/interactive/interactive.ipynb)
- [PyOpenGL viewer (also with official CUDA backend)](https://github.com/limacv/GaussianSplattingViewer.git)
- [PlayCanvas Viewer](https://github.com/playcanvas/model-viewer)
- [gsplat.js](https://github.com/dylanebert/gsplat.js)
- [Splatapult](https://github.com/hyperlogic/splatapult) - 3d gaussian splatting renderer in C++ and OpenGL, works with OpenXR for tethered VR
- [3DGS.cpp](https://github.com/shg8/3DGS.cpp) - cross-platform, high performance 3DGS renderer in C++ and Vulkan Compute, supporting Windows, macOS, Linux, iOS, and visionOS
- [vkgs](https://github.com/jaesung-cs/vkgs) - cross-platform, high performance 3DGS renderer in C++ and Vulkan Compute/Graphics
- [Gaussian Viewer](https://github.com/Florian-Barthel/gaussian_viewer) - Loads also Compact3D plys.
- [spaTV](https://github.com/antimatter15/splaTV) - WebGL Viewer for 4D Gaussians (based on SpaceTime Gaussian) with demo [here](http://antimatter15.com/splaTV/)
- [Taichi Viewer](https://github.com/uc-vision/splat-viewer)
- [uc-vision-splat-viewer](https://github.com/uc-vision/splat-viewer)(3D gaussin splatting renderer with benchmarking capability)
- [2d gaussian viewer](https://github.com/hwanhuh/2D-GS-Viser-Viewer)(2D gaussian splatting WebGPU viewer with Viser)
- [SuperSplat viewer](https://playcanvas.com/supersplat/editor)(SuperSplat 3d gaussian viewer)

### Utilities

- [Kapture](https://github.com/naver/kapture) - A unified data format to facilitate visual localization and structure from motion e.g. for bundler to colmap model conversion
- [Kapture image cropper script](https://gist.github.com/jo-chemla/258e6e40d3d6c2220b29518ff3c17c40) - Undistorted image cropper script to remove black borders with included conversion instructions
- [camorph](https://github.com/Fraunhofer-IIS/camorph) - A toolbox for conversion between camera parameter conventions e.g. Reality Capture to colmap model
- [3DGS Converter](https://github.com/francescofugazzi/3dgsconverter) - A tool for converting 3D Gaussian Splatting .ply files into a format suitable for Cloud Compare and vice-versa
- [SuperSplat](https://github.com/playcanvas/super-splat) - Open source browser-based tool to clean/filter, reorient and compress .ply/.splat files
- [SpectacularAI](https://github.com/SpectacularAI/point-cloud-tools) - Conversion scripts for different 3DGS conventions
- [GSOPs](https://github.com/david-rhodes/GSOPs) - GSOPs (Gaussian Splat Operators) for SideFX Houdini. Import, edit, and export models, or generate synthetic training data

### Tutorial

- [Tutorial from the authors of 3DGS](https://3dgstutorial.github.io/)
- [3D Gaussian Splatting Tutorial](https://3dgstutorial.github.io/), Kopanas et al., 3DV 2024 
- [3DGS render in Python](https://github.com/SY-007-Research/3dgs_render_python)

### Framework

- [msplat](https://github.com/pointrix-project/msplat) - A modular differential gaussian rasterization library.
- [GauStudio](https://github.com/GAP-LAB-CUHK-SZ/gaustudio) - Unified framework with different paper implementations
- [gaussian-splatting-lightning](https://github.com/yzslab/gaussian-splatting-lightning) - A 3D Gaussian Splatting framework with various derived algorithms and an interactive web viewer
- [gsplat](https://github.com/nerfstudio-project/gsplat) - Part of the NerfStudio project, a 3D Gaussian Splatting framework with various derived algorithms and an interactive web viewer.

### Other

- [My-exp-Gaussians](https://github.com/ingra14m/My-exp-Gaussians) - Enhancing the ability of 3D Gaussians to model complex scenes
- [360-gaussian-splatting](https://github.com/inuex35/360-gaussian-splatting) - Generate gaussian splatting directly from 360 images

## Blog Posts

1. [Gaussian Splatting is pretty cool](https://aras-p.info/blog/2023/09/05/Gaussian-Splatting-is-pretty-cool/)
2. [Making Gaussian Splats smaller](https://aras-p.info/blog/2023/09/13/Making-Gaussian-Splats-smaller/)
3. [Making Gaussian Splats more smaller](https://aras-p.info/blog/2023/09/27/Making-Gaussian-Splats-more-smaller/)
4. [Very good (technical) intro to 3D Gaussian Splatting](https://medium.com/@AriaLeeNotAriel/numbynum-3d-gaussian-splatting-for-real-time-radiance-field-rendering-kerbl-et-al-60c0b25e5544)
5. [Write up on some mathematical details of the 3DGS implementation](https://github.com/kwea123/gaussian_splatting_notes)
6. [Discussion about gs universal format](https://github.com/mkkellogg/GaussianSplats3D/issues/47#issuecomment-1801360116)
7. [Math explanation to understand 3DGS](https://github.com/chiehwangs/3d-gaussian-theory)
8. [Compressing Gaussian Splats](https://blog.playcanvas.com/compressing-gaussian-splats/)
9. [Comprehensive overview of Gaussian Splatting](https://towardsdatascience.com/a-comprehensive-overview-of-gaussian-splatting-e7d570081362)
10. [Gaussian Head Avatars: A Summary](https://towardsdatascience.com/gaussian-head-avatars-a-summary-2bd17bd48500)
11. [NeRFs vs. 3DGS](https://edwardahn.me/writing/NeRFvs3DGS/)
12. [Howto capture images for 3DGS](https://medium.com/@heyulei/capture-images-for-gaussian-splatting-81d081bbc826)
13. [Mathematical details of forward and backward passes](https://github.com/joeyan/gaussian_splatting/blob/main/MATH.md)
14. [3D in Geospatial: NeRFs, Gaussian Splatting, and Spatial Computing](https://ckoziol.com/blog/2024/radiance_methods/)
15. [NeRFs vs. 3DGS Comprehensive Overview](https://towardsdatascience.com/a-comprehensive-overview-of-gaussian-splatting-e7d570081362)

## Tutorial Videos

1. [Getting Started with 3DGS for Windows](https://youtu.be/UXtuigy_wYc?si=j1vfORNspcocSH-b)
2. [How to view 3DGS Scenes in Unity](https://youtu.be/5_GaPYBHqOo?si=6u9j1HqXwF_5WSUL)
3. [Jupyter notebook tutorial](https://www.youtube.com/watch?v=OcvA7fmiZYM&t=2s)
4. [Intro to gaussian splatting (and Unity plugin)](https://www.xuanprada.com/blog/2023/10/22/intro-to-gaussian-splatting)
5. [Comprehensive 3DGS explanation](https://youtu.be/VkIJbpdTujE?si=1GLjzBfF9LCuT22o)

## Credits

Most credits should be contributed to [Awesome 3D Gaussian Splatting](https://github.com/MrNeRF/awesome-3D-gaussian-splatting?tab=readme-ov-file#slam), [3D Gaussian Splatting Papers](https://github.com/Awesome3DGS/3D-Gaussian-Splatting-Papers)

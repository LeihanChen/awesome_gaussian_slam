# Awesome Gaussian SLAM Resources

A curated list of papers and open-source resources focused on gaussian based slam system, focusing on slam systems with gaussian based mapping representation with any utilities. The ambition is keeping pace with the anticipated surge of research in the coming months. If you have any additions or suggestions, feel free to contribute. Additional resources like blog posts, videos, etc. are also welcome.

## Table of contents

- [Seminal Introduction Material](#introduction)

  - [Nerf](#nerf)
  - [3D Gaussian Splatting](#3d-gaussian-splatting)
    <br>

- [Survey](#survey)
- [Theory](#gaussian-theory)
- [Gaussian SLAM](#gaussian-slam)
- [Navigation](#navigation)
- [Poses](#poses)
- [Large-Scale](#large-scale)
- [3D Reconstruction](#3d-reconstruction)
- [Gaussian Surfel ](#gaussian-surfel)
- [3D Generation ](#3D-Generations)
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
</details>

<br>

## Introduction:

### Nerf:
- [NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis](https://www.matthewtancik.com/nerf), Mildenhall et al., ECCV 2020 | [📄 Paper](https://arxiv.org/abs/2003.08934.pdf) | [💻 Code](https://github.com/bmild/nerf)

### 3D Gaussian Splatting:
- [3D Gaussian Splatting for Real-Time Radiance Field Rendering](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/), Kerbl et al., SIGGRAPH 2023 | [📄 Paper](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/3d_gaussian_splatting_high.pdf) | [💻 Code](https://github.com/graphdeco-inria/gaussian-splatting) | [🎥 Short Presentation](https://youtu.be/T_kXY43VZnk?si=DrkbDFxQAv5scQNT) | [🎥 Explanation Video](https://www.youtube.com/live/xgwvU7S0K-k?si=edF8NkYtsRbgTbKi)
<br>

## Survey:
- **Scene reconstruction techniques for autonomous driving: a review of 3D Gaussian splatting**, Zhu et al., Artificial Intelligence Review 2024 | [📄 Paper](https://link.springer.com/content/pdf/10.1007/s10462-024-10955-4.pdf)

- **A Survey on 3D Gaussian Splatting**, Chen et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2401.03890.pdf)

- **How NeRFs and 3D Gaussian Splatting are Reshaping SLAM: a Survey**, Tosi et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2402.13255)

- **3D Gaussian Splatting: Survey, Technologies, Challenges, and Opportunities**, Chen et al., TPAMI 2024 | [📄 Paper](https://arxiv.org/pdf/2407.17418.pdf)[🌐 Project Page](https://github.com/qqqqqqy0227/awesome-3DGS)

- **3D Gaussian as a New Vision Era: A Survey**, Fei et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2402.07181.pdf)

- **Recent Advances in 3D Gaussian Splatting**, Wu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.11134.pdf)

- **Gaussian Splatting: 3D Reconstruction and Novel View Synthesis, a Review**, Dalal et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2405.03417.pdf)

## Gaussian Theory:
- **[NeurIPS' 24]DiffGS: Functional Gaussian Splatting Diffusion**, Zhou et al., arXiv 2024 | [📄 Paper](https://arxiv.org/html/2410.19657v1) | [🌐 Project Page](https://junshengzhou.github.io/DiffGS/) | | [💻 Code](https://github.com/weiqi-zhang/DiffGS)

- **No Pose, No Problem: Surprisingly Simple 3D Gaussian Splats from Sparse Unposed Images**, Ye et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2410.24207) | [🌐 Project Page](https://noposplat.github.io/) | [💻 Code](https://github.com/cvg/NoPoSplat)

- **Octree-GS: Towards Consistent Real-time Rendering with LOD-Structured 3D Gaussians**, Ren et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2403.17898) | [🌐 Project Page](https://city-super.github.io/octree-gs/) | [💻 Code](https://github.com/city-super/Octree-GS)

- **3D Gaussian Ray Tracing: Fast Tracing of Particle Scenes**, Moenne-Loccoz et al., arXiv 2024 | [📄 Paper](https://www.arxiv.org/abs/2407.07090) | [🌐 Project Page](https://gaussiantracer.github.io/) | [🎥 Video](https://gaussiantracer.github.io/#supp_video)

- **3D Gaussian Splatting as Markov Chain Monte Carlo**, Ye et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2404.09591) | [🌐 Project Page](https://ubc-vision.github.io/3dgs-mcmc/) | [💻 Code](https://github.com/ubc-vision/3dgs-mcmc)

- **AbsGS: Recovering Fine Details for 3D Gaussian Splatting**, Ye et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2404.10484) | [🌐 Project Page](https://ty424.github.io/AbsGS.github.io/) | [💻 Code](https://github.com/TY424/AbsGS)

- **[CVPR '24 Highlight]Scaffold-GS: Structured 3D Gaussians for View-Adaptive Rendering**, Lu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2312.00109) | [🌐 Project Page](https://city-super.github.io/scaffold-gs/) | [💻 Code](https://github.com/city-super/Scaffold-GS)

- **Gaussian Splatting Lucas-Kanade**, Xie et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2407.11309v1)

- **InstantSplat: Sparse-view SfM-free Gaussian Splatting in Seconds**, Fan et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2403.20309) | [🌐 Project Page](https://instantsplat.github.io/) | [💻 Code](https://github.com/NVlabs/InstantSplat) | [🎥 Demo Video](https://www.youtube.com/watch?v=JdfrG89iPOA&t=347s) | [🎥 Demo](https://huggingface.co/spaces/kairunwen/InstantSplat)

- **Texture-GS: Disentangling the Geometry and Texture for 3D Gaussian Splatting Editing**, Xu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.10050) | [🌐 Project Page](https://slothfulxtx.github.io/TexGS/) | [💻 Code](https://github.com/slothfulxtx/Texture-GS)

- **Segment Any 4D Gaussians**, Ji et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2407.04504v2) | [🌐 Project Page](https://jsxzs.github.io/sa4d/) | [💻 Code](https://github.com/jsxzs/SA4D)

- **[CVPR '24]4D Gaussian Splatting for Real-Time Dynamic Scene Rendering**,
  Wu et al., CVPR 2024 | [📄 Paper](https://arxiv.org/abs/2310.08528.pdf) | [🌐 Project Page](https://guanjunwu.github.io/4dgs/) | [💻 Code](https://github.com/hustvl/4DGaussians)

- **Trim 3D Gaussian Splatting for Accurate Geometry Representation**, Fan et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2406.07499.pdf) | [🌐 Project Page](https://trimgs.github.io/) | [💻 Code](https://github.com/YuxueYang1204/TrimGS)

- **[CVPR '24 Best Student Paper]Mip-Splatting Alias-free 3D Gaussian Splatting**, Yu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2311.16493.pdf) | [🌐 Project Page](https://niujinshuchong.github.io/mip-splatting/) | [💻 Code](https://github.com/autonomousvision/mip-splatting)

- **[CVPR '24]COLMAP-Free 3D Gaussian Splatting**, Fu et al., arXiv 2023 | [📄 Paper](https://arxiv.org/abs/2312.07504) | [🌐 Project Page](https://oasisyang.github.io/colmap-free-3dgs/) | [💻 Code](https://github.com/NVlabs/CF-3DGS) | [🎥 Video](https://www.youtube.com/watch?v=mGeVQS4ExK4)

## Gaussian SLAM:
## 2024:
- **HI-SLAM2 Geometry-Aware Gaussian SLAM for Fast Monocular Scene Reconstruction**, Zhang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2411.17982) | [🌐 Project Page](https://hi-slam2.github.io/) | [💻 Code](https://github.com/Willyzw/HI-SLAM2)

- **DGS-SLAM: Gaussian Splatting SLAM in Dynamic Environment**, Kong et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2411.10722) | [🌐 Project Page](https://changjianjiang01.github.io/LI-GS/) | | [🎥 Video](https://www.youtube.com/watch?v=Mq3qZTTcN3E) | [💻 Code](https://github.com/kmk97/DGS-SLAM)

- **DG-SLAM: Robust Dynamic Gaussian Splatting SLAM with Hybrid Pose Optimization**, Xu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2411.08373) | [💻 Code](https://github.com/fudan-zvg/DG-SLAM)

- **LI-GS: Gaussian Splatting with LiDAR Incorporated for Accurate Large-Scale Reconstruction**, Jiang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2409.12899) | [🌐 Project Page](https://changjianjiang01.github.io/LI-GS/) | [🎥 Video](https://www.youtube.com/watch?v=DSsTCbD4mJQ)

- **MGSO: Monocular Real-time Photometric SLAM with Efficient 3D Gaussian Splatting**, Hu et al., arXiv 2024 | [📄 Paper](https://www.arxiv.org/abs/2409.13055)

- **GSFusion: Online RGB-D Mapping Where Gaussian Splatting Meets TSDF Fusion**, Wei and Leutenegger, arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2408.12677) | [🌐 Project Page](https://gs-fusion.github.io/) | [💻 Code](https://github.com/GS-Fusion/GSFusion) | | [🎥 Video](https://www.youtube.com/watch?v=rW8o_cRPZBg)

- **Visual SLAM with 3D Gaussian Primitives and Depth Priors Enabling Novel View Synthesis**, Qu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2408.05635)

- **IG-SLAM: Instant Gaussian SLAM**, Sarikamis and Alatan, arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2408.01126)

- **EndoGSLAM: Real-Time Dense Reconstruction and Tracking in Endoscopic Surgeries using Gaussian Splatting**, Wang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2403.15124)

- **SGS-SLAM: Semantic Gaussian Splatting For Neural Dense SLAM**, Li et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2402.03246.pdf) | [🎥 Demo Video](https://www.youtube.com/watch?v=y83yw1E-oUo)

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

## 2024:

- **GaussNav: Gaussian Splatting for Visual Navigation**, Lei et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.11625.pdf) | [🌐 Project Page](https://xiaohanlei.github.io/projects/GaussNav/) | [💻 Code](https://github.com/XiaohanLei/GaussNav)

- **3DGS-ReLoc: 3D Gaussian Splatting for Map Representation and Visual ReLocalization**, Jiang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.11367.pdf)

- **Beyond Uncertainty: Risk-Aware Active View Acquisition for Safe Robot Navigation and 3D Scene Understanding with FisherRF**, Liu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.11396.pdf)

- **3DGS-Calib: 3D Gaussian Splatting for Multimodal SpatioTemporal Calibration**, Herau et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.11577.pdf)

- **[CVPR '24] HUGS: Holistic Urban 3D Scene Understanding via Gaussian Splatting** Zhou et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.12722.pdf) | [🌐 Project Page](https://xdimlab.github.io/hugs_website/)| [💻 Code](https://github.com/hyzhou404/HUGS)

- **HO-Gaussian: Hybrid Optimization of 3D Gaussian Splatting for Urban Scenes**, Li et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.20032.pdf)

- **SGD: Street View Synthesis with Gaussian Splatting and Diffusion Prior**, Yu et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.20079.pdf)

## Poses:

## 2024:
- **[ECCV '24]GGRt: Towards Generalizable 3D Gaussians without Pose Priors in Real-Time**, Li et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.10147) | [🌐 Project Page](https://3d-aigc.github.io/GGRt/)

- **GS-Pose: Cascaded Framework for Generalizable Segmentation-based 6D Object Pose Estimation**, Cai et al., arXiv 2024 | [📄 Paper](https://arxiv.org/pdf/2403.10683) | [🌐 Project Page](https://dingdingcai.github.io/gs-pose/) | [💻 Code](https://github.com/dingdingcai/GS-pose) | [🎥 Short Presentation](https://youtu.be/SnJazusDLM8)

## Large-Scale:

## 2024:
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

## 2024:
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

- **Surfel-based RGB-D Reconstruction and
SLAM with Global and Local Consistency**, Yang, Msc thesis 2019 | [📄 Paper](https://www.cs.cmu.edu/~kaess/pub/Yang19thesis_ms.pdf)

## 3D Generations:

## 2024:
- **VistaDream Sampling multiview consistent images for single-view scene reconstruction**, Wang et al., arXiv 2024 | [📄 Paper](https://arxiv.org/abs/2410.16892) | [🌐 Project Page](https://vistadream-project-page.github.io/l) | [💻 Code](https://github.com/WHU-USI3DV/VistaDream)
## Data

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

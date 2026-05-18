# 3D Core Tasks

* [Classification](#Classification)
    * [Projection-based Methods](#projection-based-methods)
    * [Volumetric-based Methods](#volumetric-based-methods)
    * [Point-based Methods](#point-based-methods)
        * [MLP-based Methods](#mlp-based-methods)
        * [Convolution-based Methods](#convolution-based-methods)
        * [Graph-based Methods](#graph-based-methods)
        * [Transformer-based Methods](#transformer-based-methods)

* [Segmentation](#segmentation)
  * [Instance Segmentation](#instance-segmentation)
  * [Semantic Segmentation](#semantic-segmentation)
    * [Cross-Modality](#cross-modality)
  * [Other Types of Segmentation](#other-types-of-segmentation)
    * [Part Segmentation](#part-segmentation)
    * [Oversegmentation](#oversegmentation)
    * [3DGS-based Segmentation](#3dgs-based-segmentation)


* [Detection](#Detection)
    * [Data Representation](#Data-Representation)
       * [point-based](#point-based)
       * [voxel-based](#voxel-based)
       * [pillar-based](#pillar-based)
       * [projection-based](#projection-based)
       * [hybrid](#hybrid)
    * [Detection Stage](#Detection-Stage)
       * [One-Stage Detectors](#One-Stage-Detectors)
       * [Two-Stage Detectors](#Two-Stage-Detectors)
   * [Supervision](#Supervision)
       * [Weakly-supervised 3D Detection](#Weakly-supervised-3D-Detection)
       * [Semi-supervised 3D Detection](#Semi-supervised-3D-Detection)
       * [Self-/Unsupervised 3D Detection](#Self-/Unsupervised-3D-Detection)
 
     
* [Tracking](#Tracking)
   * [Single-Object Tracking](#Single-Object-Tracking)
      * [LiDAR Trackers](#LiDAR-Trackers)
      * [RGB-LiDAR Trackers](#RGB-LiDAR-Trackers)

* [Compression](#Compression)

* [6DoF Pose Estimation](#6DoF-Pose-Estimation)
   * [Object Pose Estimation](#Object-Pose-Estimation)
   * [Human Pose Estimation](#Human-Pose-Estimation) 

* [3D Point Cloud Registration](#3D-Point-Cloud-Registration)

 
  
---
## Classification

### Projection-based Methods

* **Multi-view convolutional neural networks for 3d shape recognition**, ICCV 2015, [ :link: ](https://openaccess.thecvf.com/content_iccv_2015/papers/Su_Multi-View_Convolutional_Neural_ICCV_2015_paper.pdf) [ :octocat: ](https://github.com/suhangpro/mvcnn)
* **Gift: A real-time and scalable 3d shape search engine**, CVPR 2016, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2016/papers/Bai_GIFT_A_Real-Time_CVPR_2016_paper.pdf)
* **Gvcnn: Group-view convolutional neural networks for 3d shape recognition**, CVPR 2018, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2018/papers/Feng_GVCNN_Group-View_Convolutional_CVPR_2018_paper.pdf) [ :octocat: ](https://github.com/waxnkw/gvcnn-pytorch)
* **Multi-view harmonized bilinear network for 3d object recognition**, CVPR 2018, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2018/CameraReady/0142.pdf) [ :octocat: ](https://github.com/liyuan24/MHBNN-PyTorch)
* **Mvtn: Multi-view transformation network for 3d shape recognition**, ICCV 2021, [ :link: ](https://openaccess.thecvf.com/content/ICCV2021/papers/Hamdi_MVTN_Multi-View_Transformation_Network_for_3D_Shape_Recognition_ICCV_2021_paper.pdf) [ :octocat: ](https://github.com/ajhamdi/MVTN)
* **Multi-view attention-convolution pooling network for 3D point cloud classification**, Springer 2022, [ :link: ](https://link.springer.com/article/10.1007/s10489-021-02840-2)
* **Clip2point: Transfer clip to point cloud classification with image-depth pre-training**, ICCV 2023, [ :link: ](https://openaccess.thecvf.com/content/ICCV2023/papers/Huang_CLIP2Point_Transfer_CLIP_to_Point_Cloud_Classification_with_Image-Depth_Pre-Training_ICCV_2023_paper.pdf) [ :octocat: ](https://github.com/tyhuang0428/CLIP2Point)
* **DTV-CNN: Neural network based on depth and thickness views for efficient 3D shape classification**, Elsevier 2023, [ :link: ](https://www.sciencedirect.com/science/article/pii/S2405844023087236)
* **Multi-view representation is what you need for point-cloud pre-training**, ICLR 2024, [ :link: ](https://openreview.net/forum?id=imZcqOrbig)
* **Pointofview: A multi-modal network for few-shot 3d point cloud classification fusing point and multi-view image features**, CVPR Workshop 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024W/3DMV/papers/Ren_PointOfView_A_Multi-modal_Network_for_Few-shot_3D_Point_Cloud_Classification_CVPRW_2024_paper.pdf)
* **3D model classification based on DRSN and multi-view feature fusion**, Elsevier 2025, [ :link: ](https://www.sciencedirect.com/science/article/abs/pii/S0957417425004944)


### Volumetric-based Methods

* **Voxnet: A 3d convolutional neural network for real-time object recognition**, IEEE/RSJ (IROS) 2015, [ :link: ](https://ieeexplore.ieee.org/document/7353481) [ :octocat: ](https://github.com/AutoDeep/VoxNet)
* **Fpnn: Field probing neural networks for 3d data**, NIPS 2016, [ :link: ](https://proceedings.neurips.cc/paper_files/paper/2016/file/854d6fae5ee42911677c739ee1734486-Paper.pdf) [ :octocat: ](https://github.com/yangyanli/FPNN)
* **Octnet: Learning deep 3d representations at high resolutions**, CVPR 2017, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2017/papers/Riegler_OctNet_Learning_Deep_CVPR_2017_paper.pdf) [ :octocat: ](https://github.com/griegler/octnet)
* **O-cnn: Octree-based convolutional neural networks for 3d shape analysis**, ACM 2017, [ :link: ](https://dl.acm.org/doi/10.1145/3072959.3073608) [ :octocat: ](https://github.com/microsoft/o-cnn)
* **Escape from cells: Deep kd-networks for the recognition of 3d point cloud models**, ICCV 2017, [ :link: ](https://openaccess.thecvf.com/content_ICCV_2017/papers/Klokov_Escape_From_Cells_ICCV_2017_paper.pdf) [ :octocat: ](https://github.com/fxia22/kdnet.pytorch)
* **MSNet: Multi-scale convolutional network for point cloud classification**, Remote Sense 2018, [ :link: ](https://www.mdpi.com/2072-4292/10/4/612)
* **Vv-net: Voxel vae net with group convolutions for point cloud segmentation**, ICCV 2019, [ :link: ](https://openaccess.thecvf.com/content_ICCV_2019/papers/Meng_VV-Net_Voxel_VAE_Net_With_Group_Convolutions_for_Point_Cloud_ICCV_2019_paper.pdf) [ :octocat: ](https://github.com/xianyuMeng/VV-Net-Voxel-VAE-Net-with-Group-Convolutions-for-Point-Cloud-Segmentation)
* **Multi-level 3D CNN for learning multi-scale spatial features**, CVPR Workshop 2019, [ :link: ](https://ieeexplore.ieee.org/document/9025500)
* **2-s3net: Attentive feature fusion with adaptive feature selection for sparse semantic segmentation network**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content/CVPR2021/papers/Cheng_AF2-S3Net_Attentive_Feature_Fusion_With_Adaptive_Feature_Selection_for_Sparse_CVPR_2021_paper.pdf)
* **Point-voxel adaptive feature abstraction for robust point cloud classification**, ArXiv 2022, [ :link: ](https://arxiv.org/abs/2210.15514) [ :octocat: ](https://github.com/zhulf0804/PV-Ada)


### Point-based Methods

#### MLP-based Methods

* **Pointnet: Deep learning on point sets for 3d classification and segmentation**, CVPR 2017, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2017/papers/Qi_PointNet_Deep_Learning_CVPR_2017_paper.pdf) [ :octocat: ](https://github.com/charlesq34/pointnet)
* **PointNet++: Deep Hierarchical Feature Learning on Point Sets in a Metric Space**, NIPS 2017, [ :octocat: ](https://github.com/charlesq34/pointnet2)
* **Momen (e) t: Flavor the moments in learning to classify shapes**, ICCVW 2019, [ :link: ](https://openaccess.thecvf.com/content_ICCVW_2019/papers/GMDL/Joseph-Rivlin_Momenet_Flavor_the_Moments_in_Learning_to_Classify_Shapes_ICCVW_2019_paper.pdf)
* **Pointweb: Enhancing local neighborhood features for point cloud processing**, IEEE/CVPR 2019, [ :link: ](https://ieeexplore.ieee.org/document/8954075) [ :octocat: ](https://github.com/hszhao/PointWeb)
* **Structural relational reasoning of point clouds**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2019/papers/Duan_Structural_Relational_Reasoning_of_Point_Clouds_CVPR_2019_paper.pdf) [ :octocat: ](https://github.com/duanyueqi/SRN)
* **Pointnext: Revisiting pointnet++ with improved training and scaling strategies**, NeurIPS 2022, [ :link: ](https://openreview.net/pdf?id=EAcWgk7JM58) [ :octocat: ](https://github.com/guochengqian/pointnext)
* **Rethinking Network Design and Local Geometry in Point Cloud: A Simple Residual MLP Framework**, ICLR 2022, [ :link: ](https://openreview.net/forum?id=3Pbra-_u76D) [ :octocat: ](https://github.com/ma-xu/pointMLP-pytorch)
* **DualMLP: a two-stream fusion model for 3D point cloud classification**, Springer 2024, [ :link: ](https://link.springer.com/article/10.1007/s00371-023-03114-3) [ :octocat: ](https://github.com/snehaputul/DualMLP)
* **Pointgl: A simple global-local framework for efficient point cloud analysis**, IEEE 2024, [ :link: ](https://ieeexplore.ieee.org/document/10414214) [ :octocat: ](https://github.com/roywangj/pointgl)
* **Improved mlp point cloud processing with high-dimensional positional encoding**, AAAI 2024, [ :link: ](https://ojs.aaai.org/index.php/AAAI/article/view/28625)
* **Interpretable point cloud classification using multiple instance learning**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/papers/De_Vries_Interpretable_point_cloud_classification_using_multiple_instance_learning_ICCV_2025_paper.pdf)
* **KAN or MLP? Point Cloud Shows the Way Forward**, ICLR 2026, [ :link: ](https://openreview.net/forum?id=1x0eJ8uUx6)


#### Convolution-based Methods

* **Point convolutional neural networks by extension operators**, Arxiv 2018, [ :link: ](https://arxiv.org/abs/1803.10091) [ :octocat: ](https://github.com/matanatz/pcnn)
* **Pointcnn: Convolution on x-transformed points**, NIPS 2018, [ :link: ](https://papers.nips.cc/paper/2018/file/f5f8590cd58a54e94377e6ae2eded4d9-Paper.pdf) [ :octocat: ](https://github.com/yangyanli/PointCNN)
* **Pointwise convolutional neural networks**, CVPR 2018, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2018/papers/Hua_Pointwise_Convolutional_Neural_CVPR_2018_paper.pdf) [ :octocat: ](https://github.com/hkust-vgd/pointwise)
* **Effective rotation-invariant point cnn with spherical harmonics kernels**, IEEE 3DV 2019, [ :link: ](https://ieeexplore.ieee.org/document/8886010) [ :octocat: ](https://github.com/adrienPoulenard/SPHnet)
* **Relation-shape convolutional neural network for point cloud analysis**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2019/papers/Liu_Relation-Shape_Convolutional_Neural_Network_for_Point_Cloud_Analysis_CVPR_2019_paper.pdf) [ :octocat: ](https://github.com/Yochengliu/Relation-Shape-CNN)
* **Kpconv: Flexible and deformable convolution for point clouds**, IEEE/ICCV 2019, [ :link: ](https://ieeexplore.ieee.org/document/9010002) [ :octocat: ](https://github.com/HuguesTHOMAS/KPConv)
* **Densepoint: Learning densely contextual representation for efficient point cloud processing**, ICCV 2019, [ :link: ](https://openaccess.thecvf.com/content_ICCV_2019/papers/Liu_DensePoint_Learning_Densely_Contextual_Representation_for_Efficient_Point_Cloud_Processing_ICCV_2019_paper.pdf) [ :octocat: ](https://github.com/Yochengliu/DensePoint)
* **ConvPoint: Continuous convolutions for point cloud processing**, Elsevier 2020, [ :link: ](https://www.sciencedirect.com/science/article/abs/pii/S0097849320300224) [ :octocat: ](https://github.com/aboulch/ConvPoint)
* **A-cnn: Annularly convolutional neural networks on point clouds**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2019/papers/Komarichev_A-CNN_Annularly_Convolutional_Neural_Networks_on_Point_Clouds_CVPR_2019_paper.pdf) [ :octocat: ](https://github.com/akomarichev/a-cnn)
* **Rotation invariant convolutions for 3d point clouds deep learning**, IEEE 3DV 2019, [ :link: ](https://ieeexplore.ieee.org/document/8886052) [ :octocat: ](https://github.com/hkust-vgd/riconv)
* **Shellnet: Efficient point cloud convolutional neural networks using concentric shells statistics**, ICCV 2019, [ :link: ](https://openaccess.thecvf.com/content_ICCV_2019/supplemental/Zhang_ShellNet_Efficient_Point_ICCV_2019_supplemental.pdf) [ :octocat: ](https://github.com/hkust-vgd/shellnet)
* **Deltaconv: anisotropic operators for geometric deep learning on point clouds**, ACM 2022, [ :link: ](https://dl.acm.org/doi/abs/10.1145/3528223.3530166) [ :octocat: ](https://github.com/rubenwiersma/deltaconv)
* **Surface representation for point clouds**, CVPR 2022, [ :link: ](https://openaccess.thecvf.com/content/CVPR2022/papers/Ran_Surface_Representation_for_Point_Clouds_CVPR_2022_paper.pdf) [ :octocat: ](https://github.com/hancyran/RepSurf)
* **Composite convolution: A flexible operator for deep learning on 3D point clouds**, Elsevier 2024, [ :link: ](https://www.sciencedirect.com/science/article/pii/S003132032400308X) [ :octocat: ](https://github.com/sirolf-otrebla/CompositeNet)
* **PointCNN++: Performant Convolution on Native Points**, Arxiv 2025, [ :link: ](https://arxiv.org/abs/2511.23227) [ :octocat: ](https://github.com/ant-research/pointelligence)

* **Primary Visual Cortex Inspired Point Cloud Analysis Framework**, AAAI 2026, [ :link: ](https://ojs.aaai.org/index.php/AAAI/article/view/37348) 


#### Graph-based Methods

* **Dynamic edge-conditioned filters in convolutional neural networks on graphs**, CVPR 2017, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2017/papers/Simonovsky_Dynamic_Edge-Conditioned_Filters_CVPR_2017_paper.pdf) [ :octocat: ](https://github.com/mys007/ecc)
* **Local spectral graph convolution for point set feature learning**, ECCV 2018, [ :link: ](https://dl.acm.org/doi/abs/10.1007/978-3-030-01225-0_4) [ :octocat: ](https://github.com/utayao/LocalSpecGCN)
* **Rgcnn: Regularized graph cnn for point cloud segmentation**, ACM 2018, [ :link: ](https://dl.acm.org/doi/10.1145/3240508.3240621) [ :octocat: ](https://github.com/tegusi/RGCNN)
* **A graph-cnn for 3d point cloud classification**, IEEE ICASSP 2018, [ :link: ](https://dl.acm.org/doi/10.1109/ICASSP.2018.8462291) [ :octocat: ](https://github.com/maggie0106/Graph-CNN-in-3D-Point-Cloud-Classification)
* **Mining point cloud local structures by kernel correlation and graph pooling**, CVPR 2018, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2018/papers/Shen_Mining_Point_Cloud_CVPR_2018_paper.pdf) [ :octocat: ](http://www.merl.com/research/license#KCNet)
* **Dynamic graph cnn for learning on point clouds**, ACM 2019, [ :link: ](https://dl.acm.org/doi/10.1145/3326362) [ :octocat: ](https://github.com/WangYueFt/dgcnn)
* **PointNGCNN: Deep convolutional networks on 3D point clouds with neighborhood graph filters**, Elsevier 2020, [ :link: ](https://www.sciencedirect.com/science/article/abs/pii/S0097849319301748)
* **Convolution in the cloud: Learning deformable kernels in 3d graph convolution networks for point cloud analysis**, CVPR 2020, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2020/papers/Lin_Convolution_in_the_Cloud_Learning_Deformable_Kernels_in_3D_Graph_CVPR_2020_paper.pdf) [ :octocat: ](https://github.com/j1a0m0e4sNTU/3dgcn)
* **Pointmanifold: Using manifold learning for point cloud classification**, Arxiv 2020, [ :link: ](https://arxiv.org/abs/2010.07215)
* **Linked dynamic graph cnn: Learning through point cloud by linking hierarchical features**, IEEE 2021, [ :link: ](https://ieeexplore.ieee.org/document/9665104/) [ :octocat: ](https://github.com/KuangenZhang/ldgcnn)
* **Pointview-gcn: 3d shape classification with multi-view point clouds**, IEEE ICIP 2021, [ :link: ](https://ieeexplore.ieee.org/document/9506426/) [ :octocat: ](https://github.com/SMohammadi89/PointView-GCN)
* **Paconv: Position adaptive convolution with dynamic kernel assembling on point clouds**, CVPR 2021, [ :link: ](https://openaccess.thecvf.com/content/CVPR2021/papers/Xu_PAConv_Position_Adaptive_Convolution_With_Dynamic_Kernel_Assembling_on_Point_CVPR_2021_paper.pdf) [ :octocat: ](https://github.com/CVMI-Lab/PAConv)
* **Walk in the cloud: Learning curves for point clouds shape analysis**, ICCV 2021, [ :link: ](https://openaccess.thecvf.com/content/ICCV2021/papers/Xiang_Walk_in_the_Cloud_Learning_Curves_for_Point_Clouds_Shape_ICCV_2021_paper.pdf) [ :octocat: ](https://github.com/tiangexiang/CurveNet)
* **PointViG: A Lightweight GNN-based Model for Efficient Point Cloud Analysis**, Arxiv 2024, [ :link: ](https://arxiv.org/abs/2407.00921)
* **Enhancing 3D Point Cloud Classification with ModelNet-R and Point-SkipNet**, Arxiv 2025, [ :link: ](https://arxiv.org/abs/2509.05198) [ :octocat: ](https://github.com/m-saeid/ModeNetR_PointSkipNet)


#### Transformer-based Methods

* **Modeling point clouds with self-attention and gumbel subset sampling**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2019/papers/Yang_Modeling_Point_Clouds_With_Self-Attention_and_Gumbel_Subset_Sampling_CVPR_2019_paper.pdf)
* **Point transformer**, ICCV 2021, [ :link: ](https://openaccess.thecvf.com/content/ICCV2021/papers/Zhao_Point_Transformer_ICCV_2021_paper.pdf)
* **Pct: Point cloud transformer**, Springer 2021, [ :link: ](https://link.springer.com/article/10.1007/s41095-021-0229-5) [ :octocat: ](https://github.com/Strawberry-Eat-Mango/PCT_Pytorch)
* **Point transformer v2: Grouped vector attention and partition-based pooling**, NeurIPS 2022, [ :link: ](https://proceedings.neurips.cc/paper_files/paper/2022/file/d78ece6613953f46501b958b7bb4582f-Paper-Conference.pdf) [ :octocat: ](https://github.com/Pointcept/PointTransformerV2)
* **Lcpformer: Towards effective 3d point cloud analysis via local context propagation in transformers**, IEEE 2023, [ :link: ](https://ieeexplore.ieee.org/document/10049597) [ :octocat: ](https://github.com/zhh6425/LocalContextPropagation)
* **Self-positioning point-based transformer for point cloud understanding**, CVPR 2023, [ :link: ](https://openaccess.thecvf.com/content/CVPR2023/papers/Park_Self-Positioning_Point-Based_Transformer_for_Point_Cloud_Understanding_CVPR_2023_paper.pdf) [ :octocat: ](https://github.com/mlvlab/spotr)
* **Point transformer v3: Simpler faster stronger**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Wu_Point_Transformer_V3_Simpler_Faster_Stronger_CVPR_2024_paper.pdf) [ :octocat: ](https://github.com/pointcept/pointtransformerv3)
* **PPT: A Point Patch Transformer for Point Cloud Classification**, Optica Open 2025, [ :link: ](https://preprints.opticaopen.org/articles/preprint/PPT_A_Point_Patch_Transformer_for_Point_Cloud_Classification/28504493/3/files/52676381.pdf)
* **Spiking point transformer for point cloud classification**, AAAI 2025, [ :link: ](https://ojs.aaai.org/index.php/AAAI/article/view/35459/37614) [ :octocat: ](https://github.com/PeppaWu/SPT)
* **An aerial point cloud classification using point transformer via multi-feature fusion**, Scientific Reports 2025, [ :link: ](https://www.nature.com/articles/s41598-025-02719-z)




## Segmentation

### Instance Segmentation

* **Any3DIS: Class-Agnostic 3D Instance Segmentation by 2D Mask Tracking**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/html/Nguyen_Any3DIS_Class-Agnostic_3D_Instance_Segmentation_by_2D_Mask_Tracking_CVPR_2025_paper.html)
* **Insightful Instance Features for 3D Instance Segmentation**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/html/Roh_Insightful_Instance_Features_for_3D_Instance_Segmentation_CVPR_2025_paper.html) [ :octocat: ](https://github.com/kuai-lab/cvpr25_IKNE)
* **Relation3D: Enhancing Relation Modeling for Point Cloud Instance Segmentation**, CVPR 2025, [ :link: ](https://ieeexplore.ieee.org/abstract/document/11092675) [ :octocat: ](https://github.com/Howard-coder191/Relation3D)
* **Sketchy Bounding-box Supervision for 3D Instance Segmentation**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/html/Deng_Sketchy_Bounding-box_Supervision_for_3D_Instance_Segmentation_CVPR_2025_paper.html) [ :octocat: ](https://github.com/dengq7/Sketchy-3DIS)


### Semantic Segmentation

#### Cross-Modality

* **All in One: Visual-Description-Guided Unified Point Cloud Segmentation**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/html/Han_All_in_One_Visual-Description-Guided_Unified_Point_Cloud_Segmentation_ICCV_2025_paper.html) [ :octocat: ](https://github.com/Hanzy1996/VDG-Uni3DSeg)
* **AiDe: Improving 3D Open-Vocabulary Semantic Segmentation by Aligned Vision-Language Learning**, WACV 2025, [ :link: ](https://ieeexplore.ieee.org/abstract/document/10943459)
* **Generalized Few-Shot Point Cloud Segmentation via LLM-Assisted Hyper-Relation Matching**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/html/Li_Generalized_Few-Shot_Point_Cloud_Segmentation_via_LLM-Assisted_Hyper-Relation_Matching_ICCV_2025_paper.html)
* **Generalized Few-shot 3D Point Cloud Segmentation with Vision-Language Model**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/html/An_Generalized_Few-shot_3D_Point_Cloud_Segmentation_with_Vision-Language_Model_CVPR_2025_paper.html) [ :octocat: ](https://github.com/ZhaochongAn/GFS-VL)
* **Functionality Understanding and Segmentation in 3D Scenes**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/html/Corsetti_Functionality_Understanding_and_Segmentation_in_3D_Scenes_CVPR_2025_paper.html) [ :octocat: ](https://github.com/tev-fbk/fun3du)
* **SAM2Object: Consolidating View Consistency via SAM2 for Zero-Shot 3D Instance Segmentation**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/html/Zhao_SAM2Object_Consolidating_View_Consistency_via_SAM2_for_Zero-Shot_3D_Instance_CVPR_2025_paper.html) [ :octocat: ](https://github.com/jihuaizhaohd/SAM2Object)
* **UniDxMD: Towards Unified Representation for Cross-Modal Unsupervised Domain Adaptation in 3D Semantic Segmentation**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/html/Liang_UniDxMD_Towards_Unified_Representation_for_Cross-Modal_Unsupervised_Domain_Adaptation_in_ICCV_2025_paper.html)
* **CACE: Sim-to-Real Indoor 3D Semantic Segmentation via Context-Aware Augmentation and Consistency Enforcement**, WACV 2025, [ :link: ](https://ieeexplore.ieee.org/abstract/document/10943913)


### Other Types of Segmentation
#### Part Segmentation
* **PartField: Learning 3D Feature Fields for Part Segmentation and Beyond**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/html/Liu_PartField_Learning_3D_Feature_Fields_for_Part_Segmentation_and_Beyond_ICCV_2025_paper.html) [ :octocat: ](https://github.com/nv-tlabs/PartField)
* **3D Part Segmentation via Geometric Aggregation of 2D Visual Features**, WACV 2025, [ :link: ](https://ieeexplore.ieee.org/abstract/document/10943567) [ :octocat: ](https://github.com/marco-garosi/COPS)

#### Oversegmentation
* **Serialization based Point Cloud Oversegmentation**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/html/Lu_Serialization_based_Point_Cloud_Oversegmentation_ICCV_2025_paper.html) [ :octocat: ](https://github.com/CHL-glitch/SPCNet)

#### 3DGS-based Segmentation
* **COB-GS: Clear Object Boundaries in 3DGS Segmentation Based on Boundary-Adaptive Gaussian Splitting**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/html/Zhang_COB-GS_Clear_Object_Boundaries_in_3DGS_Segmentation_Based_on_Boundary-Adaptive_CVPR_2025_paper.html) [ :octocat: ](https://github.com/ZestfulJX/COB-GS)


## Detection

### Data Representation
#### point-based
* **PointRCNN: 3D Object Proposal Generation and Detection from Point Cloud**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2019/papers/Shi_PointRCNN_3D_Object_Proposal_Generation_and_Detection_From_Point_Cloud_CVPR_2019_paper.pdf)  [ :octocat: ](https://github.com/sshaoshuai/PointRCNN)
* **Deep Hough Voting for 3D Object Detection in Point Clouds**, ICCV 2019, [ :link: ](https://openaccess.thecvf.com/content_ICCV_2019/papers/Qi_Deep_Hough_Voting_for_3D_Object_Detection_in_Point_Clouds_ICCV_2019_paper.pdf) [ :octocat: ](https://github.com/facebookresearch/votenet)
* **3DSSD: Point-based 3D Single Stage Object Detector**, CVPR 2020, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2020/papers/Yang_3DSSD_Point-Based_3D_Single_Stage_Object_Detector_CVPR_2020_paper.pdf) [ :octocat: ](https://github.com/JIA-Lab-research/3DSSD)
* **3Point-GNN: Graph Neural Network for 3D Object Detection in a Point Cloud**, CVPR 2020, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2020/papers/Shi_Point-GNN_Graph_Neural_Network_for_3D_Object_Detection_in_a_CVPR_2020_paper.pdf) [ :octocat: ](https://github.com/WeijingShi/Point-GNN)
* **From Points to Parts: 3D Object Detection from Point Cloud with Part-aware and Part-aggregation Network**, TPAMI 2020,[ :link: ](https://arxiv.org/abs/1907.03670), [ :octocat: ](https://github.com/sshaoshuai/PartA2-Net/blob/master/README.md)
* **An End-to-End Transformer Model for 3D Object Detection**, ICCV 2021, [ :link: ](https://openaccess.thecvf.com/content/ICCV2021/papers/Misra_An_End-to-End_Transformer_Model_for_3D_Object_Detection_ICCV_2021_paper.pdf) [ :octocat: ](https://facebookresearch.github.io/3detr/)
* **Group-Free 3D Object Detection via Transformers**, ICCV 2021, [ :link: ](https://openaccess.thecvf.com/content/ICCV2021/papers/Liu_Group-Free_3D_Object_Detection_via_Transformers_ICCV_2021_paper.pdf) [ :octocat: ](https://github.com/zeliu98/Group-Free-3D)
* **Not All Points Are Equal: Learning Highly Efficient Point-based Detectors for 3D LiDAR Point Clouds**, CVPR 2022,  [ :link: ](https://openaccess.thecvf.com/content/CVPR2022/papers/Zhang_Not_All_Points_Are_Equal_Learning_Highly_Efficient_Point-Based_Detectors_CVPR_2022_paper.pdf) [ :octocat: ](https://github.com/yifanzhang713/IA-SSD)
* **Clusterformer: Cluster-based Transformer for 3D Object Detection in Point Clouds**, ICCV 2023, [ :link: ](https://openaccess.thecvf.com/content/ICCV2023/papers/Pei_Clusterformer_Cluster-based_Transformer_for_3D_Object_Detection_in_Point_Clouds_ICCV_2023_paper.pdf)
* **DetZero: Rethinking Offboard 3D Object Detection with Long-term Sequential Point Clouds**, ICCV 2023, [ :link: ](https://openaccess.thecvf.com/content/ICCV2023/papers/Ma_DetZero_Rethinking_Offboard_3D_Object_Detection_with_Long-term_Sequential_Point_ICCV_2023_paper.pdf) [ :octocat: ](https://github.com/PJLab-ADG/DetZero)
* **Open-Vocabulary Point-Cloud Object Detection Without 3D Annotation**, , [ :link: ](https://openaccess.thecvf.com/content/CVPR2023/papers/Lu_Open-Vocabulary_Point-Cloud_Object_Detection_Without_3D_Annotation_CVPR_2023_paper.pdf) [ :octocat: ](https://github.com/lyhdet/OV-3DET)
* **PTT: Point-Trajectory Transformer for Efficient Temporal 3D Object Detection**, , [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Huang_PTT_Point-Trajectory_Transformer_for_Efficient_Temporal_3D_Object_Detection_CVPR_2024_paper.pdf) [ :octocat: ](https://github.com/kuanchihhuang/PTT)
* **FASTer: Focal Token Acquiring-and-Scaling Transformer for Long-term 3D Object Detection**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/papers/Dang_FASTer_Focal_token_Acquiring-and-Scaling_Transformer_for_Long-term_3D_Objection_Detection_CVPR_2025_paper.pdf) [ :octocat: ](https://github.com/MSunDYY/FASTer)
* **GeoFormer: Geometry Point Encoder for 3D Object Detection with Graph-based Transformer**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/papers/Jin_GeoFormer_Geometry_Point_Encoder_for_3D_Object_Detection_with_Graph-based_ICCV_2025_paper.pdf)
* **Robust 3D Object Detection using Probabilistic Point Clouds from Single-Photon LiDARs**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/papers/Goyal_Robust_3D_Object_Detection_using_Probabilistic_Point_Clouds_from_Single-Photon_ICCV_2025_paper.pdf) [ :octocat: ](https://bhavyagoyal.github.io/ppc/)

#### voxel-based

* **VoxelNet: End-to-End Learning for Point Cloud Based 3D Object Detection**, CVPR 2018, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2018/papers/Zhou_VoxelNet_End-to-End_Learning_CVPR_2018_paper.pdf) [ :octocat: ](https://github.com/ModelBunker/VoxelNet-PyTorch)
* **SECOND: Sparsely Embedded Convolutional Detection**, Sensors 2018, [ :link: ](https://www.mdpi.com/1424-8220/18/10/3337) [ :octocat: ](https://github.com/traveller59/second.pytorch)
* **Voxel R-CNN: Towards High Performance Voxel-based 3D Object Detection**, AAAI 2021, [ :link: ](https://arxiv.org/abs/2012.15712) [ :octocat: ](https://github.com/djiajunustc/Voxel-R-CNN)
* **Voxel Transformer (VoTr) for 3D Object Detection**, ICCV 2021, [ :link: ](https://arxiv.org/abs/2109.02497) [ :octocat: ](https://github.com/PointsCoder/VOTR)
* **Focal Sparse Convolutional Networks for 3D Object Detection**, CVPR 2022, [ :link: ](https://openaccess.thecvf.com/content/CVPR2022/papers/Chen_Focal_Sparse_Convolutional_Networks_for_3D_Object_Detection_CVPR_2022_paper.pdf) [ :octocat: ](https://github.com/JIA-Lab-research/FocalsConv)
* **Embracing Single Stride 3D Object Detector with Sparse Transformer (SST)**, CVPR 2022, [ :link: ](https://openaccess.thecvf.com/content/CVPR2022/papers/Fan_Embracing_Single_Stride_3D_Object_Detector_With_Sparse_Transformer_CVPR_2022_paper.pdf) [ :octocat: ](https://github.com/tusen-ai/SST)
* **DSVT: Dynamic Sparse Voxel Transformer with Rotated Sets**, CVPR 2023, [ :link: ](https://openaccess.thecvf.com/content/CVPR2023/papers/Wang_DSVT_Dynamic_Sparse_Voxel_Transformer_With_Rotated_Sets_CVPR_2023_paper.pdf) [ :octocat: ](https://github.com/Haiyang-W/DSVT)
* **VoxelNeXt: Fully Sparse VoxelNet for 3D Object Detection and Tracking**, CVPR 2023, [ :link: ](https://openaccess.thecvf.com/content/CVPR2023/html/Chen_VoxelNeXt_Fully_Sparse_VoxelNet_for_3D_Object_Detection_and_Tracking_CVPR_2023_paper.html) [ :octocat: ](https://github.com/dvlab-research/VoxelNeXt)
* **SAFDNet: A Simple and Effective Network for Fully Sparse 3D Object Detection**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Zhang_SAFDNet_A_Simple_and_Effective_Network_for_Fully_Sparse_3D_CVPR_2024_paper.pdf) [ :octocat: ](https://github.com/zhanggang001/HEDNet)
* **UniMamba: Unified Spatial-Channel Representation Learning with Group-Efficient Mamba for LiDAR-based 3D Object Detection**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/html/Jin_UniMamba_Unified_Spatial-Channel_Representation_Learning_with_Group-Efficient_Mamba_for_LiDAR-based_CVPR_2025_paper.html) [ :octocat: ](https://github.com/suhaisheng/UniMamba)
* **ViKIENet: Towards Efficient 3D Object Detection with Virtual Key Instance Enhanced Network**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/papers/Yu_ViKIENet_Towards_Efficient_3D_Object_Detection_with_Virtual_Key_Instance_CVPR_2025_paper.pdf) [ :octocat: ](https://github.com/jessieqiu/ViKIENet)
* **FSHNet: Fully Sparse Hybrid Network for 3D Object Detection**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/papers/Liu_FSHNet_Fully_Sparse_Hybrid_Network_for_3D_Object_Detection_CVPR_2025_paper.pdf) [ :octocat: ](https://github.com/Say2L/FSHNet)

#### pillar-based
* **PointPillars: Fast Encoders for Object Detection from Point Clouds**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2019/papers/Lang_PointPillars_Fast_Encoders_for_Object_Detection_From_Point_Clouds_CVPR_2019_paper.pdf) [ :octocat: ](https://github.com/nutonomy/second.pytorch)
* **PillarNet: Real-Time and High-Performance Pillar-based 3D Object Detection**, ECCV 2022, [ :link: ](https://arxiv.org/abs/2205.07403) [ :octocat: ](https://github.com/VISION-SJTU/PillarNet)
* **PillarNeXt: Rethinking Network Designs for 3D Object Detection in LiDAR Point Clouds**, CVPR 2023, [ :link: ](https://openaccess.thecvf.com/content/CVPR2023/html/Li_PillarNeXt_Rethinking_Network_Designs_for_3D_Object_Detection_in_LiDAR_Point_Clouds_CVPR_2023_paper.html) [ :octocat: ](https://github.com/qcraftai/pillarnext)
* **PillarHist: A Quantization-aware Pillar Feature Encoder based on Height-aware Histogram**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/html/Zhou_PillarHist_A_Quantization-aware_Pillar_Feature_Encoder_based_on_Height-aware_Histogram_CVPR_2025_paper.html) [ :octocat: ](https://github.com/open-mmlab/mmdetection3d) 
* **3DPillars: Pillar-based Two-stage 3D Object Detection**, ESWA 2025, [ :link: ](https://arxiv.org/abs/2509.05780) [ :octocat: ](https://github.com/open-mmlab/mmdetection3d) 

#### projection-based (BEV / range-view)
* **MV3D: Multi-View 3D Object Detection Network for Autonomous Driving**, CVPR 2017, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2017/papers/Chen_Multi-View_3D_Object_CVPR_2017_paper.pdf) [ :octocat: ](https://github.com/bostondiditeam/MV3D)
* **PIXOR: Real-time 3D Object Detection from Point Clouds**, CVPR 2018, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2018/papers/Yang_PIXOR_Real-Time_3D_CVPR_2018_paper.pdf) [ :octocat: ](https://github.com/philip-huang/PIXOR) 
* **AVOD: Joint 3D Proposal Generation and Object Detection from View Aggregation**, IROS 2018, [ :link: ](https://arxiv.org/abs/1712.02294) [ :octocat: ](https://github.com/kujason/avod)
* **LaserNet: An Efficient Probabilistic 3D Object Detector for Autonomous Driving**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2019/papers/Meyer_LaserNet_An_Efficient_Probabilistic_3D_Object_Detector_for_Autonomous_Driving_CVPR_2019_paper.pdf) [ :octocat: ](https://github.com/atyshka/Lasernet) 
* **RangeDet: In Defense of Range View for LiDAR-based 3D Object Detection**, ICCV 2021, [ :link: ](https://openaccess.thecvf.com/content/ICCV2021/papers/Fan_RangeDet_In_Defense_of_Range_View_for_LiDAR-Based_3D_Object_ICCV_2021_paper.pdf) [ :octocat: ](https://github.com/tusen-ai/RangeDet)
* **BEVFormer: Learning Bird’s-Eye-View Representation from Multi-Camera Videos**, ECCV 2022, [ :link: ](https://arxiv.org/abs/2203.17270) [ :octocat: ](https://github.com/fundamentalvision/BEVFormer)
* **BEVDepth: Acquisition of Reliable Depth for Multi-view 3D Object Detection**, AAAI 2023, [ :link: ](https://arxiv.org/abs/2206.10092) [ :octocat: ](https://github.com/Megvii-BaseDetection/BEVDepth)
* **SparseBEV: High-Performance Sparse 3D Object Detection from Multi-Camera Videos**, ICCV 2023, [ :link: ](https://openaccess.thecvf.com/content/ICCV2023/papers/Liu_SparseBEV_High-Performance_Sparse_3D_Object_Detection_from_Multi-Camera_Videos_ICCV_2023_paper.pdf) [ :octocat: ](https://github.com/MCG-NJU/SparseBEV)
* **BEVNeXt: Reviving Dense BEV Frameworks for 3D Object Detection**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Li_BEVNeXt_Reviving_Dense_BEV_Frameworks_for_3D_Object_Detection_CVPR_2024_paper.pdf) [ :octocat: ](https://github.com/woxihuanjiangguo/BEVNeXt)
* **CorrBEV: Multi-View 3D Object Detection by Correlation Learning with Multi-modal Prototypes**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/papers/Xue_CorrBEV_Multi-View_3D_Object_Detection_by_Correlation_Learning_with_Multi-modal_CVPR_2025_paper.pdf) [ :octocat: ](https://github.com/LLaVi-Lab) 
* **EVT: Efficient View Transformation for Multi-Modal 3D Object Detection**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/papers/Lee_EVT_Efficient_View_Transformation_for_Multi-Modal_3D_Object_Detection_ICCV_2025_paper.pdf) [ :octocat: ](https://github.com/open-mmlab/mmdetection3d) 
* **OpenM3D: Open-Vocabulary Multi-view Indoor 3D Object Detection without Human Annotations**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/papers/Hsu_OpenM3D_Open_Vocabulary_Multi-view_Indoor_3D_Object_Detection_without_Human_ICCV_2025_paper.pdf) [ :octocat: ](https://github.com/OpenM3D) 
* **What Matters in Range View 3D Object Detection**, CoRL 2024, [ :link: ](https://openreview.net/forum?id=EifoVoIyd5) [ :octocat: ](https://github.com/whatever50/range-view-3d-detection) 

#### hybrid (explicitly combine multiple representations and/or modalities)
* **PV-RCNN: Point-Voxel Feature Set Abstraction for 3D Object Detection**, CVPR 2020, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2020/papers/Shi_PV-RCNN_Point-Voxel_Feature_Set_Abstraction_for_3D_Object_Detection_CVPR_2020_paper.pdf) [ :octocat: ](https://github.com/sshaoshuai/PV-RCNN)
* **PV-RCNN++: Point-Voxel Feature Set Abstraction with Local Vector Representation**, IJCV 2022, [ :link: ](https://link.springer.com/article/10.1007/s11263-022-01710-9) [ :octocat: ](https://github.com/open-mmlab/OpenPCDet) 
* **PointAugmenting: Cross-Modal Augmentation for 3D Object Detection**, CVPR 2021, [ :link: ](https://openaccess.thecvf.com/content/CVPR2021/papers/Wang_PointAugmenting_Cross-Modal_Augmentation_for_3D_Object_Detection_CVPR_2021_paper.pdf) [ :octocat: ](https://github.com/VISION-SJTU/PointAugmenting)
* **VISTA: Boosting 3D Object Detection via Dual Cross-VIew SpaTial Attention**, CVPR 2022, [ :link: ](https://openaccess.thecvf.com/content/CVPR2022/papers/Deng_VISTA_Boosting_3D_Object_Detection_via_Dual_Cross-VIew_SpaTial_Attention_CVPR_2022_paper.pdf) [ :octocat: ](https://github.com/Gorilla-Lab-SCUT/VISTA) 
* **CVFNet: Real-time 3D Object Detection by Learning Cross View Features**, IROS 2022, [ :link: ](https://arxiv.org/abs/2203.06585) [ :octocat: ](https://github.com/open-mmlab/mmdetection3d) 
* **TransFusion: Robust LiDAR-Camera Fusion for 3D Object Detection with Transformers**, CVPR 2022, [ :link: ](https://openaccess.thecvf.com/content/CVPR2022/papers/Bai_TransFusion_Robust_LiDAR-Camera_Fusion_for_3D_Object_Detection_With_Transformers_CVPR_2022_paper.pdf) [ :octocat: ](https://github.com/XuyangBai/TransFusion) 
* **Bridged Transformer for Vision and Point Cloud 3D Object Detection**, CVPR 2022, [ :link: ](https://openaccess.thecvf.com/content/CVPR2022/papers/Wang_Bridged_Transformer_for_Vision_and_Point_Cloud_3D_Object_Detection_CVPR_2022_paper.pdf) [ :octocat: ](https://github.com/open-mmlab/mmdetection3d) 
* **FUTR3D: A Unified Sensor Fusion Framework for 3D Detection**, CVPRW 2023, [ :link: ](https://openaccess.thecvf.com/content/CVPR2023W/WAD/papers/Chen_FUTR3D_A_Unified_Sensor_Fusion_Framework_for_3D_Detection_CVPRW_2023_paper.pdf) [ :octocat: ](https://github.com/Tsinghua-MARS-Lab/futr3d) 
* **GAFusion: Adaptive Fusing LiDAR and Camera with Multiple Guidance for 3D Object Detection**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Li_GAFusion_Adaptive_Fusing_LiDAR_and_Camera_with_Multiple_Guidance_for_CVPR_2024_paper.pdf) [ :octocat: ](https://github.com/open-mmlab/mmdetection3d) 
* **RCBEVDet: Radar-camera Fusion in Bird’s Eye View for 3D Object Detection**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Lin_RCBEVDet_Radar-camera_Fusion_in_Birds_Eye_View_for_3D_Object_CVPR_2024_paper.pdf) [ :octocat: ](https://github.com/VDIGPKU/RCBEVDet)
* **Towards Robust 3D Object Detection with LiDAR and 4D Radar Fusion in Various Weather Conditions**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Chae_Towards_Robust_3D_Object_Detection_with_LiDAR_and_4D_Radar_CVPR_2024_paper.pdf) [ :octocat: ](https://github.com/yujeong-star/RL_3DOD) 
* **LiRaFusion: Deep Adaptive LiDAR-Radar Fusion for 3D Object Detection**, ICRA 2024, [ :link: ](https://arxiv.org/abs/2402.11735) [ :octocat: ](https://github.com/Song-Jingyu/LiRaFusion) 
* **Ev-3DOD: Pushing the Temporal Boundaries of 3D Object Detection with Event Cameras**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/papers/Cho_Ev-3DOD_Pushing_the_Temporal_Boundaries_of_3D_Object_Detection_with_CVPR_2025_paper.pdf) [ :octocat: ](https://github.com/mickeykang16/Ev3DOD) 
* **V2X-R: Cooperative LiDAR–4D Radar Fusion for 3D Object Detection**, CVPR 2025, [ :link: ](https://arxiv.org/abs/2411.08402) [ :octocat: ](https://github.com/ylwhxht/V2X-R)

### Detection Stage
#### One-Stage Detectors
* **SA-SSD: Structure Aware Single-Stage 3D Object Detection From Point Cloud**, CVPR 2020, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2020/papers/He_Structure_Aware_Single-Stage_3D_Object_Detection_From_Point_Cloud_CVPR_2020_paper.pdf) [ :octocat: ](https://github.com/skyhehe123/SA-SSD)
* **Embracing Single Stride 3D Object Detector with Sparse Transformer (SST)**, CVPR 2022, [ :link: ](https://openaccess.thecvf.com/content/CVPR2022/papers/Fan_Embracing_Single_Stride_3D_Object_Detector_With_Sparse_Transformer_CVPR_2022_paper.pdf) [ :octocat: ](https://github.com/tusen-ai/SST)
* **BEVFormer: Learning Bird’s-Eye-View Representation from Multi-Camera Images via Spatiotemporal Transformers**, ECCV 2022, [ :link: ](https://arxiv.org/abs/2203.17270) [ :octocat: ](https://github.com/fundamentalvision/BEVFormer)
* **DSVT: Dynamic Sparse Voxel Transformer with Rotated Sets**, CVPR 2023, [ :link: ](https://arxiv.org/abs/2301.06051) [ :octocat: ](https://github.com/Haiyang-W/DSVT)
* **SparseBEV: High-Performance Sparse 3D Object Detection from Multi-Camera Videos**, ICCV 2023, [ :link: ](https://arxiv.org/abs/2308.09244) [ :octocat: ](https://github.com/MCG-NJU/SparseBEV)
* **BEVNeXt: Reviving BEVDet for Efficient Multi-View 3D Object Detection**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Li_BEVNeXt_Reviving_Dense_BEV_Frameworks_for_3D_Object_Detection_CVPR_2024_paper.pdf) [ :octocat: ](https://github.com/woxihuanjiangguo/BEVNeXt)

#### Two-Stage Detectors
* **PV-RCNN: Point-Voxel Feature Set Abstraction for 3D Object Detection**, CVPR 2020, [ :link: ](https://arxiv.org/abs/1912.13192) [ :octocat: ](https://github.com/open-mmlab/OpenPCDet)
* **PV-RCNN++: Point-Voxel Feature Set Abstraction With Local Vector Representation for 3D Object Detection**, IJCV 2023, [ :link: ](https://arxiv.org/abs/2102.00463) [ :octocat: ](https://github.com/open-mmlab/OpenPCDet)
* **Voxel R-CNN: Towards High Performance Voxel-based 3D Object Detection**, AAAI 2021, [ :link: ](https://arxiv.org/abs/2012.15712) [ :octocat: ](https://github.com/djiajunustc/Voxel-R-CNN)
* **LiDAR R-CNN: An Efficient and Universal 3D Object Detector**, CVPR 2021, [ :link: ](https://arxiv.org/abs/2103.15297) [ :octocat: ](https://github.com/tusen-ai/LiDAR_RCNN)
* **Pyramid R-CNN: Towards Better Performance and Adaptability for 3D Object Detection**, ICCV 2021, [ :link: ](https://openaccess.thecvf.com/content/ICCV2021/papers/Mao_Pyramid_R-CNN_Towards_Better_Performance_and_Adaptability_for_3D_Object_ICCV_2021_paper.pdf) [ :octocat: ](https://github.com/PointsCoder/Pyramid-RCNN)
* **CT3D: Improving 3D Object Detection With Channel-Wise Transformer**, ICCV 2021, [ :link: ](https://arxiv.org/abs/2108.10723) [ :octocat: ](https://github.com/hlsheng1/CT3D)
* **DiffRefine: Diffusion-Based Proposal Refinement for 3D Object Detection**, 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/papers/Shin_DiffRefine_Diffusion-based_Proposal_Specific_Point_Cloud_Densification_for_Cross-Domain_Object_ICCV_2025_paper.pdf)
### Anchor Strategy

### Sensor Modality

### Backbone Type

### Scene Type
#### Indoor 3D Object Detection
- **ImVoteNet: Boosting 3D Object Detection in Point Clouds with Image Votes**, CVPR 2020, [ :link: ](https://arxiv.org/abs/2001.10692) [ :octocat: ](https://github.com/facebookresearch/imvotenet)
- **H3DNet: 3D Object Detection Using Hybrid Geometric Primitives**, ECCV 2020, [ :link: ](https://arxiv.org/abs/2006.05682) [ :octocat: ](https://github.com/zaiweizhang/H3DNet)
- **3DETR: An End-to-End Transformer Model for 3D Object Detection**, ICCV 2021, [ :link: ](https://arxiv.org/abs/2109.08141) [ :octocat: ](https://github.com/facebookresearch/3detr)
- **Group-Free 3D Object Detection via Transformers**, ICCV 2021, [ :link: ](https://arxiv.org/abs/2104.00678) [ :octocat: ](https://github.com/zeliu98/Group-Free-3D)
- **FCAF3D: Fully Convolutional Anchor-Free 3D Object Detection**, ECCV 2022, [ :link: ](https://arxiv.org/abs/2112.00322)
- **V-DETR: DETR with Vertex Relative Position Encoding for 3D Object Detection**, arXiv 2023, [ :link: ](https://arxiv.org/abs/2308.04409) [ :octocat: ](https://github.com/V-DETR/V-DETR)

#### Outdoor LiDAR-based 3D Object Detection
- **3DSSD: Point-Based 3D Single Stage Object Detector**, CVPR 2020, [ :link: ](https://arxiv.org/abs/2002.10187) [ :octocat: ](https://github.com/JIA-Lab-research/3DSSD)
- **SA-SSD: Structure Aware Single-stage 3D Object Detection from Point Cloud**, CVPR 2020, [ :link: ]([https://www4.comp.polyu.edu.hk/~cslzhang/paper/SA-SSD.pdf](https://openaccess.thecvf.com/content_CVPR_2020/papers/He_Structure_Aware_Single-Stage_3D_Object_Detection_From_Point_Cloud_CVPR_2020_paper.pdf)) [ :octocat: ](https://github.com/skyhehe123/SA-SSD)
- **CIA-SSD: Confident IoU-Aware Single-Stage Object Detector From Point Cloud**, AAAI 2021, [ :link: ](https://arxiv.org/abs/2012.03015) [ :octocat: ](https://github.com/Vegeta2020/CIA-SSD)
- **CenterPoint: Center-based 3D Object Detection and Tracking**, CVPR 2021, [ :link: ](https://arxiv.org/abs/2006.11275) [ :octocat: ](https://github.com/tianweiy/CenterPoint)
- **Voxel R-CNN: Towards High Performance Voxel-based 3D Object Detection**, AAAI 2021, [ :link: ](https://arxiv.org/abs/2012.15712) [ :octocat: ](https://github.com/djiajunustc/Voxel-R-CNN)
- **LiDAR R-CNN: An Efficient and Universal 3D Object Detector**, CVPR 2021, [ :link: ](https://arxiv.org/abs/2103.15297) [ :octocat: ](https://github.com/tusen-ai/LiDAR_RCNN)
- **RangeDet: In Defense of Range View for LiDAR-based 3D Object Detection**, ICCV 2021, [ :link: ](https://arxiv.org/abs/2103.10039) [ :octocat: ](https://github.com/tusen-ai/RangeDet)
- **VoTr: Voxel Transformer for 3D Object Detection**, ICCV 2021, [ :link: ](https://arxiv.org/abs/2109.02497) [ :octocat: ](https://github.com/PointsCoder/VOTR)
- **SST: Embracing Single Stride 3D Object Detector with Sparse Transformer**, CVPR 2022, [ :link: ](https://arxiv.org/abs/2112.06375) [ :octocat: ](https://github.com/tusen-ai/SST)
- **CenterFormer: Center-based Transformer for 3D Object Detection**, ECCV 2022, [ :link: ](https://arxiv.org/abs/2209.05588) [ :octocat: ](https://github.com/TuSimple/centerformer)
- **MPPNet: Multi-Frame Feature Intertwining with Proxy Points for 3D Temporal Object Detection**, ECCV 2022, [ :link: ](https://arxiv.org/abs/2205.05979) [ :octocat: ](https://github.com/open-mmlab/OpenPCDet)
- **FSD: Fully Sparse 3D Object Detection**, NeurIPS 2022, [ :link: ]([https://proceedings.neurips.cc/paper_files/paper/2022/hash/02a42f36b9d1fd6c8ec5286120a98e8e-Abstract-Conference.html) [ :octocat: ](https://github.com/liyingyanUCAS/FSD](https://arxiv.org/abs/2207.10035))
- **DSVT: Dynamic Sparse Voxel Transformer With Rotated Sets**, CVPR 2023, [ :link: ](https://arxiv.org/abs/2301.06051) [ :octocat: ](https://github.com/Haiyang-W/DSVT)
- **PillarNeXt: Rethinking Network Designs for 3D Object Detection in LiDAR Point Clouds**, CVPR 2023, [ :link: ](https://arxiv.org/abs/2305.04925) [ :octocat: ](https://github.com/qcraftai/pillarnext)
- **VoxelNeXt: Fully Sparse VoxelNet for 3D Object Detection and Tracking**, CVPR 2023, [ :link: ](https://arxiv.org/abs/2303.11301) [ :octocat: ](https://github.com/JIA-Lab-research/VoxelNeXt)

#### Outdoor LiDAR-Camera Fusion
- **PointPainting: Sequential Fusion for 3D Object Detection**, CVPR 2020, [ :link: ](https://arxiv.org/abs/1911.10150)
- **3D-CVF: Cross-View Spatial Feature Fusion for 3D Object Detection**, ECCV 2020, [ :link: ](https://arxiv.org/abs/2004.12636) [ :octocat: ](https://github.com/rasd3/3D-CVF)
- **TransFusion: Robust LiDAR-Camera Fusion for 3D Object Detection with Transformers**, CVPR 2022, [ :link: ](https://arxiv.org/abs/2203.11496) [ :octocat: ](https://github.com/XuyangBai/TransFusion)
- **BEVFusion: A Simple and Robust LiDAR-Camera Fusion Framework**, NeurIPS 2022, [ :link: ](https://arxiv.org/abs/2205.13790) [ :octocat: ](https://github.com/ADLab-AutoDrive/BEVFusion)
- **GA-Fusion: Adaptive Fusing LiDAR and Camera with Multiple Guidance for 3D Object Detection**, CVPR 2024, [ :link: ](https://arxiv.org/abs/2411.00340)
- **SparseLIF: High-Performance Sparse LiDAR-Camera Fusion for 3D Object Detection**, ECCV 2024, [ :link: ](https://arxiv.org/abs/2403.07284)
- **MambaFusion: Height-Fidelity Dense Global Fusion for Multi-modal 3D Object Detection**, arXiv 2025, [ :link: ](https://arxiv.org/abs/2507.04369) [ :octocat: ](https://github.com/AutoLab-SAI-SJTU/MambaFusion)
### Supervision
#### Weakly-supervised 3D Detection
- **WS3D: Weakly Supervised 3D Object Detection from Lidar Point Cloud**, ECCV 2020, [ :link: ](https://arxiv.org/abs/2007.11901) [ :octocat: ](https://github.com/hlesmqh/WS3D)
- **Weakly supervised 3d object detection from point clouds**, ACM MM 2020, [ :link: ](https://arxiv.org/abs/2007.13970) [ :octocat: ](https://github.com/Zengyi-Qin/Weakly-Supervised-3D-Object-Detection)
- **Towards a weakly supervised framework for 3D point cloud object detection and annotation**, T-PAMI 2021, [ :link: ](https://ieeexplore.ieee.org/document/9369074)
- **Back to Reality: Weakly-Supervised 3D Object Detection with Shape-guided Label Enhancement**, CVPR 2022, [ :link: ](https://arxiv.org/abs/2203.05238) [ :octocat: ](https://github.com/wyf-ACCEPT/BackToReality)
- **A simple vision transformer for weakly semi-supervised 3d object detection**, CVPR 2023, [ :link: ](https://openaccess.thecvf.com/content/ICCV2023/html/Zhang_A_Simple_Vision_Transformer_for_Weakly_Semi-supervised_3D_Object_Detection_ICCV_2023_paper.html) [ :octocat: ](https://github.com/DYZhang09/ViTWSS3D)
- **Prompt3D: Random Prompt Assisted Weakly-Supervised 3D Object Detection**, CVPR 2024, [ :link: ](https://ieeexplore.ieee.org/document/10655852) [ :octocat: ](https://github.com/huishengye/prompt3d)
- **G-W3D: Weakly Supervised 3D Object Detection via Multi-level Visual Guidance**, ECCV 2024, [ :link: ](https://arxiv.org/abs/2312.07530) [ :octocat: ](https://github.com/kuanchihhuang/VG-W3D)
- **Weakly supervised monocular 3D object detection by spatial-temporal view consistency**, T-PAMI 2024, [ :link: ](https://ieeexplore.ieee.org/document/10689672)

#### Semi-supervised 3D Detection
- **SESS: Self-Ensembling Semi-Supervised 3D Object Detection**, CVPR 2020, [ :link: ](https://arxiv.org/abs/1912.11803) [ :octocat: ](https://github.com/Na-Z/sess)
- **3DIoUMatch: Leveraging IoU Prediction for Semi-Supervised 3D Object Detection**, CVPR 2021, [ :link: ](https://arxiv.org/abs/2012.04355) [ :octocat: ](https://github.com/yezhen17/3DIoUMatch)
- **Semi-supervised 3D object detection with proficient teachers**, ECCV 2022, [ :link: ](https://arxiv.org/abs/2207.12655) [ :octocat: ](https://github.com/yinjunbo/ProficientTeachers)
- **NoiseDet: Learning from Noisy Data for Semi-Supervised 3D Object Detection**, ICCV 2023, [ :link: ](https://ieeexplore.ieee.org/document/10377714) [ :octocat: ](https://github.com/zehuichen123/NoiseDet)
- **Ssda3d: Semi-supervised domain adaptation for 3d object detection from point cloud**, AAAI 2023, [ :link: ](https://arxiv.org/abs/2212.02845) [ :octocat: ](https://github.com/yinjunbo/SSDA3D)
- **PatchTeacher & PillarMix: Semi-supervised 3D Object Detection with PatchTeacher and PillarMix**, AAAI 2024, [ :link: ](https://arxiv.org/abs/2407.09787) [ :octocat: ](https://github.com/LittlePey/PTPM)
- **Decoupled pseudo-labeling for semi-supervised monocular 3d object detection**, CVPR 2024, [ :link: ](https://arxiv.org/abs/2403.17387)
- **Reflective Teacher: Semi-Supervised Multimodal 3D Object Detection in Bird's-Eye-View via Uncertainty Measure**, WACV 2025, [ :link: ](https://arxiv.org/abs/2412.04337)
- **SP3D: Boosting Sparsely-Supervised 3D Object Detection via Accurate Cross-Modal Semantic Prompts**, CVPR 2025, [ :link: ](https://arxiv.org/abs/2503.06467) [ :octocat: ](https://github.com/xmuqimingxia/SP3D)
- **Leveraging temporal cues for semi-supervised multi-view 3D object detection**, CVPR 2025, [ :link: ](https://ieeexplore.ieee.org/document/11093461/)
- **Power of Cooperative Supervision: Multiple Teachers Framework for Advanced 3D Semi-Supervised Object Detection**, ICCV 2025, [ :link: ](https://arxiv.org/abs/2405.20720) [ :octocat: ](https://github.com/JH-Research/MultipleTeachers)


#### Self-/Unsupervised 3D Detection
- **Unsupervised Pre-training for 3D Point Cloud Understanding**, ECCV 2020, [ :link: ](https://arxiv.org/abs/2007.10985) [ :octocat: ](https://github.com/facebookresearch/PointContrast)
- **Unsupervised Pre-Training from Synthetic Shapes and Randomized Layouts for 3D Object Detection**, ICCV 2021, [ :link: ](https://arxiv.org/abs/2108.07794)
- **Exploring geometry-aware contrast and clustering harmonization for self-supervised 3d object detection**, ICCV 2021, [ :link: ](https://ieeexplore.ieee.org/document/9711148)
- **3d object detection with a self-supervised lidar scene flow backbone**, ECCV 2022, [ :link: ](https://arxiv.org/abs/2205.00705) [ :octocat: ](https://github.com/emecercelik/ssl-3d-detection)
- **ProposalContrast: Unsupervised Pre-training for LiDAR-Based 3D Object Detection**, ECCV 2022, [ :link: ](https://arxiv.org/abs/2207.12654) [ :octocat: ](https://github.com/yinjunbo/ProposalContrast)
- **Liso: Lidar-only self-supervised 3d object detection**, ECCV 2024, [ :link: ](https://arxiv.org/abs/2403.07071) [ :octocat: ](https://github.com/baurst/liso)
- **Approaching outside: Scaling unsupervised 3d object detection from 2d scene**, ECCV 2024, [ :link: ](https://arxiv.org/abs/2407.08569) [ :octocat: ](https://github.com/Ruiyang-061X/LiSe)
- **Commonsense prototype for outdoor unsupervised 3d object detection**, CVPR 2024, [ :link: ](https://arxiv.org/abs/2404.16493) [ :octocat: ](https://github.com/hailanyi/CPD)
- **Union: Unsupervised 3d object detection using object appearance-based pseudo-classes**, NeurIPS 2024, [ :link: ](https://arxiv.org/abs/2405.15688) [ :octocat: ](https://github.com/TedLentsch/UNION)
- **Learning to Detect Objects from Multi-Agent LiDAR Scans without Manual Labels**, CVPR 2025, [ :link: ](https://arxiv.org/abs/2503.08421) [ :octocat: ](https://github.com/xmuqimingxia/DOtAv2)
- **Patchcontrast: Self-supervised pre-training for 3d object detection**, CVPRW 2025, [ :link: ](https://arxiv.org/abs/2308.06985)
- **CMAE-3D: contrastive masked AutoEncoders for self-supervised 3D object detection**, IJCV 2025, [ :link: ](https://link.springer.com/article/10.1007/s11263-024-02313-2)

 * [](#Motion-based)
 * [Transformer-based](#Transformer-based)
* [RGB–LiDAR Trackers](#LRGB–LiDAR-Trackers)


## Tracking

### Single-Object Tracking

#### Survey

* **Visual Object Tracking across Diverse Data Modalities: A Review**, Arxiv 2024, [ :link: ](https://arxiv.org/abs/2412.09991)

### LiDAR Trackers

#### Siamese-based
 
* **Leveraging Shape Completion for 3D Siamese Tracking**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2019/html/Giancola_Leveraging_Shape_Completion_for_3D_Siamese_Tracking_CVPR_2019_paper.html), [ :octocat: ](https://github.com/SilvioGiancola/ShapeCompletion3DTracking)

* **P2B: Point-to-Box Network for 3D Object Tracking in Point Clouds**, CVPR 2020, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2020/html/Qi_P2B_Point-to-Box_Network_for_3D_Object_Tracking_in_Point_Clouds_CVPR_2020_paper.html) [ :octocat: ](https://github.com/HaozheQi/P2B)
  
* **3D-SiamRPN: An End-to-End Learning Method for Real-Time 3D Single Object Tracking Using Raw Point Cloud**, IEEE Sensors Journal 2021, [ :link: ](https://ieeexplore.ieee.org/abstract/document/9235506)

* **MLVSNet: Multi-Level Voting Siamese Network for 3D Visual Tracking**, ICCV 2021, [ :link: ](https://openaccess.thecvf.com/content/ICCV2021/html/Wang_MLVSNet_Multi-Level_Voting_Siamese_Network_for_3D_Visual_Tracking_ICCV_2021_paper.html), [ :octocat: ](https://github.com/CodeWZT/MLVSNet) 

* **Box-Aware Feature Enhancement for Single Object Tracking on Point Clouds**, ICCV 2021, [ :link: ](https://openaccess.thecvf.com/content/ICCV2021/html/Zheng_Box-Aware_Feature_Enhancement_for_Single_Object_Tracking_on_Point_Clouds_ICCV_2021_paper.html), [ :octocat: ](https://github.com/Ghostish/Open3DSOT) 

* **3D Siamese Voxel-to-BEV Tracker for Sparse Point Clouds**, NeurIPS 2021, [ :link: ](https://proceedings.neurips.cc/paper/2021/hash/f0fcf351df4eb6786e9bb6fc4e2dee02-Abstract.html), [ :octocat: ](https://github.com/fpthink/V2B) 

* **PTT: Point-Track-Transformer Module for 3D Single Object Tracking in Point Clouds**, IROS 2021, [ :link: ](https://ieeexplore.ieee.org/abstract/document/9636821), [ :octocat: ](https://github.com/shanjiayao/PTT) 

* **PTTR: Relational 3D Point Cloud Object Tracking With Transformer**, CVPR 2022, [ :link: ](https://openaccess.thecvf.com/content/CVPR2022/html/Zhou_PTTR_Relational_3D_Point_Cloud_Object_Tracking_With_Transformer_CVPR_2022_paper.html), [ :octocat: ](https://github.com/Jasonkks/PTTR) 

#### Motion-based

* **Beyond 3D Siamese Tracking: A Motion-Centric Paradigm for 3D Single Object Tracking in Point Clouds**, CVPR 2022, [ :link: ](https://openaccess.thecvf.com/content/CVPR2022/html/Zheng_Beyond_3D_Siamese_Tracking_A_Motion-Centric_Paradigm_for_3D_Single_CVPR_2022_paper.html), [ :octocat: ](https://github.com/Ghostish/Open3DSOT) 

* **A lightweight and detector-free 3d single object tracker on point clouds**, IEEE Transactions on Intelligent Transportation Systems 2023, [ :link: ](https://ieeexplore.ieee.org/abstract/document/10050385), [ :octocat: ](https://github.com/jimmy-dq/DMT) 

* **Towards Category Unification of 3D Single Object Tracking on Point Clouds**, ICLR 2024, [ :link: ](https://arxiv.org/abs/2401.11204)

* **Focustrack: One-stage focus-and-suppress framework for 3d point cloud object tracking**, ACM MM 2025, [ :link: ](https://dl.acm.org/doi/abs/10.1145/3746027.3754781) 

* **Beyond Frame-Wise Tracking: A Trajectory-Based Paradigm for Efficient Point Cloud Tracking**, IEEE Robotics and Automation Letters 2026, [ :link: ](https://ieeexplore.ieee.org/abstract/document/11358684), [ :octocat: ](https://github.com/FiBonaCci225/TrajTrack) 

#### Transformer-based

* **Real-Time 3D Single Object Tracking With Transformer**, IEEE Transactions on Multimedia 2022, [ :link: ](https://ieeexplore.ieee.org/abstract/document/9695195)

* **CXTrack: Improving 3D Point Cloud Tracking With Contextual Information**, CVPR 2023, [ :link: ](https://openaccess.thecvf.com/content/CVPR2023/html/Xu_CXTrack_Improving_3D_Point_Cloud_Tracking_With_Contextual_Information_CVPR_2023_paper.html), [ :octocat: ](https://github.com/slothfulxtx/cxtrack3d) 

* **MBPTrack: Improving 3D Point Cloud Tracking with Memory Networks and Box Priors**, ICCV 2023, [ :link: ](https://openaccess.thecvf.com/content/ICCV2023/html/Xu_MBPTrack_Improving_3D_Point_Cloud_Tracking_with_Memory_Networks_and_ICCV_2023_paper.html)

* **Correlation Pyramid Network for 3D Single Object Tracking**, CVPR 2023, [ :link: ](https://openaccess.thecvf.com/content/CVPR2023W/E2EAD/html/Wang_Correlation_Pyramid_Network_for_3D_Single_Object_Tracking_CVPRW_2023_paper.html)

* **3D Single-Object Tracking in Point Clouds with High Temporal Variation**, ECCV 2024, [ :link: ](https://link.springer.com/chapter/10.1007/978-3-031-72667-5_16)

### RGB-LiDAR Trackers

* **MMF-Track: Multi-Modal Multi-Level Fusion for 3D Single Object Tracking**, IEEE Transactions on Intelligent Vehicles 2024, [ :link: ](https://ieeexplore.ieee.org/abstract/document/10292917), [ :octocat: ](https://github.com/NEU-REAL/MMF-Tracker) 

* **Exploring Point-BEV Fusion for 3D Point Cloud Object Tracking With Transformer**, IEEE Transactions on Pattern Analysis and Machine Intelligence 2024, [ :link: ](https://ieeexplore.ieee.org/abstract/document/10460168), [ :octocat: ](https://github.com/Jasonkks/PTTR) 

* **MVCTrack: Boosting 3D Point Cloud Tracking via Multimodal-Guided Virtual Cues**, ICRA 2025, [ :link: ](https://ieeexplore.ieee.org/abstract/document/11128337)

* **3D Single Object Tracking With Cross-Modal Fusion Conflict Elimination**, IEEE Transactions on Pattern Analysis and Machine Intelligence 2024, [ :link: ](https://ieeexplore.ieee.org/abstract/document/10930556)


## Compression

* **Octree-based Point-Cloud Compression**, SPBG'06: Proceedings of the 3rd Eurographics / IEEE VGTC conference on Point-Based Graphics 2006, [ :link: ](https://dl.acm.org/doi/10.5555/2386388.2386404)

* **Point cloud attribute compression with graph transform**, IEEE International Conference on Image Processing (ICIP) 2014, [ :link: ](https://ieeexplore.ieee.org/document/7025414/)

* **Graph-based motion estimation and compensation for dynamic 3D point cloud compression**, IEEE International Conference on Image Processing (ICIP) 2015, [ :link: ](https://ieeexplore.ieee.org/document/9194311/)

* **3d point cloud geometry compression on deep learning**, ACM International Conference on Multimedia 2019, [ :link: ](https://dl.acm.org/doi/10.1145/3343031.3351061)

* **Towards 6dof http adaptive streaming through point cloud compression**, ACM International Conference on Multimedia 2019, [ :link: ](https://dl.acm.org/doi/10.1145/3343031.3350917)

* **Learning convolutional transforms for lossy point cloud geometry compression**, IEEE international conference on image processing (ICIP) 2019, [ :link: ](https://arxiv.org/pdf/1903.08548) [ :octocat: ](https://github.com/mauriceqch/pcc_geo_cnn)

* **Model-based joint bit allocation between geometry and color for video-based 3D point cloud compression**, IEEE Transactions on Multimedia 2020, [ :link: ](https://ieeexplore.ieee.org/document/9194311/) 

* **Lossy point cloud geometry compression via end-to-end learning**, IEEE Transactions on Circuits and Systems for Video Technology 2021, [ :link: ](https://ieeexplore.ieee.org/document/9321375/)

* **Voxelcontext-net: An octree based framework for point cloud compression**, CVPR 2021, [ :link: ](https://openaccess.thecvf.com/content/CVPR2021/papers/Que_VoxelContext-Net_An_Octree_Based_Framework_for_Point_Cloud_Compression_CVPR_2021_paper.pdf)

* **Multiscale point cloud geometry compression**, Data Compression Conference (DCC) 2021, [ :link: ](https://ieeexplore.ieee.org/iel7/9418628/9418635/09418789.pdf) [ :octocat: ](https://github.com/NJUVISION/PCGCv2)

* **Deep compression for dense point cloud maps**,  IEEE Robotics and Automation Letters 2021, [ :link: ](https://ieeexplore.ieee.org/document/9354895/) [ :octocat: ](https://github.com/PRBonn/deep-point-map-compression)

* **Reduced reference perceptual quality model with application to rate control for video-based point cloud compression**, IEEE Transactions on Image Processing 2021, [ :link: ](https://ieeexplore.ieee.org/document/9490512)

* **GRASP-Net: Geometric residual analysis and synthesis for point cloud compression**, Proceedings of the 1st International Workshop on Advances in Point Cloud Compression, Processing and Analysis 2022, [ :link: ](https://arxiv.org/pdf/2209.04401.pdf) [ :octocat: ](https://github.com/InterDigitalInc/GRASP-Net)


* **Octattention: Octree-based large-scale contexts model for point cloud compression**, AAAI 2022, [ :link: ](https://cdn.aaai.org/ojs/19942/19942-13-23955-1-2-20220628.pdf) [ :octocat: ](https://github.com/zb12138/OctAttention)

* **4dac: Learning attribute compression for dynamic point clouds**, Arxiv 2022, [ :link: ](https://arxiv.org/pdf/2204.11723)

* **Point cloud compression with range image-based entropy model for autonomous driving**, ECCV 2022, [ :link: ](https://www.ecva.net/papers/eccv_2022/papers_ECCV/papers/136820315.pdf)

* **Rate-distortion modeling for bit rate constrained point cloud compression**, IEEE Transactions on Circuits and Systems for Video Technology 2022, [ :link: ](https://ieeexplore.ieee.org/document/9957096)

* **Sparse tensor-based point cloud attribute compression**, International Conference on Multimedia Information Processing and Retrieval (MIPR) 2022, [ :link: ](https://ieeexplore.ieee.org/document/9874468/)

* **Lossless point cloud attribute compression using cross-scale, cross-group, and cross-color prediction**, Data Compression Conference (DCC) 2023, [ :link: ](https://ieeexplore.ieee.org/iel7/10125292/10125296/10125514.pdf)

* **YOGA: Yet another geometry-based point cloud compressor**, ACM International Conference on Multimedia 2023, [ :link: ](https://dl.acm.org/doi/10.1145/3581783.3613847) [ :octocat: ](https://github.com/3dpcc/YOGAv1)

* **Multiscale latent-guided entropy model for lidar point cloud compression**, IEEE Transactions on Circuits and Systems for Video Technology 2023, [ :link: ](https://ieeexplore.ieee.org/iel7/76/4358651/10129923.pdf)

* **Lossless point cloud geometry and attribute compression using a learned conditional probability model**, IEEE Transactions on Circuits and Systems for Video Technology 2023, [ :link: ](https://ieeexplore.ieee.org/iel7/76/10207864/10024999.pdf)

* **Efficient hierarchical entropy model for learned point cloud compression**, CVPR 2023, [ :link: ](https://openaccess.thecvf.com/content/CVPR2023/papers/,Song_Efficient_Hierarchical_Entropy_Model_for_Learned_Point_Cloud_Compression_CVPR_2023_paper.pdf)


* **msLPCC: A multimodal-driven scalable framework for deep LiDAR point cloud compression**, AAAI 2024, [ :link: ]( https://ojs.aaai.org/index.php/AAAI/article/view/28362)[ :octocat: ]( https://github.com/I2-Multimedia-Lab/Pointsoup)

* **Pointsoup: High-performance and extremely low-decoding-latency learned geometry codec for large-scale point cloud scenes**, IJCAI 2024, [ :link: ](https://www.ijcai.org/proceedings/2024/0595.pdf) [ :octocat: ]( https://github.com/I2-Multimedia-Lab/Pointsoup)


* **Pdnet: parallel dual-branch network for point cloud geometry compression and analysis**, Data Compression Conference (DCC) 2024, [ :link: ](https://ieeexplore.ieee.org/document/10533742/)


* **Inter-frame compression for dynamic point cloud geometry coding**, IEEE Transactions on Image Processing 2024, [ :link: ](https://arxiv.org/pdf/2207.12554) [ :octocat: ](https://github.com/aniqueakhtar/PointCloudCompression)

* **Ecm-opcc: Efficient context model for octree-based point cloud compression**, ICASSP 2024, [ :link: ](https://ieeexplore.ieee.org/document/10446374/)

* **Point cloud compression with implicit neural representations: A unified framework**, ICCC 2024, [ :link: ](https://ieeexplore.ieee.org/iel8/10681633/10681675/10681880.pdf) [ :octocat: ](https://github.com/RhoHenning/INR-PCC)

* **Learned compression of point cloud geometry and attributes in a single model through multimodal rate-control**, Arxiv 2024, [ :link: ](https://arxiv.org/abs/2408.00599)

* **Roi-guided point cloud geometry compression towards human and machine vision**, ACM International Conference on Multimedia 2024, [ :link: ](https://dl.acm.org/doi/10.1145/3664647.3681301)

* **PCAC-GAN: a sparse-tensor-based generative adversarial network for 3d point cloud attribute compression**, Computational Visual Media 2025, [ :link: ](https://ieeexplore.ieee.org/abstract/document/11174068/)

* **Rendering-oriented 3d point cloud attribute compression using sparse tensor-based transformer**, IEEE 2025, [ :link: ](https://ieeexplore.ieee.org/abstract/document/10908209/) [ :octocat: ](https://github.com/net-F/RO-PCAC)

* **Voxel-based point cloud geometry compression with space-to-channel context**, Arxiv 2025, [ :link: ](https://arxiv.org/abs/2503.18283)

* **Octree-STCM: Octree-Based Spatio-Temporal Context Model for Lossless Geometry Compression of Dynamic Point Cloud**, ACM 2025, [ :link: ](https://dl.acm.org/doi/abs/10.1145/3731715.3733489)

* **DeepRAHT: Learning Predictive RAHT for Point Cloud Attribute Compression**, Arxiv 2026, [ :link: ](https://arxiv.org/abs/2601.12255,) [ :octocat: ](https://github.com/zb12138/DeepRAHT)

* **Octree-based learned point cloud geometry compression: a lossy perspective**, Arxiv 2026, [ :link: ](https://arxiv.org/abs/2603.28095)

* **OctMamba: Mamba-Based Octree Context Entropy Model for Point Cloud Geometry Compression**, Pattern Recognition 2026, [ :link: ](https://www.sciencedirect.com/science/article/abs/pii/S0031320326000762)

## 6DoF Pose Estimation

### Object Pose Estimation

#### Survey
* **Deep Learning-Based Object Pose Estimation: A Comprehensive Survey**, arXiv 2024, [ :link: ](https://arxiv.org/abs/2405.07801) [ :octocat: ](https://github.com/CNJianLiu/Awesome-Object-Pose-Estimation)

#### Instance-level (known instances)
* **DenseFusion: 6D Object Pose Estimation by Iterative Dense Fusion**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2019/papers/Wang_DenseFusion_6D_Object_Pose_Estimation_by_Iterative_Dense_Fusion_CVPR_2019_paper.pdf) [ :octocat: ](https://github.com/j96w/DenseFusion)
* **PVN3D: A Deep Point-Wise 3D Keypoints Voting Network for 6DoF Pose Estimation**, CVPR 2020, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2020/papers/He_PVN3D_A_Deep_Point-Wise_3D_Keypoints_Voting_Network_for_6DoF_CVPR_2020_paper.pdf) [ :octocat: ](https://github.com/ethnhe/PVN3D)
* **FFB6D: A Full Flow Bidirectional Fusion Network for 6D Pose Estimation**, CVPR 2021, [ :link: ](https://openaccess.thecvf.com/content/CVPR2021/papers/He_FFB6D_A_Full_Flow_Bidirectional_Fusion_Network_for_6D_Pose_CVPR_2021_paper.pdf) [ :octocat: ](https://github.com/ethnhe/FFB6D)
* **CloudAAE: Learning 6D Object Pose Regression with On-line Data Synthesis on Point Clouds**, arXiv 2021, [ :link: ](https://arxiv.org/abs/2103.01977) [ :octocat: ](https://github.com/GeeeG/CloudAAE)

#### Category-level (intra-category shape variation)
* **CASS: Learning Canonical Shape Space for Category-Level 6D Object Pose and Size Estimation**, CVPR 2020, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2020/papers/Chen_Learning_Canonical_Shape_Space_for_Category-Level_6D_Object_Pose_and_CVPR_2020_paper.pdf) [ :octocat: ](https://github.com/densechen/CASS)
* **AG-Pose: Instance-Adaptive and Geometric-Aware Keypoint Learning for Category-Level 6D Object Pose Estimation**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Lin_Instance-Adaptive_and_Geometric-Aware_Keypoint_Learning_for_Category-Level_6D_Object_Pose_CVPR_2024_paper.pdf) [ :octocat: ](https://github.com/Leeiieeo/AG-Pose)
* **CD-Pose: Learning geometric consistency and discrepancy for category-level 6D object pose estimation from point clouds**, Pattern Recognition 2024, [ :link: ](https://www.sciencedirect.com/science/article/pii/S0031320323005940) 
* **GCE-Pose: Global Context Enhancement for Category-level Object Pose Estimation**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/papers/Li_GCE-Pose_Global_Context_Enhancement_for_Category-level_Object_Pose_Estimation_CVPR_2025_paper.pdf) code: —

#### Unseen / zero-shot (generalize to novel objects)
* **OVE6D: Object Viewpoint Encoding for Depth-based 6D Object Pose Estimation**, CVPR 2022, [ :link: ](https://openaccess.thecvf.com/content/CVPR2022/papers/Cai_OVE6D_Object_Viewpoint_Encoding_for_Depth-Based_6D_Object_Pose_Estimation_CVPR_2022_paper.pdf) [ :octocat: ](https://github.com/dingdingcai/OVE6D-pose)
* **FreeZe: Training-free zero-shot 6D pose estimation with geometric and vision foundation models**, ECCV 2024, [ :link: ](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/09634.pdf) [ :octocat: ](https://github.com/andreacaraffa/freeze)
* **ZeroPose: CAD-Prompted Zero-shot Object 6D Pose Estimation in Cluttered Scenes**, arXiv 2023 / TCSVT 2024–2025, [ :link: ](https://arxiv.org/html/2305.17934v3) [ :octocat: ](https://github.com/shruthibalaji2307/zeropose)

### Human Pose Estimation
#### Surveys / overviews
* **3D Human Pose and Shape Estimation from LiDAR Point Clouds: A Review**, arXiv 2025, [ :link: ](https://arxiv.org/abs/2509.12197) [ :octocat: ](https://github.com/valeoai/3D-Human-Pose-Shape-Estimation-from-LiDAR)
* **Deep learning for 3D human pose estimation and mesh recovery: A survey**, arXiv 2024, [ :link: ](https://arxiv.org/abs/2402.18844) [ :octocat: ](https://github.com/liuyangme/SOTA-3DHPE-HMR)
* **Attention-Enhanced Lightweight Hourglass Network for Human Pose Estimation** (Kappan et al.), arXiv 2024/2025, [ :link: ](https://export.arxiv.org/abs/2412.06227)

#### Body-scanned / dense point clouds
* **Learning to Estimate 3D Human Pose From Point Cloud**, IEEE Sensors Journal 2020 (arXiv version 2022), [ :link: ](https://arxiv.org/abs/2212.12910) 
* **Efficient Human Pose Estimation via 3D Event Point Cloud**, 3DV 2022, [ :link: ](https://arxiv.org/abs/2206.04511) [ :octocat: ](https://github.com/MasterHow/EventPointPose)
* **SPiKE: 3D Human Pose from Point Cloud Sequences**, 2024 (book chapter 2025), [ :link: ](https://arxiv.org/abs/2409.01879) [ :octocat: ](https://github.com/iballester/SPiKE)

#### LiDAR point clouds (sparse, outdoor / long-range)
* **3D Human Keypoints Estimation From Point Clouds in the Wild Without Human Labels**, CVPR 2023, [ :link: ](https://openaccess.thecvf.com/content/CVPR2023/papers/Weng_3D_Human_Keypoints_Estimation_From_Point_Clouds_in_the_Wild_CVPR_2023_paper.pdf)
* **LidPose: Real-Time 3D Human Pose Estimation in Sparse Lidar Point Clouds with Non-Repetitive Circular Scanning Pattern**, Sensors 2024, [ :link: ](https://www.mdpi.com/1424-8220/24/11/3427) 
* **LPFormer: LiDAR Pose Estimation Transformer with Multi-Task Network**, ICRA 2024 (arXiv 2023), [ :link: ](https://arxiv.org/abs/2306.12525)
* **LiDARCapV2: 3D human pose estimation with human–object interaction from LiDAR point clouds**, Pattern Recognition 2024, [ :link: ](https://www.sciencedirect.com/science/article/pii/S0031320324005995) [ :octocat: ](https://github.com/jingyi-zhang/LiDARCapV2_)
* **Pre-training a Density-Aware Pose Transformer for Robust LiDAR-based 3D Human Pose Estimation (DAPT)**, AAAI 2025 (arXiv 2024), [ :link: ](https://arxiv.org/abs/2412.13454) [ :octocat: ](https://github.com/AnxQ/dapt)

#### Joint pose + body shape (SMPL/mesh) from point clouds
* **LiveHPS: LiDAR-based Scene-level Human Pose and Shape Estimation in Free Environment**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Ren_LiveHPS_LiDAR-based_Scene-level_Human_Pose_and_Shape_Estimation_in_Free_CVPR_2024_paper.pdf) [ :octocat: ](https://github.com/4DVLab/LiveHPS)
* **PointHPS: Cascaded 3D Human Pose and Shape Estimation from Point Clouds**, 2023 (IJCV 2026 version), [ :link: ](https://arxiv.org/abs/2308.14492) [ :octocat: ](https://github.com/MotrixLab/PointHPS)


## 3D Point Cloud Registration

### Surveys
* **Deep Learning-Based Point Cloud Registration: A Comprehensive Survey and Taxonomy**, arXiv 2024, [ :link: ](https://arxiv.org/abs/2404.13830) [ :octocat: ](https://github.com/yxzhang15/PCR)
* **3D Registration in 30 Years: A Survey**, arXiv 2024, [ :link: ](https://arxiv.org/abs/2412.13735) [ :octocat: ](https://github.com/Amyyyy11/3D-Registration-in-30-Years-A-Survey)
* **Rigid pairwise 3D point cloud registration: A survey**, Pattern Recognition 2024, [ :link: ](https://www.sciencedirect.com/science/article/pii/S0031320324001596) 

### Classical / geometry-based
* **A Method for Registration of 3-D Shapes (ICP)**, TPAMI 1992, [ :link: ](https://www-evasion.imag.fr/Membres/Franck.Hetroy/Teaching/ProjetsImage/2007/Bib/besl_mckay-pami1992.pdf) 
* **Efficient Variants of the ICP Algorithm**, 3DIM 2001, [ :link: ](https://www.cs.princeton.edu/~smr/papers/fasticp/fasticp_paper.pdf) 
* **Fast Global Registration**, ECCV 2016, [ :link: ](https://link.springer.com/content/pdf/10.1007/978-3-319-46475-6_47.pdf) [ :octocat: ](https://github.com/isl-org/FastGlobalRegistration)
* **Guaranteed Outlier Removal (GORE) for Point Cloud Registration with Correspondences**, arXiv 2017, [ :link: ](https://arxiv.org/abs/1711.10209) 
* **Robust low-overlap 3-D point cloud registration for outlier rejection**, 2019, [ :link: ](https://arpg.github.io/papers/hmrf_icp.pdf) 
* **Comparison of Point Cloud Registration Techniques on Scanned Physical Objects**, Sensors 2024, [ :link: ](https://www.mdpi.com/1424-8220/24/7/2142) 
* **Fast Robust Point Cloud Registration Based on Compatibility Graph and Accelerated Guided Sampling**, Remote Sensing 2024, [ :link: ](https://www.mdpi.com/2072-4292/16/15/2789) 
* **Research on the Improved ICP Algorithm for LiDAR Point Cloud Registration**, Sensors 2025, [ :link: ](https://www.mdpi.com/1424-8220/25/15/4748) 

### Learning-based
#### Supervised
* **BUFFER: Balancing Accuracy, Efficiency, and Generalizability in Point Cloud Registration**, CVPR 2023, [ :link: ](https://openaccess.thecvf.com/content/CVPR2023/papers/Ao_BUFFER_Balancing_Accuracy_Efficiency_and_Generalizability_in_Point_Cloud_Registration_CVPR_2023_paper.pdf) [ :octocat: ](https://github.com/SYSU-SAIL/BUFFER)
* **RORNet: Partial-to-Partial Registration Network with Reliable Overlapping Representations**, TNNLS 2023, [ :link: ](https://ywuchina.github.io/publications/paper11/) [ :octocat: ](https://github.com/superYuezhang/RORNet)
* **PARE-Net: Position-Aware Rotation-Equivariant Networks for Robust Point Cloud Registration**, ECCV 2024, [ :link: ](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/09456.pdf) [ :octocat: ](https://github.com/yaorz97/PARENet)
* **End-to-end point cloud registration with transformer**, Artificial Intelligence Review 2024, [ :link: ](https://link.springer.com/content/pdf/10.1007/s10462-024-10985-y.pdf) 

#### Unsupervised / self-supervised
* **UDPReg: Unsupervised Deep Probabilistic Approach for Partial Point Cloud Registration**, CVPR 2023, [ :link: ](https://openaccess.thecvf.com/content/CVPR2023/papers/Mei_Unsupervised_Deep_Probabilistic_Approach_for_Partial_Point_Cloud_Registration_CVPR_2023_paper.pdf) [ :octocat: ](https://github.com/pelekageorgia/UDPReg)
* **PointMBF: A Multi-scale Bidirectional Fusion Network for Unsupervised RGB-D Point Cloud Registration**, ICCV 2023, [ :link: ](https://openaccess.thecvf.com/content/ICCV2023/papers/Yuan_PointMBF_A_Multi-scale_Bidirectional_Fusion_Network_for_Unsupervised_RGB-D_Point_ICCV_2023_paper.pdf) [ :octocat: ](https://github.com/phdymz/PointMBF)
* **EYOC: Extend Your Own Correspondences (Unsupervised Distant Point Cloud Registration)**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Liu_Extend_Your_Own_Correspondences_Unsupervised_Distant_Point_Cloud_Registration_by_CVPR_2024_paper.pdf) [ :octocat: ](https://github.com/liuQuan98/EYOC)
* **RegiFormer: Unsupervised Point Cloud Registration via Geometric Local-to-Global Transformer and Self-Augmentation**, 2024, [ :link: ](https://openreview.net/pdf?id=RVGDEDO0f4)
* **GTINet: Global Topology-aware Interactions for Unsupervised Point Cloud Registration**, TCSVT 2024, [ :link: ](https://dblp.org/rec/journals/tcsv/JiangZLLC24.html)

---


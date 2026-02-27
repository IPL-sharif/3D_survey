# 3D Core Tasks

* [Classification](#Classification)

* [Segmentation](#Segmentation)

* [Detection](#Detection)
    * [Data Representation](#Data-Representation)
       * [point-based](#point-based)
       * [voxel-based](#voxel-based)
       * [pillar-based](#pillar-based)
       * [projection-based](#projection-based)
       * [hybrid](#hybrid)
     
   * [Supervision](#Supervision)
       * [Weakly-supervised 3D Detection](#Weakly-supervised-3D-Detection)
       * [Semi-supervised 3D Detection](#Semi-supervised-3D-Detection)
       * [Self-/Unsupervised 3D Detection](#Self-/Unsupervised-3D-Detection)
 
     
* [Tracking](#Tracking)

* [Compression](#Compression)

* [Registration and 6D Pose estimation](#Registration and 6D Pose estimation)


 
  
---
## Classification

* **Weak-to-strong 3d object detection with x-ray distillation**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/html/Gambashidze_Weak-to-Strong_3D_Object_Detection_with_X-Ray_Distillation_CVPR_2024_paper.html) [ :octocat: ](https://github.com/sakharok13/X-Ray-Teacher-Patching-Tools)


## Segmentation
* **CamPoint: Boosting Point Cloud Segmentation with Virtual Camera**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/html/Zhang_CamPoint_Boosting_Point_Cloud_Segmentation_with_Virtual_Camera_CVPR_2025_paper.html) [ :octocat: ](https://github.com/freekatz/CamPoint)

* **All in One: Visual-Description-Guided Unified Point Cloud Segmentation**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/html/Han_All_in_One_Visual-Description-Guided_Unified_Point_Cloud_Segmentation_ICCV_2025_paper.html) [ :octocat: ](https://github.com/Hanzy1996/VDG-Uni3DSeg)

* **Any3DIS: Class-Agnostic 3D Instance Segmentation by 2D Mask Tracking**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/html/Nguyen_Any3DIS_Class-Agnostic_3D_Instance_Segmentation_by_2D_Mask_Tracking_CVPR_2025_paper.html)

* **Insightful Instance Features for 3D Instance Segmentation**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/html/Roh_Insightful_Instance_Features_for_3D_Instance_Segmentation_CVPR_2025_paper.html) [ :octocat: ](https://github.com/kuai-lab/cvpr25_IKNE)

* **Relation3D: Enhancing Relation Modeling for Point Cloud Instance Segmentation**, CVPR 2025, [ :link: ](https://ieeexplore.ieee.org/abstract/document/11092675) [ :octocat: ](https://github.com/Howard-coder191/Relation3D)

* **PartField: Learning 3D Feature Fields for Part Segmentation and Beyond**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/html/Liu_PartField_Learning_3D_Feature_Fields_for_Part_Segmentation_and_Beyond_ICCV_2025_paper.html) [ :octocat: ](https://github.com/nv-tlabs/PartField)

* **3D Part Segmentation via Geometric Aggregation of 2D Visual Features**, WACV 2025, [ :link: ](https://ieeexplore.ieee.org/abstract/document/10943567) [ :octocat: ](https://github.com/marco-garosi/COPS)

* **Serialization based Point Cloud Oversegmentation**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/html/Lu_Serialization_based_Point_Cloud_Oversegmentation_ICCV_2025_paper.html) [ :octocat: ](https://github.com/CHL-glitch/SPCNet)

* **COB-GS: Clear Object Boundaries in 3DGS Segmentation Based on Boundary-Adaptive Gaussian Splitting**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/html/Zhang_COB-GS_Clear_Object_Boundaries_in_3DGS_Segmentation_Based_on_Boundary-Adaptive_CVPR_2025_paper.html) [ :octocat: ](https://github.com/ZestfulJX/COB-GS)

* **Generalized Few-shot 3D Point Cloud Segmentation with Vision-Language Model**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/html/An_Generalized_Few-shot_3D_Point_Cloud_Segmentation_with_Vision-Language_Model_CVPR_2025_paper.html) [ :octocat: ](https://github.com/ZhaochongAn/GFS-VL)

* **Functionality Understanding and Segmentation in 3D Scenes**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/html/Corsetti_Functionality_Understanding_and_Segmentation_in_3D_Scenes_CVPR_2025_paper.html) [ :octocat: ](https://github.com/tev-fbk/fun3du)

* **SAM2Object: Consolidating View Consistency via SAM2 for Zero-Shot 3D Instance Segmentation**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/html/Zhao_SAM2Object_Consolidating_View_Consistency_via_SAM2_for_Zero-Shot_3D_Instance_CVPR_2025_paper.html) [ :octocat: ](https://github.com/jihuaizhaohd/SAM2Object)

* **UniDxMD: Towards Unified Representation for Cross-Modal Unsupervised Domain Adaptation in 3D Semantic Segmentation**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/html/Liang_UniDxMD_Towards_Unified_Representation_for_Cross-Modal_Unsupervised_Domain_Adaptation_in_ICCV_2025_paper.html)

* **AiDe: Improving 3D Open-Vocabulary Semantic Segmentation by Aligned Vision-Language Learning**, WACV 2025, [ :link: ](https://ieeexplore.ieee.org/abstract/document/10943459)

* **Generalized Few-Shot Point Cloud Segmentation via LLM-Assisted Hyper-Relation Matching**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/html/Li_Generalized_Few-Shot_Point_Cloud_Segmentation_via_LLM-Assisted_Hyper-Relation_Matching_ICCV_2025_paper.html)

* **CACE: Sim-to-Real Indoor 3D Semantic Segmentation via Context-Aware Augmentation and Consistency Enforcement**, WACV 2025, [ :link: ](https://ieeexplore.ieee.org/abstract/document/10943913)

* **Sketchy Bounding-box Supervision for 3D Instance Segmentation**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/html/Deng_Sketchy_Bounding-box_Supervision_for_3D_Instance_Segmentation_CVPR_2025_paper.html) [ :octocat: ](https://github.com/dengq7/Sketchy-3DIS)

## Detection

### Data Representation
#### point-based
* **PointRCNN: 3D Object Proposal Generation and Detection from Point Cloud**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2019/papers/Shi_PointRCNN_3D_Object_Proposal_Generation_and_Detection_From_Point_Cloud_CVPR_2019_paper.pdf)  [ :octocat: ](https://github.com/sshaoshuai/PointRCNN)
* **Deep Hough Voting for 3D Object Detection in Point Clouds**, ICCV 2019, [ :link: ](https://openaccess.thecvf.com/content_ICCV_2019/papers/Qi_Deep_Hough_Voting_for_3D_Object_Detection_in_Point_Clouds_ICCV_2019_paper.pdf) [ :octocat: ](https://github.com/facebookresearch/votenet)
* **3DSSD: Point-based 3D Single Stage Object Detector**, CVPR 2020, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2020/papers/Yang_3DSSD_Point-Based_3D_Single_Stage_Object_Detector_CVPR_2020_paper.pdf) [ :octocat: ](https://github.com/JIA-Lab-research/3DSSD)
* **3Point-GNN: Graph Neural Network for 3D Object Detection in a Point Cloud**, CVPR 2020, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2020/papers/Shi_Point-GNN_Graph_Neural_Network_for_3D_Object_Detection_in_a_CVPR_2020_paper.pdf) [ :octocat: ](https://github.com/WeijingShi/Point-GNN)
* **From Points to Parts: 3D Object Detection from Point Cloud with Part-aware and Part-aggregation Network**, TPAMI 2020,[ :link: ](https://arxiv.org/abs/1907.03670) [ :octocat: ](https://github.com/sshaoshuai/PartA2-Net/blob/master/README.md)
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
* **PointPillars: Fast Encoders for Object Detection from Point Clouds**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2019/papers/Lang_PointPillars_Fast_Encoders_for_Object_Detection_From_Point_Clouds_CVPR_2019_paper.pdf) [ :octocat: ](https://github.com/nutonomy/second.pytorch) *(widely used impl.)*
* **PillarNet: Real-Time and High-Performance Pillar-based 3D Object Detection**, ECCV 2022, [ :link: ](https://arxiv.org/abs/2205.07403) [ :octocat: ](https://github.com/VISION-SJTU/PillarNet)
* **PillarNeXt: Rethinking Network Designs for 3D Object Detection in LiDAR Point Clouds**, CVPR 2023, [ :link: ](https://openaccess.thecvf.com/content/CVPR2023/html/Li_PillarNeXt_Rethinking_Network_Designs_for_3D_Object_Detection_in_LiDAR_Point_Clouds_CVPR_2023_paper.html) [ :octocat: ](https://github.com/qcraftai/pillarnext)
* **PillarHist: A Quantization-aware Pillar Feature Encoder based on Height-aware Histogram**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/html/Zhou_PillarHist_A_Quantization-aware_Pillar_Feature_Encoder_based_on_Height-aware_Histogram_CVPR_2025_paper.html) [ :octocat: ](https://github.com/open-mmlab/mmdetection3d) *(no official repo found)*
* **3DPillars: Pillar-based Two-stage 3D Object Detection**, ESWA 2025, [ :link: ](https://arxiv.org/abs/2509.05780) [ :octocat: ](https://github.com/open-mmlab/mmdetection3d) *(no official repo found)*

#### projection-based (BEV / range-view)
* **MV3D: Multi-View 3D Object Detection Network for Autonomous Driving**, CVPR 2017, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2017/papers/Chen_Multi-View_3D_Object_CVPR_2017_paper.pdf) [ :octocat: ](https://github.com/bostondiditeam/MV3D)
* **PIXOR: Real-time 3D Object Detection from Point Clouds**, CVPR 2018, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2018/papers/Yang_PIXOR_Real-Time_3D_CVPR_2018_paper.pdf) [ :octocat: ](https://github.com/philip-huang/PIXOR) *(re-impl.)*
* **AVOD: Joint 3D Proposal Generation and Object Detection from View Aggregation**, IROS 2018, [ :link: ](https://arxiv.org/abs/1712.02294) [ :octocat: ](https://github.com/kujason/avod)
* **LaserNet: An Efficient Probabilistic 3D Object Detector for Autonomous Driving**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2019/papers/Meyer_LaserNet_An_Efficient_Probabilistic_3D_Object_Detector_for_Autonomous_Driving_CVPR_2019_paper.pdf) [ :octocat: ](https://github.com/atyshka/Lasernet) *(re-impl.)*
* **RangeDet: In Defense of Range View for LiDAR-based 3D Object Detection**, ICCV 2021, [ :link: ](https://openaccess.thecvf.com/content/ICCV2021/papers/Fan_RangeDet_In_Defense_of_Range_View_for_LiDAR-Based_3D_Object_ICCV_2021_paper.pdf) [ :octocat: ](https://github.com/tusen-ai/RangeDet)
* **BEVFormer: Learning Bird’s-Eye-View Representation from Multi-Camera Videos**, ECCV 2022, [ :link: ](https://arxiv.org/abs/2203.17270) [ :octocat: ](https://github.com/fundamentalvision/BEVFormer)
* **BEVDepth: Acquisition of Reliable Depth for Multi-view 3D Object Detection**, AAAI 2023, [ :link: ](https://arxiv.org/abs/2206.10092) [ :octocat: ](https://github.com/Megvii-BaseDetection/BEVDepth)
* **SparseBEV: High-Performance Sparse 3D Object Detection from Multi-Camera Videos**, ICCV 2023, [ :link: ](https://openaccess.thecvf.com/content/ICCV2023/papers/Liu_SparseBEV_High-Performance_Sparse_3D_Object_Detection_from_Multi-Camera_Videos_ICCV_2023_paper.pdf) [ :octocat: ](https://github.com/MCG-NJU/SparseBEV)
* **BEVNeXt: Reviving Dense BEV Frameworks for 3D Object Detection**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Li_BEVNeXt_Reviving_Dense_BEV_Frameworks_for_3D_Object_Detection_CVPR_2024_paper.pdf) [ :octocat: ](https://github.com/woxihuanjiangguo/BEVNeXt)
* **CorrBEV: Multi-View 3D Object Detection by Correlation Learning with Multi-modal Prototypes**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/papers/Xue_CorrBEV_Multi-View_3D_Object_Detection_by_Correlation_Learning_with_Multi-modal_CVPR_2025_paper.pdf) [ :octocat: ](https://github.com/LLaVi-Lab) *(no official repo found)*
* **EVT: Efficient View Transformation for Multi-Modal 3D Object Detection**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/papers/Lee_EVT_Efficient_View_Transformation_for_Multi-Modal_3D_Object_Detection_ICCV_2025_paper.pdf) [ :octocat: ](https://github.com/open-mmlab/mmdetection3d) *(no official repo found)*
* **OpenM3D: Open-Vocabulary Multi-view Indoor 3D Object Detection without Human Annotations**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/papers/Hsu_OpenM3D_Open_Vocabulary_Multi-view_Indoor_3D_Object_Detection_without_Human_ICCV_2025_paper.pdf) [ :octocat: ](https://github.com/OpenM3D) *(org; code not clearly released for OpenM3D)*
* **What Matters in Range View 3D Object Detection**, CoRL 2024, [ :link: ](https://openreview.net/forum?id=EifoVoIyd5) [ :octocat: ](https://github.com/whatever50/range-view-3d-detection) *(if this repo is not the authors’, swap to your preferred re-impl.)*

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

### Anchor Strategy

### Sensor Modality

### Backbone Type

### Scene Type

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




## Tracking


## Compression
* **msLPCC: A multimodal-driven scalable framework for deep LiDAR point cloud compression**, AAAI 2024, [ :link: ]( https://ojs.aaai.org/index.php/AAAI/article/view/28362)


* **Pointsoup: High-performance and extremely low-decoding-latency learned geometry codec for large-scale point cloud scenes**, IJCAI 2024, [ :link: ](https://www.ijcai.org/proceedings/2024/0595.pdf) [ :octocat: ]( https://github.com/I2-Multimedia-Lab/Pointsoup)


* **Pdnet: parallel dual-branch network for point cloud geometry compression and analysis**, Data Compression Conference (DCC) 2024, [ :link: ](https://ieeexplore.ieee.org/document/10533742/)


* **Inter-frame compression for dynamic point cloud geometry coding**, IEEE Transactions on Image Processing 2024, [ :link: ](https://arxiv.org/pdf/2207.12554) [ :octocat: ](https://github.com/aniqueakhtar/PointCloudCompression)


* **Ecm-opcc: Efficient context model for octree-based point cloud compression**, ICASSP 2024, [ :link: ](https://ieeexplore.ieee.org/document/10446374/)



* **Point cloud compression with implicit neural representations: A unified framework**, ICCC 2024, [ :link: ](https://ieeexplore.ieee.org/iel8/10681633/10681675/10681880.pdf) [ :octocat: ](https://github.com/RhoHenning/INR-PCC)



* **Learned compression of point cloud geometry and attributes in a single model through multimodal rate-control**, Arxiv 2024, [ :link: ](https://arxiv.org/abs/2408.00599)



* **Roi-guided point cloud geometry compression towards human and machine vision**, ACM International Conference on Multimedia 2024, [ :link: ](https://dl.acm.org/doi/10.1145/3664647.3681301)



* **Lossless point cloud attribute compression using cross-scale, cross-group, and cross-color prediction**, Data Compression Conference (DCC) 2023, [ :link: ](https://ieeexplore.ieee.org/iel7/10125292/10125296/10125514.pdf)



* **YOGA: Yet another geometry-based point cloud compressor**, ACM International Conference on Multimedia 2023, [ :link: ](https://dl.acm.org/doi/10.1145/3581783.3613847) [ :octocat: ](https://github.com/3dpcc/YOGAv1)



* **Multiscale latent-guided entropy model for lidar point cloud compression**, IEEE Transactions on Circuits and Systems for Video Technology 2023, [ :link: ](https://ieeexplore.ieee.org/iel7/76/4358651/10129923.pdf)



* **Lossless point cloud geometry and attribute compression using a learned conditional probability model**, IEEE Transactions on Circuits and Systems for Video Technology 2023, [ :link: ](https://ieeexplore.ieee.org/iel7/76/10207864/10024999.pdf)



* **Efficient hierarchical entropy model for learned point cloud compression**, CVPR 2023, [ :link: ](https://openaccess.thecvf.com/content/CVPR2023/papers/,Song_Efficient_Hierarchical_Entropy_Model_for_Learned_Point_Cloud_Compression_CVPR_2023_paper.pdf)


* **GRASP-Net: Geometric residual analysis and synthesis for point cloud compression**, Proceedings of the 1st International Workshop on Advances in Point Cloud Compression, Processing and Analysis 2022, [ :link: ](https://arxiv.org/pdf/2209.04401.pdf) [ :octocat: ](https://github.com/InterDigitalInc/GRASP-Net)


* **Octattention: Octree-based large-scale contexts model for point cloud compression**, AAAI 2022, [ :link: ](https://cdn.aaai.org/ojs/19942/19942-13-23955-1-2-20220628.pdf) [ :octocat: ](https://github.com/zb12138/OctAttention)



* **4dac: Learning attribute compression for dynamic point clouds**, Arxiv 2022, [ :link: ](https://arxiv.org/pdf/2204.11723)



* **Point cloud compression with range image-based entropy model for autonomous driving**, ECCV 2022, [ :link: ](https://www.ecva.net/papers/eccv_2022/papers_ECCV/papers/136820315.pdf)



* **Rate-distortion modeling for bit rate constrained point cloud compression**, IEEE Transactions on Circuits and Systems for Video Technology 2022, [ :link: ](https://ieeexplore.ieee.org/document/9957096)



* **Sparse tensor-based point cloud attribute compression**, International Conference on Multimedia Information Processing and Retrieval (MIPR) 2022, [ :link: ](https://ieeexplore.ieee.org/document/9874468/)


* **Lossy point cloud geometry compression via end-to-end learning**, IEEE Transactions on Circuits and Systems for Video Technology 2021, [ :link: ](https://ieeexplore.ieee.org/document/9321375/)



* **Voxelcontext-net: An octree based framework for point cloud compression**, CVPR 2021, [ :link: ](https://openaccess.thecvf.com/content/CVPR2021/papers/Que_VoxelContext-Net_An_Octree_Based_Framework_for_Point_Cloud_Compression_CVPR_2021_paper.pdf)



* **Multiscale point cloud geometry compression**, Data Compression Conference (DCC) 2021, [ :link: ](https://ieeexplore.ieee.org/iel7/9418628/9418635/09418789.pdf) [ :octocat: ](https://github.com/NJUVISION/PCGCv2)



* **Deep compression for dense point cloud maps**,  IEEE Robotics and Automation Letters 2021, [ :link: ](https://ieeexplore.ieee.org/document/9354895/) [ :octocat: ](https://github.com/PRBonn/deep-point-map-compression)


* **Reduced reference perceptual quality model with application to rate control for video-based point cloud compression**, IEEE Transactions on Image Processing 2021, [ :link: ](https://ieeexplore.ieee.org/document/9490512)



* **Model-based joint bit allocation between geometry and color for video-based 3D point cloud compression**, IEEE Transactions on Multimedia 2020, [ :link: ](https://ieeexplore.ieee.org/document/9194311/) 


* **3d point cloud geometry compression on deep learning**, ACM International Conference on Multimedia 2019, [ :link: ](https://dl.acm.org/doi/10.1145/3343031.3351061)


* **Towards 6dof http adaptive streaming through point cloud compression**, ACM International Conference on Multimedia 2019, [ :link: ](https://dl.acm.org/doi/10.1145/3343031.3350917)


* **Learning convolutional transforms for lossy point cloud geometry compression**, IEEE international conference on image processing (ICIP) 2019, [ :link: ](https://arxiv.org/pdf/1903.08548) [ :octocat: ](https://github.com/mauriceqch/pcc_geo_cnn)


* **Graph-based motion estimation and compensation for dynamic 3D point cloud compression**, IEEE International Conference on Image Processing (ICIP) 2015, [ :link: ](https://ieeexplore.ieee.org/document/9194311/)


* **Point cloud attribute compression with graph transform**, IEEE International Conference on Image Processing (ICIP) 2014, [ :link: ](https://ieeexplore.ieee.org/document/7025414/)


* **Octree-based Point-Cloud Compression**, SPBG'06: Proceedings of the 3rd Eurographics / IEEE VGTC conference on Point-Based Graphics 2006, [ :link: ](https://dl.acm.org/doi/10.5555/2386388.2386404)

## Registration and 6D Pose estimation

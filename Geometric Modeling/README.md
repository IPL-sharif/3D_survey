# 3D Geometric Modeling

* [Generation](#Generation)

  *  [Unconditional generation](#unconditional)
  *  [Point cloud completion](#completion)
  *  [Weakly conditional generation](#weakly-conditional)

* [Reconstruction](#Reconstruction)

  *  [Traditional Reconstruction (SfM & MVS)](#traditional-reconstruction-sfm--mvs)
  *  [Implicit Reconstruction (NeRF and Neural Fields)](#implicit-reconstruction-nerf-and-neural-fields)
  *  [Explicit Reconstruction (3D Gaussian Splatting)](#explicit-reconstruction-3d-gaussian-splatting)
  *  [Surface Reconstruction](#surface-reconstruction)
---
## Generation
### Unconditional generation


### Point cloud completion

* **Domain adaptive point transformer for point cloud completion**, AAAI 2025, [ :link: ](https://arxiv.org/html/2412.19062v1) [ :octocat: ](https://github.com/Yinghui-Li-New/DAPoinTr)

* **DuInNet: Dual-Modality Feature Interaction for Point Cloud Completion**, IEEE Transactions on Multimedia 2025, [ :link: ](https://ieeexplore.ieee.org/iel8/6046/10844992/11153898.pdf) [ :octocat: ](https://github.com/xinpuliu/DuInNet)

* **PCDreamer: Point Cloud Completion Through Multi-view Diffusion Priors**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/papers/Wei_PCDreamer_Point_Cloud_Completion_Through_Multi-view_Diffusion_Priors_CVPR_2025_paper.pdf) [ :octocat: ](https://github.com/GSW-D/PCDreamerCode)


* **MAENet: Boost image-guided point cloud completion more accurate and even**, Information Fusion 2025, [ :link: ](https://www.sciencedirect.com/science/article/abs/pii/S1566253525002520) [ :octocat: ]( https://github.com/lmomoy/MAENet)


* **WalkFormer: Point Cloud Completion via Guided Walks**, WACV 2024, [ :link: ](https://openaccess.thecvf.com/content/WACV2024/papers/Zhang_WalkFormer_Point_Cloud_Completion_via_Guided_Walks_WACV_2024_paper.pdf)


* **Explicitly guided information interaction network for cross-modal point cloud completion**, ECCV 2024, [ :link: ](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/01946.pdf) [ :octocat: ](https://github.com/WHU-USI3DV/EGIInet)


* **Cross-modal learning for image-guided point cloud shape completion**, NeurIPS 2022, [ :link: ](https://papers.neurips.cc/paper_files/paper/2022/file/f2a11632520f4b7473d7838f074a7d25-Paper-Conference.pdf) [ :octocat: ](https://github.com/Yinghui-Li-New/DAPoinTr)


* **Seedformer: Patch seeds based point cloud completion with upsample transformer**, ECCV 2022, [ :link: ](https://www.ecva.net/papers/eccv_2022/papers_ECCV/papers/136630409.pdf) [ :octocat: ]( https://github.com/hrzhou2/seedformer)


* **View-guided point cloud completion**, CVPR 2021, [ :link: ](https://openaccess.thecvf.com/content/CVPR2021/papers/Zhang_View-Guided_Point_Cloud_Completion_CVPR_2021_paper.pdf) [ :octocat: ](https://github.com/Hydrogenion/ViPC)


* **Pointr: Diverse point cloud completion with geometry-aware transformers**, ICCV 2021, [ :link: ](https://openaccess.thecvf.com/content/ICCV2021/papers/Yu_PoinTr_Diverse_Point_Cloud_Completion_With_Geometry-Aware_Transformers_ICCV_2021_paper.pdf) [ :octocat: ](https://github.com/yuxumin/PoinTr)



* **Pf-net: Point fractal network for 3d point cloud completion**, CVPR 2020, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2020/papers/Huang_PF-Net_Point_Fractal_Network_for_3D_Point_Cloud_Completion_CVPR_2020_paper.pdf) [ :octocat: ](https://github.com/zztianzz/PF-Net-Point-Fractal-Network)


* **Rl-gan-net: A reinforcement learning agent controlled gan network for real-time point cloud shape completion**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2019/papers/Sarmad_RL-GAN-Net_A_Reinforcement_Learning_Agent_Controlled_GAN_Network_for_Real-Time_CVPR_2019_paper.pdf) [ :octocat: ](https://github.com/iSarmad/RL-GAN-Net)


* **Topnet: Structural point cloud decoder**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2019/papers/Tchapmi_TopNet_Structural_Point_Cloud_Decoder_CVPR_2019_paper.pdf) [ :octocat: ](http://completion3d.stanford.edu)


* **PU-Net: Point Cloud Upsampling Network**, CVPR 2018, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2018/papers/Yu_PU-Net_Point_Cloud_CVPR_2018_paper.pdf) [ :octocat: ](https://github.com/yulequan/PU-Net)


* **A Papier-Mˆach ́e Approach to Learning 3D Surface Generation**, CVPR 2018, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2018/papers/Groueix_A_Papier-Mache_Approach_CVPR_2018_paper.pdf) [ :octocat: ](https://github.com/ThibaultGROUEIX/AtlasNet)


* **Foldingnet: Point cloud auto-encoder via deep grid deformation**, CVPR 2018, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2018/papers/Yang_FoldingNet_Point_Cloud_CVPR_2018_paper.pdf) [ :octocat: ](https://github.com/qinglew/FoldingNet)


* **PCN: Point Completion Network**, International conference on 3D vision (3DV) 2018, [ :link: ](https://arxiv.org/pdf/1808.00671) [ :octocat: ]( https://wentaoyuan.github.io/pcn)


### Weakly conditional generation



## Reconstruction

### Survey Papers

* **A Survey of 3D Reconstruction: The Evolution from Multi-View Geometry to NeRF and 3DGS**, Sensors 2025, [ :link: ](https://doi.org/10.3390/s25185748)
* **A survey on surface reconstruction based on 3D Gaussian splatting**, PeerJ Computer Science 2025, [ :link: ](https://doi.org/10.7717/peerj-cs.3034)
* **Deep-learning-based 3-d surface reconstruction—a survey**, Proceedings of the IEEE 2023, [ :link: ](https://ieeexplore.ieee.org/document/10301359)

### Traditional Reconstruction (SfM & MVS)

* **Building Rome in a Day**, Commun. ACM 2011, [ :link: ](https://dl.acm.org/doi/10.1145/2001269.2001293)
* **Discrete-continuous optimization for large-scale structure from motion**, CVPR 2011, [ :link: ](https://ieeexplore.ieee.org/document/5995626)
* **Very large-scale global sfm by distributed motion averaging**, CVPR 2018, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2018/papers/Zhu_Very_Large-Scale_Global_CVPR_2018_paper.pdf)
* **Global fusion of relative motions for robust, accurate and scalable structure from motion**, ICCV 2013, [ :link: ](https://www.cv-foundation.org/openaccess/content_iccv_2013/papers/Moulon_Global_Fusion_of_2013_ICCV_paper.pdf)
* **Modeling and recognition of landmark image collections using iconic scene graphs**, ECCV 2008, [ :link: ](https://link.springer.com/chapter/10.1007/978-3-540-88682-2_33)
* **Towards linear-time incremental structure from motion**, 3DV 2013, [ :link: ](https://dl.acm.org/doi/10.1109/3DV.2013.25)
* **Modeling the world from internet photo collections**, IJCV 2008, [ :link: ](https://link.springer.com/article/10.1007/s11263-007-0107-3)
* **Structure-from-motion revisited**, CVPR 2016, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2016/papers/Schonberger_Structure-From-Motion_Revisited_CVPR_2016_paper.pdf) [ :octocat: ](https://github.com/colmap/colmap)
* **Multi-view stereo for community photo collections**, ICCV 2007, [ :link: ](https://www.computer.org/csdl/proceedings-article/iccv/2007/04408933/12OmNyeECCL)
* **Pixelwise view selection for unstructured multi-view stereo**, ECCV 2016, [ :link: ](https://link.springer.com/chapter/10.1007/978-3-319-46487-9_31)
* **Massively parallel multiview stereopsis by surface normal diffusion**, ICCV 2015, [ :link: ](https://www.cv-foundation.org/openaccess/content_iccv_2015/papers/Galliani_Massively_Parallel_Multiview_ICCV_2015_paper.pdf)
* **Cascade cost volume for high-resolution multi-view stereo and stereo matching**, CVPR 2020, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2020/papers/Gu_Cascade_Cost_Volume_for_High-Resolution_Multi-View_Stereo_and_Stereo_Matching_CVPR_2020_paper.pdf) [ :octocat: ](https://github.com/alibaba/cascade-mvsnet)
* **Fast-mvsnet: Sparse-to-dense multi-view stereo with learned propagation and gauss-newton refinement**, CVPR 2020, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2020/papers/Yu_Fast-MVSNet_Sparse-to-Dense_Multi-View_Stereo_With_Learned_Propagation_and_Gauss-Newton_Refinement_CVPR_2020_paper.pdf)
* **Efficient multi-view stereo by iterative dynamic cost volume**, CVPR 2022, [ :link: ](https://openaccess.thecvf.com/content/CVPR2022/papers/Wang_Efficient_Multi-View_Stereo_by_Iterative_Dynamic_Cost_Volume_CVPR_2022_paper.pdf)
* **Mvsnet: Depth inference for unstructured multi-view stereo**, ECCV 2018, [ :link: ](https://openaccess.thecvf.com/content_ECCV_2018/papers/Yao_Yao_MVSNet_Depth_Inference_ECCV_2018_paper.pdf) [ :octocat: ](https://github.com/YoYo000/MVSNet)
* **Recurrent mvsnet for high-resolution multi-view stereo depth inference**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2019/papers/Yao_Recurrent_MVSNet_for_High-Resolution_Multi-View_Stereo_Depth_Inference_CVPR_2019_paper.pdf) [ :octocat: ](https://github.com/yoyo000/recurrent-mvsnet)
* **Vis-mvsnet: Visibility-aware multi-view stereo network**, IJCV 2023, [ :link: ](https://www.springerprofessional.de/en/vis-mvsnet-visibility-aware-multi-view-stereo-network/23607004)

### Implicit Reconstruction (NeRF and Neural Fields)

* **Ibrnet: Learning multi-view image-based rendering**, CVPR 2021, [ :link: ](https://openaccess.thecvf.com/content/CVPR2021/papers/Wang_IBRNet_Learning_Multi-View_Image-Based_Rendering_CVPR_2021_paper.pdf) [ :octocat: ](https://github.com/googleinterns/IBRNet)
* **Nerf: Representing scenes as neural radiance fields for view synthesis**, Commun. ACM 2021, [ :link: ](https://dl.acm.org/doi/10.1145/3503250) [ :octocat: ](https://github.com/bmild/nerf)
* **pixelnerf: Neural radiance fields from one or few images**, CVPR 2021, [ :link: ](https://openaccess.thecvf.com/content/CVPR2021/papers/Yu_pixelNeRF_Neural_Radiance_Fields_From_One_or_Few_Images_CVPR_2021_paper.pdf) [ :octocat: ](https://github.com/sxyu/pixel-nerf)
* **D-nerf: Neural radiance fields for dynamic scenes**, CVPR 2021, [ :link: ](https://openaccess.thecvf.com/content/CVPR2021/papers/Pumarola_D-NeRF_Neural_Radiance_Fields_for_Dynamic_Scenes_CVPR_2021_paper.pdf) [ :octocat: ](https://github.com/albertpumarola/D-NeRF)
* **E-nerf: Neural radiance fields from a moving event camera**, IEEE RAL 2023, [ :link: ](https://ieeexplore.ieee.org/document/10028738)
* **Neural scene flow fields for space-time view synthesis of dynamic scenes**, CVPR 2021, [ :link: ](https://openaccess.thecvf.com/content/CVPR2021/papers/Li_Neural_Scene_Flow_Fields_for_Space-Time_View_Synthesis_of_Dynamic_CVPR_2021_paper.pdf) [ :octocat: ](https://github.com/google/nsff)
* **Nerfplayer: A streamable dynamic scene representation with decomposed neural radiance fields**, IEEE TVCG 2023, [ :link: ](https://dl.acm.org/doi/10.1109/TVCG.2023.3247082)
* **Nerfies: Deformable neural radiance fields**, ICCV 2021, [ :link: ](https://openaccess.thecvf.com/content/ICCV2021/papers/Park_Nerfies_Deformable_Neural_Radiance_Fields_ICCV_2021_paper.pdf) [ :octocat: ](https://github.com/google/nerfies)
* **Tensor4d: Efficient neural 4d decomposition for high-fidelity dynamic reconstruction and rendering**, CVPR 2023, [ :link: ](https://openaccess.thecvf.com/content/CVPR2023/papers/Shao_Tensor4D_Efficient_Neural_4D_Decomposition_for_High-Fidelity_Dynamic_Reconstruction_and_CVPR_2023_paper.pdf)
* **Baking neural radiance fields for real-time view synthesis**, ICCV 2021, [ :link: ](https://openaccess.thecvf.com/content/ICCV2021/papers/Hedman_Baking_Neural_Radiance_Fields_for_Real-Time_View_Synthesis_ICCV_2021_paper.pdf) [ :octocat: ](https://github.com/google/baking-nerf)
* **Instant neural graphics primitives with a multiresolution hash encoding**, ACM Trans. Graph. 2022, [ :link: ](https://dl.acm.org/doi/10.1145/3528223.3530127) [ :octocat: ](https://github.com/NVlabs/instant-ngp)
* **Lightning nerf: Efficient hybrid scene representation for autonomous driving**, ICRA 2024, [ :link: ](https://arxiv.org/abs/2403.05907)
* **Neural sparse voxel fields**, NeurIPS 2020, [ :link: ](https://proceedings.neurips.cc/paper/2020/hash/b4b758962f17808746e9bb832a6fa4b8-Abstract.html) [ :octocat: ](https://github.com/facebookresearch/NSVF)
* **Nerfacc: Efficient sampling accelerates nerfs**, ICCV 2023, [ :link: ](https://openaccess.thecvf.com/content/ICCV2023/papers/Li_NerfAcc_Efficient_Sampling_Accelerates_NeRFs_ICCV_2023_paper.pdf) [ :octocat: ](https://github.com/KAIR-BAIR/nerfacc)
* **Recursive-nerf: An efficient and dynamically growing nerf**, IEEE TVCG 2022, [ :link: ](https://dl.acm.org/doi/10.1109/TVCG.2022.3204608)
* **Tensorf: Tensorial radiance fields**, ECCV 2022, [ :link: ](https://link.springer.com/chapter/10.1007/978-3-031-19824-3_20) [ :octocat: ](https://github.com/apchenstu/TensoRF)
* **Zip-nerf: Anti-aliased grid-based neural radiance fields**, ICCV 2023, [ :link: ](https://openaccess.thecvf.com/content/ICCV2023/papers/Barron_Zip-NeRF_Anti-Aliased_Grid-Based_Neural_Radiance_Fields_ICCV_2023_paper.pdf)
* **Bad-nerf: Bundle adjusted deblur neural radiance fields**, CVPR 2023, [ :link: ](https://openaccess.thecvf.com/content/CVPR2023/papers/Wang_BAD-NeRF_Bundle_Adjusted_Deblur_Neural_Radiance_Fields_CVPR_2023_paper.pdf)
* **Mip-nerf: A multiscale representation for anti-aliasing neural radiance fields**, ICCV 2021, [ :link: ](https://openaccess.thecvf.com/content/ICCV2021/papers/Barron_Mip-NeRF_A_Multiscale_Representation_for_Anti-Aliasing_Neural_Radiance_Fields_ICCV_2021_paper.pdf) [ :octocat: ](https://github.com/google/mipnerf)
* **Nerf++: Analyzing and improving neural radiance fields**, arXiv 2020, [ :link: ](https://arxiv.org/abs/2010.07492) [ :octocat: ](https://github.com/Kai-46/nerfplusplus)
* **Nerf in the wild: Neural radiance fields for unconstrained photo collections**, CVPR 2021, [ :link: ](https://openaccess.thecvf.com/content/CVPR2021/papers/Martin-Brualla_NeRF_in_the_Wild_Neural_Radiance_Fields_for_Unconstrained_Photo_CVPR_2021_paper.pdf) [ :octocat: ](https://github.com/cretaw/nerf-w)
* **Nerflix: High-quality neural view synthesis by learning a degradation-driven inter-viewpoint mixer**, CVPR 2023, [ :link: ](https://arxiv.org/abs/2303.06919)
* **Uhdnerf: Ultra-high-definition neural radiance fields**, ICCV 2023, [ :link: ](https://openaccess.thecvf.com/content/ICCV2023/papers/Li_UHDNeRF_Ultra-High-Definition_Neural_Radiance_Fields_ICCV_2023_paper.pdf)
* **Flipnerf: Flipped reflection rays for few-shot novel view synthesis**, ICCV 2023, [ :link: ](https://openaccess.thecvf.com/content/ICCV2023/papers/Seo_FlipNeRF_Flipped_Reflection_Rays_for_Few-shot_Novel_View_Synthesis_ICCV_2023_paper.pdf)
* **Freenerf: Improving few-shot neural rendering with free frequency regularization**, CVPR 2023, [ :link: ](https://openaccess.thecvf.com/content/CVPR2023/papers/Yang_FreeNeRF_Improving_Few-Shot_Neural_Rendering_With_Free_Frequency_Regularization_CVPR_2023_paper.pdf)
* **Hg3-nerf: Hierarchical geometric, semantic, and photometric guided neural radiance fields for sparse view inputs**, arXiv 2024, [ :link: ](https://arxiv.org/abs/2401.11711)
* **Mixnerf: Modeling a ray with mixture density for novel view synthesis from sparse inputs**, CVPR 2023, [ :link: ](https://openaccess.thecvf.com/content/CVPR2023/papers/Seo_MixNeRF_Modeling_a_Ray_With_Mixture_Density_for_Novel_View_CVPR_2023_paper.pdf)

### Explicit Reconstruction (3D Gaussian Splatting)

* **Drivinggaussian: Composite gaussian splatting for surrounding dynamic autonomous driving scenes**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Zhou_DrivingGaussian_Composite_Gaussian_Splatting_for_Surrounding_Dynamic_Autonomous_Driving_Scenes_CVPR_2024_paper.pdf)
* **Gs-slam: Dense visual slam with 3d gaussian splatting**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Yan_GS-SLAM_Dense_Visual_SLAM_with_3D_Gaussian_Splatting_CVPR_2024_paper.pdf)
* **Ig-slam: Instant gaussian slam**, arXiv 2024, [ :link: ](https://arxiv.org/abs/2408.01126)
* **pixelsplat: 3d gaussian splats from image pairs for scalable generalizable 3d reconstruction**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Charatan_pixelSplat_3D_Gaussian_Splats_from_Image_Pairs_for_Scalable_Generalizable_CVPR_2024_paper.pdf) [ :octocat: ](https://github.com/dcharatan/pixelsplat)
* **Vastgaussian: Vast 3d gaussians for large scene reconstruction**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Lin_VastGaussian_Vast_3D_Gaussians_for_Large_Scene_Reconstruction_CVPR_2024_paper.pdf)
* **3D Gaussian splatting for real-time radiance field rendering**, ACM Trans. Graph. 2023, [ :link: ](https://dl.acm.org/doi/10.1145/3592433) [ :octocat: ](https://github.com/graphdeco-inria/gaussian-splatting)
* **Depthsplat: Connecting gaussian splatting and depth**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/papers/Xu_DepthSplat_Connecting_Gaussian_Splatting_and_Depth_CVPR_2025_paper.pdf)
* **4d gaussian splatting for real-time dynamic scene rendering**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Wu_4D_Gaussian_Splatting_for_Real-Time_Dynamic_Scene_Rendering_CVPR_2024_paper.pdf)
* **Dn-4dgs: Denoised deformable network with temporal-spatial aggregation for dynamic scene rendering**, NeurIPS 2024, [ :link: ](https://proceedings.neurips.cc/paper_files/paper/2024/hash/35b2c1d2b0c5e5f4c6e7d8a9b0c1d2e3-Abstract.html)
* **Deformable 3d gaussians for high-fidelity monocular dynamic scene reconstruction**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Yang_Deformable_3D_Gaussians_for_High-Fidelity_Monocular_Dynamic_Scene_Reconstruction_CVPR_2024_paper.pdf)
* **Gaussian-flow: 4d reconstruction with dynamic 3d gaussian particle**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Lin_Gaussian-Flow_4D_Reconstruction_with_Dynamic_3D_Gaussian_Particle_CVPR_2024_paper.pdf)
* **V4d: Voxel for 4d novel view synthesis**, IEEE TVCG 2023, [ :link: ](https://dl.acm.org/doi/abs/10.1109/TVCG.2023.3312127)
* **Compgs: Smaller and faster gaussian splatting with vector quantization**, ECCV 2024, [ :link: ](https://dl.acm.org/doi/10.1007/978-3-031-73411-3_19)
* **Distwar: Fast differentiable rendering on raster-based rendering pipelines**, arXiv 2023, [ :link: ](https://arxiv.org/abs/2401.05345)
* **Eagles: Efficient accelerated 3d gaussians with lightweight encodings**, ECCV 2024, [ :link: ](https://dl.acm.org/doi/10.1007/978-3-031-73036-8_4)
* **Lightgaussian: Unbounded 3d gaussian compression with 15x reduction and 200+ fps**, NeurIPS 2024, [ :link: ](https://proceedings.neurips.cc/paper_files/paper/2024/hash/fd881d3b625437354d4421818f81058f-Abstract-Conference.html)
* **Sugar: Surface-aligned gaussian splatting for efficient 3d mesh reconstruction and high-quality mesh rendering**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Guedon_SuGaR_Surface-Aligned_Gaussian_Splatting_for_Efficient_3D_Mesh_Reconstruction_and_CVPR_2024_paper.pdf)
* **Letsgo: Large-scale garage modeling and rendering via lidar-assisted gaussian primitives**, ACM Trans. Graph. 2024, [ :link: ](https://dl.acm.org/doi/10.1145/3687908)
* **Li-gs: Gaussian splatting with lidar incorporated for accurate large-scale reconstruction**, IEEE RAL 2024, [ :link: ](https://arxiv.org/abs/2409.12899)
* **Lidarf: Delving into lidar for neural radiance field on street scenes**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Sun_LidaRF_Delving_into_Lidar_for_Neural_Radiance_Field_on_Street_CVPR_2024_paper.pdf)
* **Gaussianpro: 3d gaussian splatting with progressive propagation**, ICML 2024, [ :link: ](https://dl.acm.org/doi/abs/10.5555/3692070.3692390)
* **Multi-scale 3d gaussian splatting for anti-aliased rendering**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Yan_Multi-Scale_3D_Gaussian_Splatting_for_Anti-Aliased_Rendering_CVPR_2024_paper.pdf)
* **Mip-splatting: Alias-free 3d gaussian splatting**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Yu_Mip-Splatting_Alias-free_3D_Gaussian_Splatting_CVPR_2024_paper.pdf)
* **Scaffold-gs: Structured 3d gaussians for view-adaptive rendering**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Lu_Scaffold-GS_Structured_3D_Gaussians_for_View-Adaptive_Rendering_CVPR_2024_paper.pdf)
* **Supergs: Super-resolution 3d gaussian splatting via latent feature field and gradient-guided splitting**, arXiv 2024, [ :link: ](https://arxiv.org/abs/2410.02571)
* **Fsgs: Real-time few-shot view synthesis using gaussian splatting**, ECCV 2024, [ :link: ](https://dl.acm.org/doi/10.1007/978-3-031-72933-1_9)
* **Lm-gaussian: Boost sparse-view 3d gaussian splatting with large model priors**, arXiv 2024, [ :link: ](https://arxiv.org/abs/2409.03456)
* **Mcgs: Multiview consistency enhancement for sparse-view 3d gaussian radiance fields**, IEEE TPAMI 2025, [ :link: ](https://arxiv.org/abs/2410.11394)
* **SparseGS: Real-time 360 sparse view synthesis using Gaussian splatting**, 2024 (Thesis), [ :link: ](https://arxiv.org/abs/2312.00206)

### Surface Reconstruction

* **Dynamic Gaussians Mesh: Consistent Mesh Reconstruction from Dynamic Scenes**, arXiv 2024, [ :link: ](https://arxiv.org/abs/2404.12379)
* **GSDeformer: Direct Cage-based Deformation for 3D Gaussian Splatting**, arXiv 2024, [ :link: ](https://arxiv.org/abs/2405.15491)
* **Mags: Reconstructing and simulating dynamic 3d objects with mesh-adsorbed gaussian splatting**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/papers/Ma_MaGS_Reconstructing_and_Simulating_Dynamic_3D_Objects_with_Mesh-adsorbed_Gaussian_ICCV_2025_paper.pdf)
* **Sa-gs: Semantic-aware gaussian splatting for large scene reconstruction with geometry constrain**, arXiv 2024, [ :link: ](https://arxiv.org/abs/2405.16923)
* **Sc-gs: Sparse-controlled gaussian splatting for editable dynamic scenes**, CVPR 2024, [ :link: ](https://openaccess.thecvf.com/content/CVPR2024/papers/Huang_SC-GS_Sparse-Controlled_Gaussian_Splatting_for_Editable_Dynamic_Scenes_CVPR_2024_paper.pdf)
* **3dgsr: Implicit surface reconstruction with 3d gaussian splatting**, ACM Trans. Graph. 2024, [ :link: ](https://arxiv.org/pdf/2404.00409?)
* **Gaussian opacity fields: Efficient adaptive surface reconstruction in unbounded scenes**, ACM Trans. Graph. 2024, [ :link: ](https://dl.acm.org/doi/10.1145/3687937)
* **Gsdf: 3dgs meets sdf for improved neural rendering and reconstruction**, NeurIPS 2024, [ :link: ](https://proceedings.neurips.cc/paper_files/paper/2024/hash/ea13534ee239bb3977795b8cc855bacc-Abstract-Conference.html)
* **Neusg: Neural implicit surface reconstruction with 3d gaussian splatting guidance**, arXiv 2023, [ :link: ](https://arxiv.org/abs/2312.00846)
* **GS-Octree: Octree-based 3D Gaussian Splatting for Robust Object-level 3D Reconstruction Under Strong Lighting**, Computer Graphics Forum 2024, [ :link: ](https://onlinelibrary.wiley.com/doi/10.1111/cgf.15206)
* **2d gaussian splatting for geometrically accurate radiance fields**, ACM SIGGRAPH 2024, [ :link: ](https://dl.acm.org/doi/10.1145/3641519.3657428)
* **Mani-gs: Gaussian splatting manipulation with triangular mesh**, CVPR 2025, [ :link: ](https://openaccess.thecvf.com/content/CVPR2025/papers/Gao_Mani-GS_Gaussian_Splatting_Manipulation_with_Triangular_Mesh_CVPR_2025_paper.pdf)
* **Quadratic Gaussian Splatting for Efficient and Detailed Surface Reconstruction**, arXiv 2024, [ :link: ](https://arxiv.org/abs/2411.16392)
* **RoGs: Large Scale Road Surface Reconstruction with Meshgrid Gaussian**, arXiv 2024, [ :link: ](https://arxiv.org/abs/2405.14342)
* **Tetsphere splatting: Representing high-quality geometry with lagrangian volumetric meshes**, arXiv 2024, [ :link: ](https://arxiv.org/abs/2405.20283)
* **Gs2mesh: Surface reconstruction from gaussian splatting via novel stereo views**, ECCV 2024, [ :link: ](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/12486.pdf)
* **Surface reconstruction from 3d gaussian splatting via local structural hints**, ECCV 2024, [ :link: ](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/00274.pdf)
* **Gaustudio: A modular framework for 3d gaussian splatting and beyond**, arXiv 2024, [ :link: ](https://arxiv.org/abs/2403.19632) [ :octocat: ](https://github.com/GAP-LAB-CUHK-SZ/gaustudio)
* **OMEGAS: Object Mesh Extraction from Large Scenes Guided by Gaussian Segmentation**, IEEE TCSVT 2025, [ :link: ](https://ieeexplore.ieee.org/document/11072471)
* **Rade-gs: Rasterizing depth in gaussian splatting**, arXiv 2024, [ :link: ](https://arxiv.org/abs/2406.01467)
* **Quadratic Gaussian Splatting: High Quality Surface Reconstruction with Second-order Geometric Primitives**, ICCV 2025, [ :link: ](https://openaccess.thecvf.com/content/ICCV2025/papers/Zhang_Quadratic_Gaussian_Splatting_High_Quality_Surface_Reconstruction_with_Second-order_Geometric_ICCV_2025_paper.pdf)
* **Trim 3d gaussian splatting for accurate geometry representation**, arXiv 2024, [ :link: ](https://arxiv.org/abs/2406.07499)
* **Differentiable volumetric rendering: Learning implicit 3d representations without 3d supervision**, CVPR 2020, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2020/papers/Niemeyer_Differentiable_Volumetric_Rendering_Learning_Implicit_3D_Representations_Without_3D_Supervision_CVPR_2020_paper.pdf) [ :octocat: ](https://github.com/autonomousvision/differentiable_volumetric_rendering)
* **DeepSDF: Learning continuous signed distance functions for shape representation**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2019/papers/Park_DeepSDF_Learning_Continuous_Signed_Distance_Functions_for_Shape_Representation_CVPR_2019_paper.pdf) [ :octocat: ](https://github.com/facebookresearch/DeepSDF)
* **Learning implicit fields for generative shape modeling**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2019/papers/Chen_Learning_Implicit_Fields_for_Generative_Shape_Modeling_CVPR_2019_paper.pdf)
* **Occupancy networks: Learning 3d reconstruction in function space**, CVPR 2019, [ :link: ](https://openaccess.thecvf.com/content_CVPR_2019/papers/Mescheder_Occupancy_Networks_Learning_3D_Reconstruction_in_Function_Space_CVPR_2019_paper.pdf) [ :octocat: ](https://github.com/autonomousvision/occupancy_networks)
* **A papier-mâché approach to learning 3d surface generation**, CVPR 2018, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2018/papers/Groueix_A_Papier-Mache_Approach_CVPR_2018_paper.pdf) [ :octocat: ](https://github.com/ThibaultGROUEIX/AtlasNet)
* **Mesh r-cnn**, ICCV 2019, [ :link: ](https://openaccess.thecvf.com/content_ICCV_2019/papers/Gkioxari_Mesh_R-CNN_ICCV_2019_paper.pdf) [ :octocat: ](https://github.com/facebookresearch/meshrcnn)
* **Pixel2mesh: Generating 3d mesh models from single rgb images**, ECCV 2018, [ :link: ](https://openaccess.thecvf.com/content_ECCV_2018/papers/Nanyang_Wang_Pixel2Mesh_Generating_3D_ECCV_2018_paper.pdf) [ :octocat: ](https://github.com/nywang16/Pixel2Mesh)
* **Poisson surface reconstruction**, Eurographics Symposium on Geometry Processing 2006, [ :link: ](https://dl.acm.org/doi/10.2312/SGP/SGP06/061-070)
* **Foldingnet: Point cloud auto-encoder via deep grid deformation**, CVPR 2018, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2018/papers/Yang_FoldingNet_Point_Cloud_CVPR_2018_paper.pdf)
* **Pcn: Point completion network**, 3DV 2018, [ :link: ](https://arxiv.org/abs/1808.00671)
* **A point set generation network for 3d object reconstruction from a single image**, CVPR 2017, [ :link: ](https://openaccess.thecvf.com/content_cvpr_2017/papers/Fan_A_Point_Set_CVPR_2017_paper.pdf)
* **Kinectfusion: Real-time dense surface mapping and tracking**, ISMAR 2011, [ :link: ](https://dl.acm.org/doi/10.1109/ISMAR.2011.6092378)
* **The ball-pivoting algorithm for surface reconstruction**, IEEE TVCG 1999, [ :link: ](http://mesh.brown.edu/taubin/pdfs/bernardini-etal-tvcg99.pdf)
* **Three-dimensional reconstruction of complex shapes based on the Delaunay triangulation**, SPIE 1993, [ :link: ](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/1905/0000/Three-dimensional-reconstruction-of-complex-shapes-based-on-the-Delaunay/10.1117/12.148710.full)
* **Voronoi diagrams and Delaunay triangulations**, Handbook of Discrete and Computational Geometry 2017, [ :link: ](https://www.csun.edu/~ctoth/Handbook/chap27.pdf)

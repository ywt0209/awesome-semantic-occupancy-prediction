# Semantic Occupancy Prediction — Paper Survey (2026)

**Scope:** Semantic Occupancy Prediction / Semantic Scene Completion / Semantic Occupancy Forecasting / Panoptic Occupancy Benchmark.  
**Excluded:** Papers where occupancy is only an auxiliary signal for 3D detection or planning.  
**Conferences covered:** 3DV 2026, WACV 2026, AAAI 2026, ICLR 2026, CVPR 2026  
**Total:** 20 papers

---

## Quick-Reference Comparison Table

| # | Paper | Venue | Input Modality | Core Method | Task | Scene | arXiv / Link |
|---|-------|-------|---------------|-------------|------|-------|-------------|
| 1 | ForecastOcc | 3DV 2026 | Camera | — | Occ Forecasting | AD | [2602.08006](https://arxiv.org/abs/2602.08006) |
| 2 | SGFormer | 3DV 2026 | Satellite + Ground Camera | Transformer | SSC | General | [2503.16825](https://arxiv.org/abs/2503.16825) |
| 3 | One Step Closer | 3DV 2026 | Monocular Camera | Future-frame synthesis | SSC | AD | [2507.13801](https://arxiv.org/abs/2507.13801) |
| 4 | FairScene | WACV 2026 | Camera | Disentangled 2D/3D repr. | SSC | AD | [CVF PDF](https://openaccess.thecvf.com/content/WACV2026/papers/Jia_FairScene_Learning_Class-Disentangled_2D3D_Representations_for_Semantic_Scene_Completion_WACV_2026_paper.pdf) |
| 5 | Vision-Only GS Collab. | AAAI 2026 | Camera (multi-agent) | Gaussian Splatting | Occ Prediction | AD | [2508.10936](https://arxiv.org/abs/2508.10936) |
| 6 | SPSC | AAAI 2026 | Camera + LiDAR | Sparse | Occ Prediction | AD | [AAAI vol.40 no.6](https://ojs.aaai.org/index.php/AAAI/issue/view/733) |
| 7 | HD²-SSC | AAAI 2026 | Camera | High-dim dense repr. | SSC | AD | [2511.07925](https://arxiv.org/abs/2511.07925) |
| 8 | 3D Object-Centric SSC | AAAI 2026 | Camera | Object-centric features | SSC | AD | [2511.13031](https://arxiv.org/abs/2511.13031) |
| 9 | Temporal Fusion Beyond FoV | AAAI 2026 | Camera | Temporal fusion | SSC | AD | [2511.12498](https://arxiv.org/abs/2511.12498) |
| 10 | SplatSSC | AAAI 2026 | Camera | Gaussian Splatting + depth | SSC | AD | [2508.02261](https://arxiv.org/abs/2508.02261) |
| 11 | PG-Occ (Prog. Gaussian Transformer) | ICLR 2026 | Camera | Gaussian + Transformer | Open-vocab Occ | AD | [OpenReview](https://openreview.net/forum?id=mHFaflQv93) |
| 12 | G²-Occ | ICLR 2026 | Camera | Geometry-guided Gaussian | Occ Prediction | Embodied | [OpenReview](https://openreview.net/forum?id=uw9MfZJmlb) |
| 13 | S2GO | ICLR 2026 | Camera | Sparse Gaussian, streaming | Occ Prediction | AD | [OpenReview](https://openreview.net/forum?id=z8ggdMlSco) |
| 14 | Dr.Occ | CVPR 2026 | Surround Camera | Depth + Region guidance | Occ Prediction | AD | [2603.01007](https://arxiv.org/abs/2603.01007) |
| 15 | OccAny | CVPR 2026 | Camera | — | Occ Prediction | AD / General | [2603.23502](https://arxiv.org/abs/2603.23502) |
| 16 | VG3S | CVPR 2026 | Camera | Visual Geometry + Gaussian | Occ Prediction | AD | [2603.06210](https://arxiv.org/abs/2603.06210) |
| 17 | Can We Trust Unreliable Voxels? | CVPR 2026 | Camera | Label-noise robustness | SSC | AD | [2603.06279](https://arxiv.org/abs/2603.06279) |
| 18 | L2COcc | CVPR 2026 | Camera (LiDAR distillation) | Knowledge distillation | SSC | AD | [2503.12369](https://arxiv.org/abs/2503.12369) |
| 19 | OccuFly | CVPR 2026 | Aerial Camera | — | Benchmark (SSC) | Aerial | [2512.20770](https://arxiv.org/abs/2512.20770) |
| 20 | Instance-Centric Panoptic Occ | CVPR 2026 | Camera | Instance-centric | Benchmark (Panoptic) | AD | [2603.27238](https://arxiv.org/abs/2603.27238) |

---

## Papers by Conference

### 3DV 2026

#### ForecastOcc: Vision-based Semantic Occupancy Forecasting
- **Authors:** Mohan, Riya; Hurtado, Juana Valeria; Mohan, Rohit; Valada, Abhinav
- **Tags:** `camera` `forecasting` `autonomous-driving`
- **arXiv:** https://arxiv.org/abs/2602.08006

#### SGFormer: Satellite-Ground Fusion for 3D Semantic Scene Completion
- **Authors:** Guo, Xiyue; Hu, Jiarui; Hu, Junjie; Bao, Hujun; Zhang, Guofeng
- **Tags:** `satellite` `ground-camera` `multi-modal` `transformer` `SSC`
- **arXiv:** https://arxiv.org/abs/2503.16825

#### One Step Closer: Creating the Future to Boost Monocular Semantic Scene Completion
- **Authors:** Lu, Haoang; Su, Yuanqi; Zhang, Xiaoning; Hu, Hao
- **Tags:** `monocular-camera` `future-frame-synthesis` `SSC` `autonomous-driving`
- **arXiv:** https://arxiv.org/abs/2507.13801

---

### WACV 2026

#### FairScene: Learning Class-Disentangled 2D/3D Representations for Semantic Scene Completion
- **Authors:** Jia, Dian; Yu, Pei; Tang, Wei
- **Tags:** `camera` `class-disentanglement` `2D-3D-repr` `SSC` `autonomous-driving`
- **Link:** [CVF Open Access](https://openaccess.thecvf.com/content/WACV2026/papers/Jia_FairScene_Learning_Class-Disentangled_2D3D_Representations_for_Semantic_Scene_Completion_WACV_2026_paper.pdf)

---

### AAAI 2026

#### Vision-Only Gaussian Splatting for Collaborative Semantic Occupancy Prediction
- **Authors:** Chen, Cheng; Huang, Hao; Bagchi, Saurabh
- **Tags:** `camera` `gaussian-splatting` `collaborative` `multi-agent` `autonomous-driving`
- **arXiv:** https://arxiv.org/abs/2508.10936 | **AAAI:** https://ojs.aaai.org/index.php/AAAI/article/view/37269

#### SPSC: Sparse and Scalable Multi-Modal 3D Occupancy Prediction for Autonomous Driving
- **Authors:** Guo, Qingju; Li, Shuang; Xie, Binhui; Geng, Jing; Li, Wei
- **Tags:** `camera` `LiDAR` `multi-modal` `sparse` `scalable` `autonomous-driving`
- **AAAI:** https://ojs.aaai.org/index.php/AAAI/issue/view/733

#### HD²-SSC: High-Dimension High-Density Semantic Scene Completion for Autonomous Driving
- **Authors:** Yang, Zhiwen; Peng, Yuxin
- **Tags:** `camera` `high-density` `high-dimension` `SSC` `autonomous-driving`
- **arXiv:** https://arxiv.org/abs/2511.07925

#### Towards 3D Object-Centric Feature Learning for Semantic Scene Completion
- **Authors:** Wang, Weihua; Cui, Yubo; Lin, Xiangru; Li, Zhiheng; Fang, Zheng
- **Tags:** `camera` `object-centric` `SSC` `autonomous-driving`
- **arXiv:** https://arxiv.org/abs/2511.13031

#### Towards Temporal Fusion Beyond the Field of View for Camera-based Semantic Scene Completion
- **Authors:** Bae, Jongseong; Ha, Junwoo; Heo, Jinnyeong; Lee, Yeongin; Kim, Ha Young
- **Tags:** `camera` `temporal-fusion` `beyond-FoV` `SSC` `autonomous-driving`
- **arXiv:** https://arxiv.org/abs/2511.12498

#### SplatSSC: Decoupled Depth-Guided Gaussian Splatting for Semantic Scene Completion
- **Authors:** Qian, Rui; Cao, Haozhi; Deng, Tianchen; Yuan, Shenghai; Xie, Lihua
- **Tags:** `camera` `gaussian-splatting` `depth-guided` `SSC` `autonomous-driving`
- **arXiv:** https://arxiv.org/abs/2508.02261 | **GitHub:** https://github.com/Made-Gpt/SplatSSC

---

### ICLR 2026

#### PG-Occ: Progressive Gaussian Transformer with Anisotropy-aware Sampling for Open Vocabulary Occupancy Prediction
- **Authors:** Yan, Chi; Xu, Dan
- **Tags:** `camera` `gaussian` `transformer` `open-vocabulary` `anisotropy` `autonomous-driving`
- **OpenReview:** https://openreview.net/forum?id=mHFaflQv93

#### G²-Occ: Geometry-Guided Gaussian Primitives for Embodied Semantic Occupancy Prediction
- **Authors:** Sun, TianFang; Gong, Jingyu; Zhang, Zhizhong; Tan, Xin; Xie, Yuan
- **Tags:** `camera` `gaussian` `geometry-guided` `embodied` `indoor`
- **OpenReview:** https://openreview.net/forum?id=uw9MfZJmlb

#### S2GO: Streaming Sparse Gaussian Occupancy
- **Authors:** Park, Jinhyung; Peng, Chensheng; Hu, Yihan; Zheng, Wenzhao; Kitani, Kris; Zhan, Wei
- **Tags:** `camera` `gaussian` `sparse` `streaming` `temporal` `autonomous-driving`
- **OpenReview:** https://openreview.net/forum?id=z8ggdMlSco

---

### CVPR 2026

#### Dr.Occ: Depth- and Region-Guided 3D Occupancy from Surround-View Cameras for Autonomous Driving
- **Authors:** Zhu, Xubo; Zhang, Haoyang; He, Fei; Wu, Rui; Shan, Yanhu; Yang, Wen; Yu, Huai
- **Tags:** `surround-camera` `depth-guided` `region-guided` `autonomous-driving`
- **arXiv:** https://arxiv.org/abs/2603.01007

#### OccAny: Generalized Unconstrained Urban 3D Occupancy
- **Authors:** Cao, Anh-Quan; Vu, Tuan-Hung
- **Tags:** `camera` `generalized` `unconstrained` `urban` `autonomous-driving`
- **arXiv:** https://arxiv.org/abs/2603.23502

#### VG3S: Visual Geometry Grounded Gaussian Splatting for Semantic Occupancy Prediction
- **Authors:** Yan, Xiaoyang; Pei, Muleilan; Shen, Shaojie
- **Tags:** `camera` `gaussian-splatting` `visual-geometry` `autonomous-driving`
- **arXiv:** https://arxiv.org/abs/2603.06210

#### Can We Trust Unreliable Voxels? Exploring 3D Semantic Occupancy Prediction under Label Noise
- **Authors:** Li, Wenxin; Peng, Kunyu; Wen, Di; Zheng, Junwei; Wei, Jiale; Duan, Mengfei; Zhang, Yuheng; Fan, Rui; Yang, Kailun
- **Tags:** `camera` `label-noise` `robustness` `SSC` `autonomous-driving`
- **arXiv:** https://arxiv.org/abs/2603.06279

#### L2COcc: Lightweight Camera-Centric Semantic Scene Completion via Distillation of LiDAR Model
- **Authors:** Wang, Ruoyu; Ma, Yukai; Yao, Yi; Tao, Sheng; Li, Haoang; Zhu, Zongzhi; Liu, Yong; Zuo, Xingxing
- **Tags:** `camera` `LiDAR-distillation` `lightweight` `SSC` `autonomous-driving`
- **arXiv:** https://arxiv.org/abs/2503.12369

#### OccuFly: A 3D Vision Benchmark for Semantic Scene Completion from the Aerial Perspective
- **Authors:** Gross, Markus; Matha, Sai B.; Fahmy, Aya; Song, Rui; Cremers, Daniel; Meess, Henri
- **Tags:** `aerial-camera` `benchmark` `SSC` `aerial`
- **arXiv:** https://arxiv.org/abs/2512.20770 | **GitHub:** https://github.com/markus-42/OccuFly

#### An Instance-Centric Panoptic Occupancy Prediction Benchmark for Autonomous Driving
- **Authors:** Feng, Yi; E, Junwu; Guo, Zizhan; Ma, Yu; Wang, Hanli; Fan, Rui
- **Tags:** `camera` `instance-centric` `panoptic` `benchmark` `autonomous-driving`
- **arXiv:** https://arxiv.org/abs/2603.27238

---

## Thematic Clusters

### 1. Gaussian Splatting for Occupancy (5 papers)
> A dominant trend in 2026: using 3D Gaussian primitives as the scene representation backbone.

- Vision-Only GS Collab. (AAAI) — multi-agent collaborative setting
- SplatSSC (AAAI) — depth decoupling
- PG-Occ (ICLR) — open-vocabulary + anisotropy-aware sampling
- G²-Occ (ICLR) — embodied / geometry-guided
- VG3S (CVPR) — visual geometry grounding
- S2GO (ICLR) — sparse + streaming

### 2. Depth / Geometry Guided (3 papers)
> Explicitly incorporating geometric cues (depth maps, geometry priors) to improve 3D reconstruction.

- SplatSSC (AAAI)
- G²-Occ (ICLR)
- Dr.Occ (CVPR)

### 3. Temporal Reasoning (2 papers)
> Extending occupancy models across time — either forecasting or fusing temporal context.

- ForecastOcc (3DV) — future occupancy prediction
- Temporal Fusion Beyond FoV (AAAI) — temporal context beyond camera field of view
- S2GO (ICLR) — streaming/online temporal setting

### 4. Lightweight / Efficient / Sparse (3 papers)
> Addressing scalability and deployment efficiency.

- SPSC (AAAI) — sparse + scalable multi-modal
- S2GO (ICLR) — sparse Gaussian, streaming
- L2COcc (CVPR) — lightweight via LiDAR-to-camera distillation

### 5. Novel Domains / Benchmarks (3 papers)
> Expanding occupancy prediction beyond standard AD front/surround cameras.

- SGFormer (3DV) — satellite + ground fusion
- OccuFly (CVPR) — aerial perspective benchmark
- G²-Occ (ICLR) — embodied (indoor) setting
- Instance-Centric Panoptic Occ (CVPR) — panoptic benchmark for AD

### 6. Robustness / Representation Quality (3 papers)
> Improving representation or handling real-world challenges.

- FairScene (WACV) — class imbalance via disentanglement
- HD²-SSC (AAAI) — high-density high-dimension voxel repr.
- Can We Trust Unreliable Voxels? (CVPR) — label noise robustness
- 3D Object-Centric SSC (AAAI) — object-level feature learning

### 7. Open-Vocabulary / Generalized (2 papers)
> Moving beyond fixed class sets toward open or unconstrained recognition.

- PG-Occ (ICLR)
- OccAny (CVPR)

---

## Papers to Prioritize (AD Semantic Occupancy Main Track)

| Priority | Paper | Reason |
|----------|-------|--------|
| ★★★ | PG-Occ (ICLR) | Open-vocab + Gaussian Transformer, novel direction |
| ★★★ | S2GO (ICLR) | Streaming sparse Gaussian, practical deployment |
| ★★★ | OccAny (CVPR) | Generalized unconstrained urban, broad applicability |
| ★★★ | Dr.Occ (CVPR) | Depth+region guidance from surround cameras |
| ★★★ | L2COcc (CVPR) | LiDAR→Camera distillation, efficiency focus |
| ★★☆ | SPSC (AAAI) | Multi-modal sparse scalable |
| ★★☆ | VG3S (CVPR) | Visual geometry + Gaussian |
| ★★☆ | ForecastOcc (3DV) | Forecasting sub-task |
| ★☆☆ | OccuFly (CVPR) | Benchmark, different domain (aerial) |
| ★☆☆ | Instance-Centric Panoptic (CVPR) | Benchmark, panoptic extension |

---

## TODO (Next Steps)

- [ ] Fetch arXiv abstracts for each paper to fill in method details
- [ ] Add benchmark results (nuScenes mIoU / IoU) per paper
- [ ] Add BibTeX entries
- [ ] Verify arXiv IDs that are post-Aug-2025 (knowledge cutoff)

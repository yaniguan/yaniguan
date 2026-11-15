<p align="center">
  <img src="assets/header.svg" width="560" alt="Text, drawings and atoms flowing into one symmetry-aware model; the same molecule comes out, just held three different ways">
</p>

### Hi, I'm Yani. I build AI that respects physics, and I make it train fast.

Rotate a water molecule and it's still water. Charge an electrode and the whole interface rearranges. Most models have to learn the rules of nature the hard way. I build ones that know them from the start: molecules, materials, electrochemical interfaces, and the dynamics in between.

I'm a Ph.D. candidate in computational chemistry at UCLA (done December 2026). These days I'm drawn to LLM/VLM pretraining, post-training, alignment, and multimodal models for science.

<img src="assets/multiscale.svg" width="18" align="top"> **Scientist by training.** A chemical engineering Ph.D. spent on multi-scale modeling of electrochemical systems (DFT → MD → kMC → P2D → 3D simulation). Irreps, Clebsch–Gordan and spherical harmonics are my everyday tools.

<img src="assets/gpu.svg" width="18" align="top"> **Engineer by habit.** I build and tune GPU training pipelines on A100, H100 and H200. I profile with Nsight, read rooflines, and reach for FP8, cuEquivariance and torch.compile when a model is slower than it should be.

<img src="assets/posttrain.svg" width="18" align="top"> **Post-training, the big picture.** Offline SFT and DPO teach a model from the textbook. But under SFT, small errors pile up once the model runs on its own. On-policy RL (PPO, GRPO) fixes that with rollouts: the model leaves the textbook, tries things itself, and learns from what actually happens. A lot like life.

#### The cast

| | | |
|:-:|---|---|
| <img src="assets/wignerflow.svg" width="22"> | **[WignerFlow](https://github.com/yaniguan/WignerFlow)** | An E(3)-equivariant transformer that *writes* MD trajectories autoregressively, so it replaces the integrator. Public results so far are argon only, and I say so up front. |
| <img src="assets/ylm.svg" width="22"> | **[YLM](https://github.com/yaniguan/YLM)** | A language model that understands 3D. Text tokens attend to l ≥ 1 irreps through Clebsch–Gordan products, so directions, forces and handedness survive rotation. Equivariance error < 1e-9 in fp64. |
| <img src="assets/ouroboros.svg" width="22"> | **[ouroboros-ocsr](https://github.com/yaniguan/ouroboros-ocsr)** | Picture → SMILES with a C<sub>N</sub> steerable CNN encoder. It handles rotations and deliberately *not* reflections, because a mirror image flips stereocenters. |
| <img src="assets/verdict.svg" width="22"> | **VERDICT** · [arXiv:2608.22183](https://arxiv.org/abs/2608.22183) | Four structure recognizers vote, and when they disagree that flags a wrong structure. No labels needed. AUROC 0.916; chemists rated 400 released labels at 0.995 precision. |
| <img src="assets/labbench.svg" width="22"> | **[labbench-posttrain](https://github.com/yaniguan/labbench-posttrain)** | A LAB-Bench eval harness plus RL environments built from lab protocols. Rewards are verifiable, and there's an audit that checks whether the model found a way to cheat them. |
| <img src="assets/gpu.svg" width="22"> | **[equivariant-gpu-lab](https://github.com/yaniguan/equivariant-gpu-lab)** | Where the physics meets the hardware: roofline analysis of O(3)-equivariant models, Morton-order graph locality, FP8 spherical scaling. |

#### <img src="assets/posttrain.svg" width="20" align="top"> The plot twist

On image-to-SMILES I ran LoRA SFT on three open VLMs and got **59.8%** exact match on 331 journal figures (MolScribe gets 58.3%). Then DPO pushed preference accuracy to **90–97%**, and exact match dropped to **0–2%**.

The DPO numbers looked great on paper. **I kept SFT.** The model had gotten good at being preferred and stopped getting the molecule right, and I'd rather ship the version that's actually correct.

<sub>Same habit, smaller scale: when e3nn or NVIDIA NeMo RL break, I file the bug upstream.</sub>

#### Intermission

<img src="assets/camera.svg" width="18" align="top"> a Canon R5 and a 6D Mark II &nbsp;·&nbsp;
<img src="assets/book.svg" width="18" align="top"> Shakespeare (*"there are more things in heaven and earth…"*) &nbsp;·&nbsp;
<img src="assets/road.svg" width="18" align="top"> very long drives to very empty places

<img src="assets/home.svg" width="18" align="top"> More at **[yaniguan.github.io](https://yaniguan.github.io)**

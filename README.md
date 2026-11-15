<p align="center">
  <img src="assets/header.svg" width="780" alt="Physics from DFT to full cells feeds many kinds of input into one symmetry-aware core. Out come SMILES, argon MD frames, a molecule that stays the same however it is turned, and a vote that flags wrong structures. Underneath: pretraining, SFT, DPO and on-policy RL, running on A100, H100 and H200 GPUs.">
</p>

<p align="center"><b>Rotate a molecule and it's still the same molecule. I build models that know this from the start, and make them train fast.</b></p>

<p align="center"><sub>Ph.D. at UCLA, done December 2026 &nbsp;·&nbsp; molecules, materials, electrochemical interfaces &nbsp;·&nbsp; DFT → MD → kMC → P2D → 3D</sub></p>

<br>

I pretrain equivariant foundation models for molecules and electrolytes, and I care just as much about the hardware: training pipelines on A100, H100 and H200, profiled with Nsight, tuned with FP8, cuEquivariance and torch.compile. Lately: post-training, alignment, and multimodal models for science.

<br>

<table>
  <tr><th colspan="3" align="left"><sub>SEE &nbsp;·&nbsp; read the world as it is drawn</sub></th></tr>
  <tr>
    <td><img src="assets/ouroboros.svg" width="22"> <a href="https://github.com/yaniguan/ouroboros-ocsr"><b>ouroboros-ocsr</b></a></td>
    <td>Picture → SMILES. A C<sub>N</sub> steerable encoder that handles rotations but not mirrors, because a mirror flips stereocenters.</td>
    <td align="right"><b>54.0%</b><br><sub>exact match, 298 real figures</sub></td>
  </tr>
  <tr>
    <td><img src="assets/verdict.svg" width="22"> <b>VERDICT</b><br><sub><a href="https://arxiv.org/abs/2608.22183">arXiv:2608.22183</a></sub></td>
    <td>Four structure recognizers vote. Disagreement flags a wrong structure, no labels needed.</td>
    <td align="right"><b>0.916</b><br><sub>AUROC</sub></td>
  </tr>
  <tr><th colspan="3" align="left"><sub>MODEL &nbsp;·&nbsp; physics built in, not learned the hard way</sub></th></tr>
  <tr>
    <td><img src="assets/wignerflow.svg" width="22"> <a href="https://github.com/yaniguan/WignerFlow"><b>WignerFlow</b></a></td>
    <td>An E(3)-equivariant transformer that replaces the MD integrator, 50 fs per step. Public results are argon only, and I say so up front.</td>
    <td align="right"><b>25.8 ns/day</b><br><sub>argon, one A100</sub></td>
  </tr>
  <tr>
    <td><img src="assets/ylm.svg" width="22"> <a href="https://github.com/yaniguan/YLM"><b>YLM</b></a></td>
    <td>A language model that reads 3D. Text attends to l ≥ 1 irreps via Clebsch–Gordan, so forces and handedness survive rotation.</td>
    <td align="right"><b>&lt; 1e-9</b><br><sub>equivariance error, fp64</sub></td>
  </tr>
  <tr><th colspan="3" align="left"><sub>TRAIN &nbsp;·&nbsp; make it learn, make it run fast</sub></th></tr>
  <tr>
    <td><img src="assets/labbench.svg" width="22"> <a href="https://github.com/yaniguan/labbench-posttrain"><b>labbench-posttrain</b></a></td>
    <td>LAB-Bench evals and RL environments from lab protocols, with verifiable rewards and an audit for reward cheating.</td>
    <td align="right"><b>49,139</b><br><sub>records, 20 sources</sub></td>
  </tr>
  <tr>
    <td><img src="assets/gpu.svg" width="22"> <a href="https://github.com/yaniguan/equivariant-gpu-lab"><b>equivariant-gpu-lab</b></a></td>
    <td>Equivariant models meet the hardware: roofline, Morton-order graph locality, FP8 spherical scaling.</td>
    <td align="right"><b>A100 → H100</b><br><sub>roofline</sub></td>
  </tr>
</table>

<br>

<img src="assets/posttrain.svg" width="18" align="top"> **On post-training.** SFT and DPO learn from the textbook; on-policy RL (PPO, GRPO) leaves it and learns from its own rollouts. And when DPO pushed preference accuracy to 90–97% but dropped exact match on 331 journal figures from 59.8% to 0–2%, I kept SFT.

<img src="assets/road.svg" width="18" align="top"> <img src="assets/paw.svg" width="18" align="top"> <img src="assets/camera.svg" width="18" align="top"> <img src="assets/book.svg" width="18" align="top"> &nbsp;Off the clock: a very long drive to a very empty place, my partner riding shotgun, my dog in charge of the back seat, a Canon R5 and a 6D Mark II for the light, and Shakespeare to remind me there are more things in heaven and earth than are dreamt of in any loss function.

<br>

<img src="assets/home.svg" width="18" align="top"> [yaniguan.github.io](https://yaniguan.github.io)

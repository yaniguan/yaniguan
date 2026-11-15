<p align="center">
  <img src="assets/header.svg" width="780" alt="Small biomolecules, catalyst surfaces, crystals and interfaces, from molecules to micro-environments to living cells and devices, feed many kinds of input into one symmetry-aware core. Out come SMILES, argon MD frames, a molecule that stays the same however it is turned, and a vote that flags wrong structures. Underneath: pretraining, SFT, DPO and on-policy RL, running on A100, H100 and H200 GPUs.">
</p>

<p align="center"><b>I build AI that already knows the laws of physics, and I make it train fast.</b></p>

<p align="center"><sub>Ph.D. at UCLA, done December 2026 &nbsp;·&nbsp; small biomolecules, catalysts, semiconductors, interfaces &nbsp;·&nbsp; quantum to device scale</sub></p>

<br>

I pretrain equivariant foundation models on molecules and materials, and I care just as much about the hardware: training pipelines on A100, H100 and H200, profiled with Nsight and tuned down to FP8. Lately: post-training, alignment, and multimodal models for science.

<sub>Math: linear algebra, group and representation theory, probability and statistics, optimization. Physics: quantum mechanics, statistical mechanics, electrochemistry, transport.</sub>

<br>

<table>
  <tr>
    <td width="33%" valign="top"><sub>SEE</sub><br><br><img src="assets/ouroboros.svg" width="20" align="top"> <a href="https://github.com/yaniguan/ouroboros-ocsr"><b>ouroboros-ocsr</b></a><br><sub>molecule images to SMILES</sub><br><b>54.0%</b> <sub>exact match</sub><br><br><img src="assets/verdict.svg" width="20" align="top"> <a href="https://arxiv.org/abs/2608.22183"><b>VERDICT</b></a><br><sub>label-free error flags</sub><br><b>0.916</b> <sub>AUROC</sub></td>
    <td width="33%" valign="top"><sub>MODEL</sub><br><br><img src="assets/wignerflow.svg" width="20" align="top"> <a href="https://github.com/yaniguan/WignerFlow"><b>WignerFlow</b></a><br><sub>equivariant MD, argon so far</sub><br><b>25.8 ns/day</b> <sub>one A100</sub><br><br><img src="assets/ylm.svg" width="20" align="top"> <a href="https://github.com/yaniguan/YLM"><b>YLM</b></a><br><sub>a language model that reads 3D</sub><br><b>&lt; 1e-9</b> <sub>equivariance error</sub></td>
    <td width="33%" valign="top"><sub>TRAIN</sub><br><br><img src="assets/labbench.svg" width="20" align="top"> <a href="https://github.com/yaniguan/labbench-posttrain"><b>labbench-posttrain</b></a><br><sub>RL from wet-lab protocols</sub><br><b>49,139</b> <sub>records</sub><br><br><img src="assets/gpu.svg" width="20" align="top"> <a href="https://github.com/yaniguan/equivariant-gpu-lab"><b>equivariant-gpu-lab</b></a><br><sub>equivariance meets the GPU</sub><br><b>A100 → H100</b> <sub>roofline</sub></td>
  </tr>
</table>

<br>

<img src="assets/posttrain.svg" width="18" align="top"> **On post-training.** SFT and DPO learn from the textbook; on-policy RL (PPO, GRPO) leaves it and learns from its own rollouts. And when DPO pushed preference accuracy to 90–97% but dropped exact match on 331 journal figures from 59.8% to 0–2%, I kept SFT.

<img src="assets/road.svg" width="18" align="top"> <img src="assets/paw.svg" width="18" align="top"> <img src="assets/camera.svg" width="18" align="top"> <img src="assets/book.svg" width="18" align="top"> &nbsp;Off the clock: long empty roads, my dog running the back seat, two Canons, and more things in heaven and earth than any loss function.

<br>

<img src="assets/home.svg" width="18" align="top"> [yaniguan.github.io](https://yaniguan.github.io)

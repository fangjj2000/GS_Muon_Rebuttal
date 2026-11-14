### Table G: Geometric diagnostics around task transitions

**Experimental setting.** Matched-state geometry on Qwen2.5-1.5B, seed 0. Fresh matched-state rerun with the first 500 examples per task and transitions at steps 500/1000. All metrics come from model.layers.{0,14,27}.self_attn.q_proj.weight and model.layers.{0,14,27}.mlp.up_proj.weight (six matrix blocks), sampled every 10 updates.

| Access | Task-shift stream | Delta_orient | Delta_A | Fraction rho<1 | Residual ratio c |  Mean $\Delta_\mathcal M$ |
| --- | --- | --- | --- | --- | --- | --- |
| FO | SST-2 -> WiC | 3.30081 | 0.115166 | 0.937482 | 0.894939 |  0.403101 |
| FO | SQuAD -> DROP | 1.1412 | 0.0485753 | 0.981305 | 0.74938 |  0.24966 |
| FO | WSC -> ReCoRD -> SQuAD | 1.07088 | 0.0911304 | 0.912674 | 0.615392 | 0.187122 |
| ZO | SST-2 -> WiC | 0.143565 | 0.0521078 | 0.968347 | 0.79073 |  0.484592 |
| ZO | SQuAD -> DROP | 0.143817 | 0.0473581 | 0.966667 | 0.78904 |  0.433938 |
| ZO | WSC -> ReCoRD -> SQuAD | 0.143762 | 0.0493341 | 0.95 | 0.801753 |  0.459169 |

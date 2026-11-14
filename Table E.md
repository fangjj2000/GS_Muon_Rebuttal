### Table E: Hyperparameter and reproducibility record

**Experimental setting.** The single-task experiments used 1,000 stream positions and the same stream for hyperparameter selection and score reporting.

| Experiment | Hyperparameter | Candidate values / fixed setting |
| --- | --- | --- |
| AdamW (FO) | Learning rate / betas / optimizer epsilon | {5e-6, 1e-5, 2e-5} / (0.9, 0.999) / 1e-8 |
| FT-Muon (FO) | Learning rate / momentum / NS steps | {5e-5, 1e-4, 2e-4} / 0.95 / 5 |
| GS-Muon (FO) | Learning rate / momentum / steering $\alpha$ / NS steps | {5e-5, 1e-4, 2e-4} / {0.8, 0.9, 0.95} / {0.05, 0.1, 0.2} / 3 + steering + 1 |
| Mixing (FO) | Learning rate / momentum / mixing $\lambda$ | {5e-5, 1e-4, 2e-4} / 0.95 / 0.1 for matched comparison |
| Adaptive Momentum (FO) | Learning rate / maximum momentum | {5e-5, 1e-4, 2e-4} / 0.95 |
| Shared ZO | Perturbation scale $\epsilon$ / direction / samples | {1e-4, 1e-3, 1e-2} / one-sided / 1 |
| MeZO | Learning rate | {5e-8, 1e-7, 2e-7} |
| HiZOO | Learning rate / Hessian smoothing | {2.5e-7, 5e-7, 1e-6} / constant1e-4 |
| SubZero | Learning rate / rank / basis refresh | {5e-8, 1e-7, 2e-7} / 48 / 50 steps (U and V together) |
| LOZO | Learning rate / rank / basis refresh | {5e-8, 1e-7, 2e-7} / 4 / 100 steps |
| FT-Muon (ZO) | Learning rate / estimator / momentum / rank / refresh | {5e-6, 1e-5, 2e-5} / SubZero / 0.95 / 48 / 50 steps |
| GS-Muon (ZO) | Learning rate / estimator / rank / refresh / momentum / steering $\alpha$ / NS steps | {5e-6, 1e-5, 2e-5} / SubZero / 48 / 50 steps / {0.8, 0.9, 0.95} / {0.05, 0.1, 0.2} / 3 + steering + 1 |
| Mixing (ZO) | Learning rate / estimator / rank / refresh / mixing $\lambda$ | {5e-6, 1e-5, 2e-5} / SubZero / 48 / 50 steps / 0.1 for matched comparison |
| Adaptive Momentum (ZO) | Learning rate / estimator / rank / refresh / maximum momentum | {5e-6, 1e-5, 2e-5} / SubZero / 48 / 50 steps / 0.95 |

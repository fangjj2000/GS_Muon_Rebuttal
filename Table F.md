### Table F: Runtime and Peak GPU Memory Across Model Scales (min / GiB)

**Experimental setting.** We profile the complete online stream of up to 1,000 examples per task for Qwen2.5-1.5B and Llama-3-8B. Each cell reports total runtime (minutes) / peak allocated GPU memory (GiB).

| Model | Method | SST-2 | RTE | CB | BoolQ | WSC | WiC | MultiRC | COPA | ReCoRD | SQuAD | DROP | Avg. |
|:--|:--|--:|--:|--:|--:|--:|--:|--:|--:|--:|--:|--:|--:|
| Qwen2.5-1.5B | GS-Muon (FO) | 33.02 / 15.62 | 32.48 / 15.63 | 8.49 / 15.63 | 32.53 / 15.64 | 18.28 / 15.63 | 32.38 / 15.63 | 32.92 / 15.66 | 12.92 / 15.62 | 36.54 / 15.64 | 34.00 / 15.63 | 33.48 / 15.64 | 27.91 / 15.63 |
| Qwen2.5-1.5B | GS-Muon (ZO) | 7.37 / 4.31 | 7.23 / 4.31 | 1.94 / 4.31 | 7.30 / 4.56 | 4.17 / 4.31 | 7.15 / 4.31 | 7.55 / 4.31 | 2.93 / 4.31 | 11.40 / 4.31 | 10.50 / 4.31 | 9.07 / 4.31 | 6.96 / 4.33 |
| Llama-3-8B | GS-Muon (FO) | 244.16 / 80.58 | 244.42 / 80.58 | 61.41 / 80.58 | 245.71 / 80.58 | 135.51 / 80.58 | 244.30 / 80.58 | 248.95 / 80.58 | 97.35 / 80.58 | 252.81 / 80.58 | 246.77 / 80.58 | 286.57 / 76.58 | 209.82 / 80.21 |
| Llama-3-8B | GS-Muon (ZO) | 15.39 / 18.16 | 15.48 / 18.16 | 4.14 / 18.16 | 15.97 / 18.16 | 8.45 / 18.16 | 15.37 / 18.16 | 19.09 / 18.16 | 6.17 / 18.16 | 22.45 / 18.16 | 18.42 / 18.17 | 23.86 / 18.17 | 14.98 / 18.16 |

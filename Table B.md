### Table B: First-order optimizer comparison on both model scales

**Experimental setting.** Compare AdamW, FT-Muon (five NS steps), and GS-Muon on Qwen2.5-1.5B and Llama-3-8B with exact FO gradients.

| Model / Method | SST-2 | RTE | CB | BoolQ | WSC | WiC | MultiRC | COPA | ReCoRD | SQuAD | DROP | Avg. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Qwen2.5-1.5B: AdamW (FO) | 83.0 | 84.1 | 72.4 | **79.6** | 50.7 | 52.6 | **78.9** | 80.3 | 51.3 | 73.9 | **55.8** | 69.3 |
| Qwen2.5-1.5B: FT-Muon (FO) | 86.7 | 83.9 | 80.0 | 78.9 | 50.4 | 51.4 | 76.3 | 80.0 | 56.6 | 85.1 | 48.6 | 70.7 |
| **Qwen2.5-1.5B: GS-Muon (FO)** | **88.5** | **84.6** | **82.4** | 79.1 | **52.9** | **61.5** | 78.7 | **81.5** | **57.0** | **85.9** | 49.8 | **72.9** |
| Meta-Llama-3-8B: AdamW (FO) | 87.7 | 79.7 | 70.2 | 75.7 | 49.8 | 51.2 | 69.1 | 87.5 | 72.8 | 88.4 | 65.3 | 72.5 |
| Meta-Llama-3-8B: FT-Muon (FO) | 90.9 | 80.5 | 65.2 | 61.2 | 51.8 | 50.5 | 74.4 | 88.3 | 74.4 | **89.4** | 70.4 | 72.5 |
| Meta-Llama-3-8B: GS-Muon (FO) | **91.0** | **81.7** | **71.6** | **79.8** | **52.5** | **56.2** | **79.3** | **88.8** | **74.8** | **89.4** | **71.0** | **76.0** |

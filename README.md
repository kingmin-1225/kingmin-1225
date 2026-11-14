### Min Wang

Undergraduate studying on-device AI inference optimization.
I learn by putting models on edge devices, measuring why they are slow, and making them faster.

- 🎓 Hanyang University ERICA, Artificial Intelligence, 3rd year
- 🔬 Interests: quantization (PTQ, QAT, low-bit LLMs), inference runtimes (TensorRT, llama.cpp), CUDA kernel profiling
- 📫 kingmin1225@hanyang.ac.kr

#### Projects

| Project | What I did |
|---|---|
| [python-BitLoRA-research](https://github.com/kingmin-1225/python-BitLoRA-research) | Ternary (1.58-bit) and binary LoRA adapters for Llama-3.2-3B-Instruct, compared with FP32 LoRA on a single 8 GB GPU. At r=8 the ternary adapter is 16× smaller (2.9 MB vs 46.4 MB), val loss 0.463 vs 0.451. A ternary r=16 adapter (5.8 MB) beats an FP32 r=4 adapter (23.2 MB) at 1/4 the size: 0.452 vs 0.460 |
| [EXAONE-1.2B-Quant](https://github.com/kingmin-1225/EXAONE-1.2B-Quant) | LG Aimers 8th, LLM compression hackathon. Training-free W4A16 GPTQ on EXAONE-4.0-1.2B. Keeping the sensitive K/V projections in full precision with act-order raised the score from 0.500 to 0.521; SmoothQuant brought it to 0.523 |
| [python-BitNet-study](https://github.com/kingmin-1225/python-BitNet-study) | Implemented BitNet b1.58 BitLinear (ternary weights, 8-bit activations, STE) in a vanilla Transformer and a Llama-style model |
| [gpt2-small-matmul](https://github.com/kingmin-1225/gpt2-small-matmul) | CUDA batched matmul for GPT-2 attention (QKᵀ, PV) with 32×32 shared-memory tiling and 2×2 thread coarsening, profiled step by step with Nsight Compute. 75× over the naive kernel, 89% of cuBLAS (970 µs vs 869 µs) on an RTX 4060 Ti |
| [icpbl-project-self-parking](https://github.com/kingmin-1225/icpbl-project-self-parking) | Two-person team. Built the reverse-parking path planner with bidirectional Hybrid A* |

[![Solved.ac Profile](http://mazassumnida.wtf/api/generate_badge?boj=lesserpanda)](https://solved.ac/lesserpanda)

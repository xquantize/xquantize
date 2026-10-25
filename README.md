## Zane Neave

**Machine Learning Engineer** · retrieval & search · real-time perception · efficient inference

MSc AI (First Class Hons). By day I lead ML at **Syos Aerospace**: real-time perception on Jetson / TensorRT, plus multi-sensor fusion and tracking for uncrewed vehicles. Outside work I build retrieval systems with proper evaluation, work on efficient LLM inference, and contribute to open-source ML.

### What I work on

- **Retrieval & search**: embedding-based image retrieval, hybrid dense + full-text search, Reciprocal Rank Fusion, evaluated with Hit@k, MRR and nDCG
- **Perception**: real-time detection and tracking, deployed to edge hardware as optimised TensorRT engines
- **Efficient inference**: quantization, KV-cache tooling, MLX builds for Apple Silicon
- **Evaluation**: reproducible harnesses, significance testing, honest negative results

### Selected projects

| Project | What it is |
|---|---|
<!-- | [TODO-retrieval-repo](https://github.com/xquantize/TODO) | TODO: one-line description + headline metric | -->
| [pgvector-rag-pipeline](https://github.com/xquantize/pgvector-rag-pipeline) | Hybrid vector + full-text RAG in PostgreSQL / pgvector, fused with RRF in pure SQL. Evaluation harness: Hit@5 100%, MRR 0.90, nDCG@5 0.93. Runs fully offline on local models. In progress |
| [meta-ts-correction](https://github.com/xquantize/meta-ts-correction) | Can a tiny corrector recover a frozen time-series foundation model's (Chronos-Bolt) accuracy at a fraction of the compute? Leakage-audited harness validated against M4 Naive2, with Wilcoxon / Diebold–Mariano / Holm testing. In progress |
| [eqx-zoo](https://github.com/xquantize/eqx-zoo) | Verified Equinox ports of pretrained models, numerically matched against Hugging Face |
| [rl-playground](https://github.com/xquantize/rl-playground) | From-scratch PPO in PyTorch, verified against Stable-Baselines3 on a custom racing environment, with multi-seed ablations |
| [swellsense](https://github.com/xquantize/swellsense) | A surf assistant for New Zealand surfers that answers questions about boards, swell, spots and safety from cited sources |

### Open source

Merged contributions focused on device-agnostic support (Apple Silicon / MPS / CPU), correctness fixes and KV-cache tooling.

- **Hugging Face Accelerate**: report MPS as the accelerator in `accelerate env` ([#4158](https://github.com/huggingface/accelerate/pull/4158))
- **MLX-LM** (Apple): validate adapter tensors when loading adapters ([#1727](https://github.com/ml-explore/mlx-lm/pull/1727)); fix an off-by-one in size parsing caused by float truncation ([#1726](https://github.com/ml-explore/mlx-lm/pull/1726))
- **KVCache-Factory**: device-agnostic input placement for MPS / CPU ([#66](https://github.com/Zefan-Cai/KVCache-Factory/pull/66)); fix model max length ([#67](https://github.com/Zefan-Cai/KVCache-Factory/pull/67))
- **Hugging Face Transformers** *(in review)*: image-text contrastive loss for BLIP-2 image-text retrieval ([#48583](https://github.com/huggingface/transformers/pull/48583))

[All pull requests →](https://github.com/pulls?q=is%3Apr+author%3Axquantize)

### Practice

I keep my fundamentals sharp by implementing ML from scratch: deep learning, linear algebra, optimisation and classical ML.

- [Deep-ML](https://www.deep-ml.com/profile/y5eQDK23TydlcwRhgUfZwKolL0D2): actively solving problems · solutions and labs in [deep-ml](https://github.com/xquantize/deep-ml)
- [TensorTonic](https://www.tensortonic.com/profile/xquantize)

### Models & datasets

- [K2-geoscience-7B (4-bit MLX)](https://huggingface.co/xquantize/k2-geoscience-7b-4bit-mlx): the first MLX build of a geoscience LLM
- [Global natural events 2011–2026](https://huggingface.co/datasets/xquantize/global-natural-events-eonet-2011-2026): ~41.6k events from NASA EONET
- [Global earthquakes 2020–2026](https://huggingface.co/datasets/xquantize/Global-Earthquakes-2020-2026): ~11.8k events

### Stack

Python · PyTorch · Transformers · MLX · TensorRT · ONNX · PostgreSQL / pgvector · OpenCV · C++ · ROS2 · Docker

### Connect

[LinkedIn](https://www.linkedin.com/in/zane-neave-rex/) · [Hugging Face](https://huggingface.co/xquantize) · [Deep-ML](https://www.deep-ml.com/profile/y5eQDK23TydlcwRhgUfZwKolL0D2) · [TensorTonic](https://www.tensortonic.com/profile/xquantize) · [Kaggle](https://www.kaggle.com/zaneneave) · [ORCID](https://orcid.org/0009-0005-1559-1426)

<sub>off the clock: surfing · football · somewhere on the coast</sub>

## Ashritha Gonuguntla

Carnegie Mellon University. I work on **whether AI systems actually do what we
claim they do**: evaluation that holds up, and the systems engineering
underneath it.

Most of my recent work follows one thread: the standard way to measure something
is often subtly invalid, and measuring it properly changes the answer.

### Publications

**[The Plan, Not the Decoder](https://arxiv.org/abs/2608.21713)** · MUCG Workshop @ ECCV 2026 (**oral**)
Reasoning-augmented text-to-image models emit a machine-readable plan before
decoding. I show compositional failures originate in the plan rather than the
decoder, and repair them at inference time by editing the plan alone.
[code](https://github.com/AshrithaG/compositional-t2i-diagnostics)

**[The Replay Gap](https://arxiv.org/abs/2608.08239)** · Efficient Reasoning Workshop @ COLM 2026
Every LLM-routing benchmark scores routers by replaying logged trajectories. In a
multi-step agent that is unsound. ~900 branching rollouts show early model swaps
diverge at the first post-fork action 74–77% of the time, leaving ~3% of replayed
states valid.
[code](https://github.com/AshrithaG/replay-gap) ·
[data](https://huggingface.co/datasets/ashritha0907/replay-gap-trajectories) ·
[page](https://ashrithag.github.io/replay-gap/)

### Selected work

| | |
|---|---|
| **[nanoinfer](https://github.com/AshrithaG/nanoinfer)** | Inference engine from scratch in C++: own conv kernels, liveness-based memory planner, int8 quantization. Within 1% of ONNX Runtime on dense models, and honest about the 1.3–1.7× gap on depthwise ones. Its int8 GEMM reaches 122.8 TOPS in hand-written CUDA and 540 TOPS in Triton, matching cuBLAS once cuBLAS is called in its fast layout. |
| **[batch-invariance](https://github.com/AshrithaG/batch-invariance)** | What determinism costs in vLLM. The batch-invariant mode holds with CUDA graphs on (0 of 30 prompts change, against 13 of 30 by default) and costs 54 to 67% of throughput, because its kernels are slower. |
| **[specdec](https://github.com/AshrithaG/specdec)** | Speculative decoding from scratch. It loses at every window size, and the reason is one number: a 0.6B draft pass costs 0.649 of a 4B target pass, which is also the break-even acceptance rate. |
| **[query-rewrite-eval](https://github.com/AshrithaG/query-rewrite-eval)** | Does ROUGE measure query rewriting? Across systems that genuinely differ, it ranks them close to backwards from retrieval quality (Kendall tau -0.73 to -0.87). Includes a hand-written sharded BM25 index. |
| **[mlops-replay](https://github.com/AshrithaG/mlops-replay)** | An MLOps platform evaluated rather than merely built: nine years of NYC taxi data replayed monthly, with a measured detection rate and false-alarm rate for its own monitoring. |
| **[gated-residual-rl](https://github.com/AshrithaG/gated-residual-rl)** | A learned gate decides when to override a frozen base policy on contact-rich peg insertion. 85% success vs 45% base, intervening in 66% of timesteps. |
| **[gridpilot](https://github.com/AshrithaG/gridpilot)** | An LLM agent operating a simulated power grid during cascading failure: IEEE 118-bus physics, verified tools, simulate-before-apply guardrail, 50-incident benchmark. |
| **[federated-fault-diagnosis](https://github.com/AshrithaG/federated-fault-diagnosis)** | FedAvg vs FedProx on CWRU bearing data under non-IID clients, partial participation, and stragglers. |

📫 agonugun@andrew.cmu.edu
